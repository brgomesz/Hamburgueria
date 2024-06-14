<template>
  <div>
    <Navbar :logo="logo_src" :alt="app_name" />
  </div>
  <router-view></router-view>
  <div>
    <Footer />
  </div>
</template>

<script>
import Navbar from "./components/Navbar.vue";
import Footer from "./components/Footer.vue";
export default {
  components: {
    Navbar,
    Footer,
  },
  data() {
    return {
      logo_src: "/img/logo.png",
      app_name: "burger do brunão ",
    };
  },
};
</script>

<style>
* {
  font-family: Arial, Helvetica, sans-serif;
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

.main-conteiner {
  /* margin: 50px; */
  margin-bottom: 50px;
  min-height: 350px;
}

h1 {
  text-align: center;
  font-size: 42px;
  margin-bottom: 30px;
  color: #222;
}
</style>
