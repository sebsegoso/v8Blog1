<template>
  <div id="wrapper">
    <Navbar />
    <!-- ROUTER VIEW QUE CARGARÁ LAS VISTAS (INICIO, SOBRE MÍ, CONTACTO, ETC.) -->
    <div class="vista-router">
      <router-view></router-view>
    </div>
    <Footer />
  </div>
</template>

<script>
import Navbar from "./components/Navbar";
import Footer from "./components/Footer";
export default {
  components: {
    Navbar,
    Footer,
  },
};
</script>

<style lang="scss">
* {
  margin: 0;
  box-sizing: border-box;
  transition: all 1s ease;
}
#wrapper {
  background-color: #ddd;
  min-height: 100vh;
}
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.vista-router {
  padding-top: 56px;
}
.masthead {
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
  background-blend-mode: difference;
}
header {
  padding: 150px 0;
  color: #fff;
  text-shadow: 2px 2px 0 #000, 0 0 10px #777;
}
</style>
