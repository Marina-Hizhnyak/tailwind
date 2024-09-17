<script setup>
import Nav from './Nav.vue';
import Footer from './Footer.vue';
import PrimaryButton from './PrimaryButton.vue';
</script>

<template>
  <div class="flex flex-col min-h-screen">
    <header>
      <Nav>Accueil</Nav>
    </header>

    <main class="flex-grow py-5">
      <div class="container mx-auto">
        <slot name="title" />
        <slot name="content" />
      </div>
      <PrimaryButton/>
    </main>

    <Footer />
  </div>
</template>