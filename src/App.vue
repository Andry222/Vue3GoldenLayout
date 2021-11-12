<template id="app">
  <div id="nav">
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link> |
    <router-link to="/dashboard">Dashboard</router-link>
  </div>
  <router-view/>
</template>


<style>
html {
    height: 100%;
}
body {
    height: 100%;
    margin: 0;
    overflow: hidden;
}
.full-height, #app {
    height: 100%;
}
#app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
}
#nav {
    text-align: center;
}

button{

}
</style>