<template>
  <div class="board">
    <Marubatu v-for="n of 9" v-bind:key="n" />
  </div>
</template>

<script>
import Marubatu from "./components/Marubatu.vue";
export default {
  name: "App",
  data() {
    return {
      count: 0,
    }
  },
  components: {
    Marubatu,
  },
};
</script>

<style>
.board {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  width: 450px;
}
</style>