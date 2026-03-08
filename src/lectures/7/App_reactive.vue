<template>
  <div>
    <p>{{ message }}</p>
    <button v-on:click="addMessage">add click</button>
  </div>
</template>
<script>
  import {reactive} from 'vue';

  export default{
    setup() {
      let message = reactive('Hello Vue');
      const addMessage = () => {
        message = message + '!';
      }
      return {
        message,
        addMessage
      }
    }
  }
</script>