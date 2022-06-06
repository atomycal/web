<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://vuejs.org/api/sfc-script-setup.html#script-setup
import HelloWorld from './components/HelloWorld.vue'
import SiteMenu from './components/SiteMenu.vue'
</script>

<template>
  <site-menu></site-menu>
  <h1>Something explosive is coming</h1>
</template>

<style lang="scss">
body, html {
  margin: 0;
  font-size: 16px;
}

#app {
  font-family: Mulish, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.button {
  font-family: Montserrat, Helvetica, sans-serif;
  font-weight: bold;
}
</style>
