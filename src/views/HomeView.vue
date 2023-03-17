<template>
  <div class="home">
    <h3> Page to show git Repositories</h3>
    <p>{{data}}</P>
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'
export default {
  data(){
    return {
      data: "",
    };
  },
  mounted(){
    fetch("https://api.github.com/users/{{isaacton}}/repos",{
      headers:{
        accept: "application/json",
      },
    })
    .then((res) => res.json())
    .then((data) => (this.data = data))
  }
  }
</script>


<style>
h3{
  
  color: #fff;
}
*{
  background-color: blue;
}
</style>