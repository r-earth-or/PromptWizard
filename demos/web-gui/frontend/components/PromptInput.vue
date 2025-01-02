<template>
  <div>
    <label for="prompt">Enter your prompt:</label>
    <input type="text" id="prompt" v-model="prompt" @keyup.enter="submitPrompt" />
    <button @click="submitPrompt">Submit</button>
  </div>
</template>

<script>
export default {
  name: 'PromptInput',
  data() {
    return {
      prompt: ''
    }
  },
  methods: {
    submitPrompt() {
      // Placeholder for the actual submit logic
      console.log('Prompt submitted:', this.prompt);
    }
  }
}
</script>

<style scoped>
div {
  margin: 20px;
}

label {
  margin-right: 10px;
}

input {
  padding: 5px;
  font-size: 16px;
}

button {
  padding: 5px 10px;
  font-size: 16px;
  background-color: #42b983;
  color: white;
  border: none;
  cursor: pointer;
}

button:hover {
  background-color: #369b73;
}
</style>
