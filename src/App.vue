<template>
  <v-app class="main">
    <v-main>
      <HomePage />
      <div class="img"></div>
    </v-main>
  </v-app>
</template>

<script setup>
import HomePage from "./components/HomePage.vue";
</script>

<style scoped>
.main {
  background-color: hsl(225, 100%, 94%);
  background-image: url("/src/assets/pattern-background-desktop.svg");
  background-size: contain;
  background-position: center -80px;
  background-repeat: no-repeat;
  min-height: 100vh; /* Ensures it covers the full screen height */
  display: flex;
  justify-content: center;
  align-items: center;
}
@media (max-width: 720px) {
  /* Adjust the max-width to your medium breakpoint */
  .main {
    background-image: none; /* Remove the background image */
  }
}
</style>