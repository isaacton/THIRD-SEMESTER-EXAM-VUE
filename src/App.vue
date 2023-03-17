<template>
  <nav>
    <router-link to="/">Home</router-link> |
    <router-link to="/about">Single Repository</router-link>
  </nav>
  <router-view/>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 60px;
  
}

nav a {
  border-radius: 5px;
  padding: 20px;
  margin: 30px;
  font-weight: bold;
  color: #fff;
  background-color: green;
}

nav a.router-link-exact-active {
 
  background-color: red;
}
</style>
