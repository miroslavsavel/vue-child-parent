<template>
    <div class="child">
        <h1>Child Component</h1>
        <p>{{localData}}</p>
        <button @click="sendToParent()">Send data to parent</button>
    </div>
</template>

<script>
export default {
    props:["parentData"],
    data() {
        return {
            localData:null,
            childData: "How are you my parent?"
        }
    },
    created(){
        this.localData = this.parentData
    },
    methods:{
        sendToParent(){
            this.$emit('from-child',this.childData)
        }
    }
}
</script>

<style scoped>
.child{
    width:500px;
    height: 200px;
    background: grey;
    margin: auto;
    padding: 30px;
}
</style>