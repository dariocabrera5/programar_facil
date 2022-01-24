<template>
  <div id="app">
  <h1>HOLA DESDE APP</h1>
    <img src="./assets/logo.png">
    <Node/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld'
import Node from './components/Node.vue'

export default {
  name: 'App',
  components: {
    Node
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
