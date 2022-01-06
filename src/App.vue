<template>

  <user/>
  <products/>
  <child v-bind:users ='users'/>

</template>

<script>
import user from './components/user.vue'
import products from './components/products.vue'
import child from './components/child.vue'


export default {
  name: 'App',
  components: {
    user, 
    products,
    child,
  },
  data()
  {
    return {
      users:[
        {name:"tom",mail:"abc@mail.com"},
        {name:"john",mail:"john@mail.com"}
      ],
      // pr:'sam'
    }
  }
};
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
