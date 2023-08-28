<script setup>
  import { ref } from 'vue';

  let count = ref(0)


  let AddCount = ()=>{
    count.value = count.value + 1
  }

  let SubCount = ()=>{
    count.value = count.value - 1
  }
</script>


<template>
  <main>
    <div class='counter'>
      <div class="cont">
        <h4 >Le Compteur est a ....</h4>
      <h1>{{count}}</h1>
      <button @click="SubCount()">-</button>
      <button @click="AddCount()">+</button>
      </div>
    </div>
  </main>
</template>