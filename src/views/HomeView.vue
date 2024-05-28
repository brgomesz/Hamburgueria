<template>
  <div>
    <Banner />
  </div>
  <div class="main-conteiner">
    <h1>Monte o seu hamburguer</h1>
    <p>formulário</p>
  </div>
</template>

<script>
import Banner from "../components/Banner.vue";

export default {
  name: "Home",
  components: {
    Banner,
  },
};
</script>
