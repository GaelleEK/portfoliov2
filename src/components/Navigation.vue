<template>
  <nav class="navbar" role="navigation" aria-label="main navigation">
    <div class="navbar-brand">
      <router-link class="navbar-item" to="/">
        <img id="logo" class="image" src="../assets/img/LogoGEK1.png" />
      </router-link>

      <a id="burger" role="button" class="navbar-burger" :class="isActive" @click="open">
        <span aria-hidden="true"></span>
        <span aria-hidden="true"></span>
        <span aria-hidden="true"></span>
      </a>
    </div>

    <div id="navbar" class="navbar-menu" :class="isActive">
      <div class="navbar-start">
        <router-link to="/" class="navbar-item">Home</router-link>
        <router-link to="/about" class="navbar-item">About</router-link>
        <div class="navbar-item has-dropdown is-hoverable">
          <a class="navbar-link"> More </a>

          <div class="navbar-dropdown">
            <a class="navbar-item"> About </a>
            <a class="navbar-item"> Jobs </a>
            <a class="navbar-item"> Contact </a>
            <hr class="navbar-divider" />
            <a class="navbar-item"> Report an issue </a>
          </div>
        </div>
      </div>

      <div class="navbar-end">
        <div class="navbar-item">
          <div class="buttons">
            <a class="button is-primary">
              <strong>Sign up</strong>
            </a>
            <a class="button is-light"> Log in </a>
          </div>
        </div>
      </div>
    </div>
  </nav>
</template>
<script lang="ts">
import { defineComponent } from "vue";

const Navigation = defineComponent({
  data() {
    return {
      isActive: "",
    };
  },
  methods: {
    open() {
      if (this.isActive === "") {
        this.isActive = "is-active";
      } else {
        this.isActive = "";
      }
    },
  },
});
export default Navigation;
</script>
