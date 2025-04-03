<template>
  <nav class="top-menu">
    <ul>
      <li><a href="#home">Home</a></li>
      <li><a href="#quem-somos">Quem Somos</a></li>
      <li><a href="#agenda">Agenda</a></li>
      <li><a href="#convites">Convites</a></li>
      <li><a href="#redes-sociais">Redes Sociais</a></li>
    </ul>
  </nav>
</template>

<script setup>
import { onMounted } from 'vue';

onMounted(() => {
  document.querySelectorAll('nav a').forEach(anchor => {
    anchor.addEventListener('click', function (event) {
      event.preventDefault();
      const targetId = this.getAttribute('href');
      const targetElement = document.querySelector(targetId);
      if (targetElement) {
        window.scrollTo({
          top: targetElement.offsetTop,
          behavior: 'smooth'
        });
      }
    });
  });
});
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Alumni+Sans+SC:wght@400;700&display=swap');

.top-menu {
  position: fixed;
  top: 0;
  left: 50%;
  transform: translateX(-50%);
  background: rgba(0, 0, 0, 0.7);
  box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.5);
  padding: 10px 25px;
  border-radius: 0 0 15px 15px;
  z-index: 1000;
  display: flex;
  justify-content: center;
}

.top-menu ul {
  display: flex;
  list-style: none;
  padding: 0;
  margin: 0;
}

.top-menu li {
  margin: 0 25px;
}

.top-menu a {
  color: white;
  text-decoration: none;
  font-size: 14px;
  font-weight: semi-condensed;
  transition: color 0.3s;
  font-family: 'Alumni Sans SC', sans-serif;
}

.top-menu a:hover {
  color: #621EAA;
}

.quem-somos-section {
  min-height: 100vh;
  padding: 50px 20px;
}
</style>
