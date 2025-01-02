<template>
  <div>
    <h2>Optimized Prompt</h2>
    <p>{{ optimizedPrompt }}</p>
    <h2>Expert Profile</h2>
    <p>{{ expertProfile }}</p>
  </div>
</template>

<script>
export default {
  name: 'PromptOutput',
  props: {
    optimizedPrompt: {
      type: String,
      required: true
    },
    expertProfile: {
      type: String,
      required: true
    }
  }
}
</script>

<style scoped>
div {
  margin: 20px;
}

h2 {
  color: #42b983;
}

p {
  font-size: 16px;
  color: #2c3e50;
}
</style>
