<template>
  <button type="button" @click="response">Click Me!</button>
</template>

<script>
import Axios from "axios";
export default {
  name: "login",
  methods:{
    response(){
      // alter(123);
      Axios.get('http://localhost:3000/users').then(function(response){
        console.log("你已连接！");
      })
    }
  }

}
</script>

<style>

</style>
