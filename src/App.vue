<template>
  <div>
    <TransformOne />
    <!-- <TransformTwo /> -->
  </div>
</template>

<script>
import TransformOne from './components/transformOne/index.vue';
// import TransformTwo from './components/transformTwo/index.vue';
export default {
  name: 'App',
  components: {
    TransformOne, 
    // TransformTwo
  }
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
