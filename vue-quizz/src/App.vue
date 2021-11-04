<template>
<div>
  <ul id="questions">
  <li 
  v-for="question in questions" 
  :key="question.question"
  >
<Question question/>
  </li>
</ul>
  
</div>
</template>

<script>
import Question from './components/Question.vue'
export default {
  name: 'App',
  components: {
    Question
  },
  data() {

  return {
    questions: [
      {
        question:"who is batman",
        alternatives:["batman", "gemberss","horunge", "turk"],
        answear:"batman"
      },
      {
        question:"who is batman",
        alternatives:["batman", "gemberss","horunge", "turk"],
        answear:"batman"
      },
    ]
  }
  }
}
</script>

<style>
</style>