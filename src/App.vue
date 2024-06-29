<script setup>
import { ref } from "vue";
  
  const count = ref(0)
  const handleCounter = ()=>{
    count.value++
    console.log(count.value)
  }
</script>

<template>
    <div class='main'>
      <h2>{{count}}</h2>
      <div class="btn-box">
        <button class="button button-yellow" @click="count=0" >بازنشانی</button>
        <button class="button button-light" @click="handleCounter" >شمارنده</button>
      </div>
    </div>
</template>
