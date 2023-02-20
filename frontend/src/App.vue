<template>
  <div id="app">
    <MyDonut/>
  </div>
</template>

<script>
import MyDonut from './components/MyDonut.vue'

export default {
  name: 'App',
  components: {
    MyDonut: MyDonut
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
