<template>
  <nav>
  <Header/>
  </nav>
  <router-view/>
</template>
 <script>
 import Header from '../src/components/Header.vue'
 export default {
  components:{
    // eslint-disable-next-line vue/no-unused-components
    Header
  }
 }
 </script>
<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
body {
background:#ffffff;
font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
font-weight: 400;
line-height: 1.75;
display: flex;
justify-content: center;
flex-direction: column;
align-items: center;
 width: 100%;
}

.dark-mode {
  background-color: black;
  color: white;
}
nav {
     
     cursor: pointer;
     user-select: none;
     color: #636363;
     padding: 10px 0;
     border: 2px solid transparent;
     
     border-color: transparent transparent rgba(146, 146, 146, 0.1) transparent;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
