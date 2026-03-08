<template>
  <div>
    <button v-on:click="increment">Counter: {{ counter }}</button>
  </div>
</template>

<script>
  import {onMounted, ref} from 'vue';

  export default {
    setup() {
      const counter = ref(0);
      const increment = () => counter.value++;

      return {
        counter,
        increment,
      }
    }, 
    mounted() {
      console.log('컴포너트가 마운트 됨')
    }
  }
</script>