<template>
    <h1> Users component</h1>
    <h3 v-bind:style="{color:'blue'}">inline style binding</h3>
    <!-- display class will bind only when value of show is true -->

    <h3 v-bind:class="{display:show}">class binding w object</h3> 
    <h3 v-bind:class=[aclass]>class binding with array</h3>
    <h3 v-bind:class="[show?'yesclass':'noclass']">bind class dynamically w condition</h3>
</template>

<script>
export default {
    name:'user',
    data(){
        return{
            activeColor:'red',
            show:true,
            aclass:'arrclass'
        }
    }
} 
</script>

<style>
    h1{
        margin: 20px;
        background-color: rgb(136, 110, 77);
    }
    .display{
        background-color: cadetblue;
    }
    .arrclass{
        background-color: coral;
    }
</style>