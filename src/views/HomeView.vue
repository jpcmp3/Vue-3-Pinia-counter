<template>
  <div class="home">
    <Counter/>
    <div class="buttons">
      <button @click="storeCounter.decreaseCount">-</button>
      <button @click="storeCounter.increaseCount">+</button>
    </div>

    <div>
      This counter is: {{ storeCounter.oddOrEven }}
    </div>
<hr>
<div>
  <h1>Edit counter: </h1>
  <input 
  v-model="storeCounter.count"
  type="number">

</div>
  </div>
</template>

<script setup>
import Counter from '@/components/Counter.vue'
import { useCounterStore } from '@/stores/counter'

  const storeCounter = useCounterStore()
</script>

<style>
.count {
  font-size: 60px;
  margin: 20px;
  }
  .buttons {
  background-color: rgb(164, 171, 67); 
  padding: 10px;
}
.buttons button {
  font-size: 40px;
  margin: 10px;
}
</style>