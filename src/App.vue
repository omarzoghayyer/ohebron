<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div>
    <router-view/>
  </div>
</template>

<style>
*{
  padding: 10;
  margin: 0;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;

}

#nav {
  background-color: rgb(247, 248, 242);
  position: relative;
  color: #6dfdb5;
  font-size: 29px;
font-family:Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
}

#nav a {
  font-weight: 400;
  color: #0c0c0c;
}

#nav a.router-link-exact-active {

  text-decoration: none;
}
</style>
