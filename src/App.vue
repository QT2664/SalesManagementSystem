<template>
  <div id="app">
    <img src="./assets/logo.png">
    <!-- <router-view/> -->
    <!-- <HelloWorld></HelloWorld> -->
    <hello></hello>
    <!-- <template v-if="ok">
      <h2>´«²Î</h2>
    </template> -->
  </div>
</template>

<script>
import Hello from './components/Hello'
import HelloWorld from './components/HelloWorld'
export default {
  name: 'App',
  components: {
    Hello,
    HelloWorld
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
