<template>
  <div id="app">
    <Wireless />
  </div>
</template>

<script>
import Wireless from './components/Wireless.vue'

export default {
  name: 'App',
  components: {
    Wireless
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
