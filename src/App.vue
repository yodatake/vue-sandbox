<template>
  <div id="app">
    <img src="./assets/logo.png">
    <hello-world msg="Welcome to Your Vue.js + TypeScript App"/>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import HelloWorld from "./components/HelloWorld.vue";
import InputText from "./components/nest/InputText.vue";
import ListTable from "./components/nest/ListTable.vue";

@Component({
  components: {
    HelloWorld,
    InputText,
    ListTable
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
