<template>
    <div>
        <h1>Parent component in Vue js 3</h1>
        <User></User>
        <p>{{childData}}</p>
        <div>
            <Child :parentData="fromParent" v-on:from-child="fromChild"/>
        </div>
    </div>
</template>

<script>
import User from './User.vue'
import Child from './Child'

export default {
    name: "Home",
    data:()=>({
        fromParent: "Hi, my Child",
        childData:null,
    }),
    methods:{
        fromChild(data){
            console.log('event chyteny')
            this.childData = data;
        }
    },
    components:{
        User, Child
    }
}
</script>

<style>
h1 {
    color: orange
}
</style>