<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header>
    <nav>
      <RouterLink to="/">Home</RouterLink>
      <RouterLink to="/about">About</RouterLink>
    </nav>
  </header>

  <RouterView />
</template>

<style scoped>
nav {
  padding: 1rem 0;
  border-bottom: 1px solid var(--color-border);
}

nav a {
  margin-right: 1.5rem;
  color: var(--color-text);
  text-decoration: none;
}

nav a:hover,
nav a.router-link-exact-active {
  color: hsla(160, 100%, 37%, 1);
}
</style>
