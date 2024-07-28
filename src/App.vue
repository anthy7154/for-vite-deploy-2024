<script setup>
  import { ref } from 'vue';

  const num = ref(2); // 先定義值，再決定如何操作；關注點分離的做法
  // console.log(num.value);

  // setInterval(() => {
  // 	num.value++
  // }, 500);

  function clickMe() {
    num.value++
  }
</script>

<template>
  <div>

    {{ num }}

    <!-- v-on 是一個監聽器 -->
    <button type="button" v-on:click="clickMe">點我</button>
  </div>
</template>


