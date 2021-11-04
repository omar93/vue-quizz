<template>
    <div id="question-container">
        <span id="question-title">Who is batman</span>
        <ul id="answear-list">
            <li> <button @click="handleClick">batman</button> </li>
            <li> <button @click="handleClick">iron man</button> </li>
            <li> <button @click="handleClick">the flash</button> </li>
            <li> <button @click="handleClick">superman</button> </li>
        </ul>
    </div>
</template>

<script>
export default {
  props: {
    data: Array
  },
  methods: {
      handleClick() {
          alert('kebab')
      }
  }
}
</script>

<style scoped>

div {
    display: flex;
    flex-direction: column;
}


ul {
    list-style: none;
    padding: 0;
    margin: 0;
    margin-top: 20px;
}
</style>
