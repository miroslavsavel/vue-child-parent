<template>
  <div>
    <Home><User></User></Home>
  </div>
</template>

<script>
import User from './components/User.vue'
import Home from './components/Home.vue'

export default {
  name: 'App',
  components: {
    User, Home
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
