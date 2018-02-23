<template>
  <div id="app">

    <router-view/>
  </div>
</template>

<script>
  export default {
    name: 'App'
  }
</script>

<style>
  body {
    background-image: url("./assets/images/background.jpg");
    height: 100vh;
    background-size: cover;
    /* background-repeat: no-repeat; */
    background-position: center center;
    background-attachment: fixed;
  }
</style>