<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <price-format :price="1000000000000"></price-format>
  </div>
</template>

<script>
import PriceFormat from './components/PriceFormat.vue'

export default {
  name: 'app',
  components: {
    PriceFormat
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
