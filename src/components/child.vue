<template>
    <p>child component</p>
   
    <li v-for="user in users" :key="user.name">
        {{user.name}} and mail id is {{user.mail}}
    </li>
</template>

<script>
export default {
    name:'child',
    props:['users']
}
</script>

<style>

</style>