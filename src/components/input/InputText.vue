<template>
  <div class="input">
    <input  v-model="txt" placeholder="edit me" />
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue,  Model } from 'vue-property-decorator';

@Component
export default class InputText extends Vue {
  @Model() private txt!: string;
  update () : void{
    console.info(this.txt);
  }


}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
input {
  margin: 40px 0 0;
  font: outline;
  color: blue;
  font-family: Arial, Helvetica, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
button {
  width: 10px;
}
</style>
