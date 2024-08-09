<script setup>
import { RouterLink } from "vue-router";
</script>

<template>
  <header>
    <nav class="container">
      <div class="branding">
        <img src="@/assets/Vue_Logo_Black.png" alt="" />
        <h1>Туду на Vue</h1>
      </div>
      <ul class="nav-routes">
        <RouterLink :to="{ name: 'todos' }">Задачи</RouterLink>
        <RouterLink :to="{ name: 'about' }">О нас</RouterLink>
      </ul>
    </nav>
  </header>
</template>

<style lang="scss" scoped>
header {
  background-color: #b8e2d1;
  nav {
    display: flex;
    align-items: center;
    padding: 25px 16px;

    .branding {
      display: flex;
      align-items: center;
      gap: 8px;
      img {
        max-width: 50px;
      }

      h1 {
        font-size: 24px;
      }
    }

    .nav-routes {
      display: flex;
      flex: 1;
      justify-content: flex-end;
      gap: 12px;
      list-style: none;

      a {
        text-decoration: none;
        color: inherit;
      }
    }
  }
}
</style>
