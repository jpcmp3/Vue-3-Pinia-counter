<template>
   <h1>Result</h1>
   <div class="heading">
      <h2>{{ displayText }}</h2>
      <hr>
    </div>
  
    <div class="input">
      <h3>Enter text here</h3>
      <input type="text" v-model="inputText"> <!-- Bind inputText to the input field -->
      <button @click="displayData">Send</button>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        displayText: '',
        inputText: ''
      };
    },
    methods: {
      displayData() {
        this.displayText = this.inputText; // Update displayText with inputText
      }
    }
  };
  </script>

<style>
.input {
    margin-top: 20px;
}
</style>