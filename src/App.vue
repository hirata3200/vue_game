// app.vue
<template>
<div class="contianer mx-auto mt-4" style="width:300px">
<Quiz v-bind:quiz="mondai" />
<Answer v-bind:answer="kotae.a" />
<Answer v-bind:answer="kotae.b" />
<Answer v-bind:answer="kotae.c" />
<Answer v-bind:answer="kotae.d" />
</div>
</template>

<script>
import Quiz from './components/Quiz.vue';
import Answer from './components/Answer.vue';

export default {
  name: 'App',
  components: {
    Quiz,
    Answer
  },
  data() {
    return {
      mondai:"世界で一番高い山は？",
      kotae:{
      a:"東京タワー",
      b:"ヒマダナ山脈",
      c:"エベレスト",
      d:"琵琶湖"
      }
    }
  }
}
</script>