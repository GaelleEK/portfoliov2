<template>
  <div class="card">
    <div class="card-header">
      <p class="card-header-title">
        {{ projet.title }}
      </p>
    </div>
    <div class="card-image">
      <figure class="image is-4by3">
        <img :src="projet.imageUrl" alt="Placeholder image" />
      </figure>
    </div>
    <div class="card">
      <div class="card-content">
        <div class="content">
          {{ projet.description }}
        </div>
      </div>
    </div>
    <footer class="card-footer">
      <a href="#" class="card-footer-item">Lien Github</a>
    </footer>
  </div>
</template>
<script lang="ts">
// import { defineComponent } from "vue";
// const Projet = defineComponent({
//   data() {
//     return {
//       projet: {
//         title: "test",
//         description: "test",
//         imageUrl: "test",
//         lienGit: "test",
//       },
//     };
//   },
// });
// export default Projet;
</script>
