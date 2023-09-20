<template>
  <div class="app-container">
    <header>
      <div class="logo">Johann Ogbebor</div>
      <nav>
        <ul>
          <li><router-link to="/">Home</router-link></li>
          <li><router-link to="/about">About</router-link></li>
          <li><router-link to="/projects">Projects</router-link></li>
          <li><router-link to="/contact">Contact</router-link></li>
        </ul>
      </nav>
    </header>
    
    <main>
      <router-view></router-view>
    </main>

    <footer>
      <FooterComponent />
    </footer>
  </div>
</template>

<script setup>
import { RouterLink, RouterView } from 'vue-router'
import FooterComponent from './components/FooterComponent.vue';
</script>

<style scoped>
/* Reset some default styles */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: Arial, sans-serif;
  background-color: #f4f4f4;
}

/* Styling for the entire app container */
.app-container {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}

/* Header styles */
header {
  background-color: #333;
  color: #fff;
  padding: 1rem;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo {
  font-size: 1.5rem;
  font-family: Arial;
}

nav ul {
  list-style: none;
  display: flex;
  gap: 1rem;
}

nav ul li {
  margin-right: 1rem;
}

nav ul li a {
  text-decoration: none;
  color: #fff;
  transition: color 0.3s;
}

nav ul li a:hover {
  color: #6f7173;
}

/* Main content styles */
main {
  flex-grow: 1;
  padding: 2rem;
}

/* Footer styles */
footer {
  background-color: #333;
  color: #fff;
  text-align: center;
  padding: 1rem;
}

/* Media query for small screens */
@media (max-width: 768px) {
  header {
    flex-direction: column;
    align-items: flex-start;
  }

  nav ul {
    flex-direction: column;
  }

  nav ul li {
    margin-right: 0;
    margin-bottom: 0.5rem;
  }
}
</style>
