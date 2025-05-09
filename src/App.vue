<template>
  <div>
    <input type="text" v-model='test' placeholder=".shop주소 도메인명을 쓰시오">
    <button v-on:click="move">뭅뭅</button>
  </div>
</template>

<script setup>
  import { ref } from 'vue';

  const test = ref('');

  function move() {
    location.href='https://' + test.value + '.shop/health';
  }
</script>

<style scoped>

</style>