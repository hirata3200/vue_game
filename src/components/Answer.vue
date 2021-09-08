<template>
  <div v-on:click="doAction">{{answer}}</div>
</template>

<script>
export default {
  name: "Answer",
  props: {
    answer: String
  },
  methods: {
      doAction(){
        // console.log("正解")
        // console.log(this.answer)
        if(this.answer === "エベレスト"){
          console.log("正解")
        }else{
          console.log("不正解")
        }
      }
  },
};
</script>