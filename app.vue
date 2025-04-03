<template>
  <div class="site-container">
    <MenuSuperior />
    <Home />
    <QuemSomos />

    <section id="agenda">
      <h1>Agenda</h1>
    </section>
    <section id="convites">
      <h1>Convites</h1>
    </section>
    <section id="redes-sociais">
      <h1>Redes Sociais</h1>
    </section>
  </div>
</template>

<script setup>
import MenuSuperior from './components/MenuSuperior.vue';
import Home from './components/Home.vue';
import QuemSomos from './components/QuemSomos.vue';
</script>

<style>
html, body {
  margin: 0;
  padding: 0;
  background-color: #0E0124 !important;
  color: white;
  scroll-behavior: smooth;
  overflow-x: hidden;
  min-height: 100vh;
}

.site-container {
  width: 100%;
  min-height: 100vh;
  background-color: #0E0124;
}

section {
  min-height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  color: white;
  font-size: 2rem;
}
</style>
