<template>
    <h1>Product component</h1>
    <databind/>
</template>

<script>
import databind from './databind.vue'
export default {
    name:'products',
    components:{
        databind,
    }
}
</script>

<style>
    h1{
        margin: 20px;
        background-color: aqua;
    }
</style>