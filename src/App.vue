<template>
  <NAVIGATION></NAVIGATION>
  <nav>
    <router-link to="/">网络测速</router-link> |
    <router-link to="/about">其他</router-link>
  </nav>
  <router-view />
</template>
<script>
import NAVIGATION from './views/navigation/navigation.vue'
export default {
  name: 'APP',
  components: {
    NAVIGATION
  }
}
</script>
<style lang="less">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: right;
  color: #2c3e50;
}

nav {
  padding: 5px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #259ce6;
    }
  }
}
</style>
