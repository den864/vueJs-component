<template>
    <div style="background-color:grey">
        <h3>component inside products component</h3>
        {{message}}
        <br>
        <input type="text" v-model="message">
        <br><br><br>

        <p style="white-space:pre-line">{{newLineText}}</p>
        <textarea type="text" v-model="newLineText"/>
    </div>
</template>

<script>
export default {
    name:'databind',
    data(){
        return{
            message:'hi',
            newLineText:'new lin',
        }
    }
}
</script>

<style>

</style>