<template>
  <HeaderTop/>
  <HelloWorld msg="Welcome to Your Vue.js App"/>
</template>

<script>
import HeaderTop from './components/HeaderTop.vue'
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    HeaderTop
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
}
</style>
