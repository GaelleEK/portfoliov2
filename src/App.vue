<template>
  <Navigation />
  <router-view />
</template>
<script lang="ts">
import Navigation from "./components/Navigation.vue";
export default {
  name: "App",
  components: {
    Navigation,
  },
};
</script>

<style>
@import "./assets/styles/styles.css";
</style>
