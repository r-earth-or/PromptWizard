<template>
  <div id="app">
    <Header />
    <PromptInput />
    <PromptOutput />
    <Footer />
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Footer from './components/Footer.vue';
import PromptInput from './components/PromptInput.vue';
import PromptOutput from './components/PromptOutput.vue';

export default {
  name: 'App',
  components: {
    Header,
    Footer,
    PromptInput,
    PromptOutput
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
