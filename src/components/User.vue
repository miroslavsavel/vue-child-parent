<template>
<div>
    <h2>User Component as child component</h2>
    <!-- <button>Send username to parent</button>  -->
</div>
</template>

<script>
/* eslint-disable vue/no-unused-components */
export default {
  components: { },
    name: "User",
    data()
    {
        return {
           userName: "Peter" 
        }
    }
}
</script>

<style>

</style>