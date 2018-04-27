<template>
  <div class="input">
    <input type="text" v-model="txt" placeholder="edit me" />
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';

@Component
export default class InputText extends Vue {
  txt!: string;

  constructor () {
    super();
    this.txt = '';
  }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
input {
  margin: 40px 0 0;
  color: blue;
  text-align: center;
}
</style>
