<template>
  <div class="about">
    <button 
    @click="storeCounter.increaseCount"
    class="counter-button">
      {{ storeCounter.count }}
    </button>
  </div>
</template>

<script setup>
  import { useCounterStore } from '@/stores/counter'

  const storeCounter = useCounterStore()
</script>

<style>
.counter-button {
  font-size: 50px;
  margin: 20px;
}
</style>