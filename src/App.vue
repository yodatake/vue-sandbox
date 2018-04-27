<template>
  <div id="app">
    <img src="./assets/logo.png">
    <global-header />
    <router-view propsMessage="vue-router"></router-view>
    <global-footer />
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import GlobalFooter from "./components/globals/GlobalFooter.vue";
import GlobalHeader from "./components/globals/GlobalHeader.vue";

@Component({
  components: {
    GlobalHeader,
    GlobalFooter
  }
})
export default class App extends Vue {}
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
