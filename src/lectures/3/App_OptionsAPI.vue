<template>
  <div>
    <button v-on:click="increment">Counter: {{ counter }}</button>
  </div>
</template>

<script>
  import {ref} from 'vue';

  
  export default {
    data() {
      return {
        counter: 0,
      }
    },
    methods: {
      increment() {
        this.counter++;
      }
    },
    mounted() {
      console.log('컴포너트가 마운트 됨')
    }
  }
</script>
