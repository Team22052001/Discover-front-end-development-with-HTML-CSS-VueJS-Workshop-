<template>
  <div id="app">
    <HearderBar></HearderBar>
    <router-view/>
  </div>
</template>

<script>
    import HearderBar from './components/HearderBar.vue'
    export default {
        components: { HearderBar },
        HearderBar
    }
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #50482c;

    &.router-link-exact-active {
      color: #b11111;
    }
  }
}
</style>
