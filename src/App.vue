<!-- App -->
<template>
  <div id="app">
    <Menu/>
    <Header/>
    <router-view />
    <Home/>
    <Footer/>
  </div>
</template>

<script>
  import Header from "./components/Header.vue";
  import Footer from "./components/Footer.vue";
  import Home from "./views/Home.vue";

  import "./css/bootstrap.min.css";
  import "./css/font-awesome.min.css";
  import "./css/templatemo-green.css";
  import Menu from "@/components/Menu";

  export default {
    name: 'App',
    components: {
      Menu,
      Home,
      Header,
      Footer
    }
  }
</script>

<!-- style global -->
<style>
  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
    background-color: #eae6e6;
  }
</style>
