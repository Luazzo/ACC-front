<template>
  <div id="app">
    <StarterNavbar></StarterNavbar>

    <router-view/>

    <MainFooter></MainFooter>
  </div>
</template>

<script>

  import StarterNavbar from './layout/StarterNavbar';
  import MainFooter from './layout/MainFooter';
  export default {
    components: {
      StarterNavbar,
      MainFooter
    },
  }
</script>

<style>
  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }
</style>
