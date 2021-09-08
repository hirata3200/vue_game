<template>
<div class="alert alert-primary">
  <div v-on:click="doAction"><p ref="msg">{{answer}}</p></div>
  </div>
</template>

<script>
export default {
  name: "Answer",
  props: {
    answer: String
  },
  methods: {
      doAction(){
        if(this.answer === "エベレスト"){
          this.$refs.msg.innerHTML="正解"
        }else{
          this.$refs.msg.innerHTML="不正解"
        }
      }
  },
};
</script>