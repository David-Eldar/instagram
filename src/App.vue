<template>
  <div id="app">
    
    <router-view />
  </div>
</template>

<script>
  
  export default {
    created() {
      this.$store.dispatch({type: 'loadPosts'})
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
  }
</style>
