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
@import url('https://fonts.googleapis.com/css2?family=Lobster&display=swap');
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  background-color: rgb(0, 0, 0);
  position: fixed;
  top: 0;
  width: 100%;
}

li {
  float: left;
}

li a {
  display: block;
  color: rgb(255, 255, 255);
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

li a:hover:not(.active) {
  background-color: #111;
}

.active {
  background-color: #0011ff;
}
</style>
