<template>
  <div class="heading">
    <router-link :to="{ name: 'Home' }" class="title">
      <h1>Home</h1>
    </router-link>
  </div>
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
.heading{
  background: rgb(250, 198, 198);
  padding: 20px 0;
}
</style>
