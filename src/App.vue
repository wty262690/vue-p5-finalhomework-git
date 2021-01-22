<template>
    <router-view/>

</template>

<script>
export default {
  data() {
          return {
          }
  },
  
}

</script>

<style>
@import './font.css';
@import './menu.css';

body{
  margin:0;
  background-color:black;
}
#app {
  margin:0;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: white;
  position:absolute;
}


#nav a {
  font-weight: bold;
  color: white;
}

#nav a.router-link-exact-active {
  color: #42b983;
}



</style>
