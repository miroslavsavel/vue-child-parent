<template>
  <h1>Send Data Child to parent in Vue js 3</h1>
  <User></User>
</template>

<script>
import User from './User.vue'
export default {
    name: "Home",
    components:{
        User
    }
}
</script>

<style>
h1 {
    color: orange
}
</style>