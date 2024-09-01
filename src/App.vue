<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import WelcomeHeading from './components/WelcomeHeading.vue'
</script>

<template>
  <div class="wrapper">
    <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="125" height="125" />
    <div class="right-part">
      <div class="top-part">
        <WelcomeHeading />
        <nav>
          <RouterLink to="/"> Home </RouterLink>
          <RouterLink to="/author"> Author </RouterLink>
        </nav>
      </div>
      <RouterView />
    </div>
  </div>
</template>

<style scoped>
.wrapper {
  display: flex;
  flex-direction: column;
}

.right-part {
  display: flex;
  flex-direction: column;
}

.logo {
  display: block;
  margin: 0 auto 1rem;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin: 1rem 0;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  .wrapper {
    flex-direction: row;
    align-items: flex-start;
    gap: 10px;
  }

  .right-part{
    gap: 20px;
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;
  }
}
</style>
