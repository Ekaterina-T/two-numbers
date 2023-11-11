<script setup lang="ts">
import { ref } from 'vue';

const leftNumber = ref(0)
const rightNUmber = ref(0)
</script>

<template>
  <section class="input-area">
    <label class="input-area__input">
      <span>Enter left number</span>
      <input type="number" id="number1" v-model.number="leftNumber"/>
    </label>

      <label class="input-area__input">
        <span>Enter right number</span>
        <input type="number" id="number2" v-model.number="rightNUmber"/>
    </label>
  </section>
</template>

<style scoped>
.input-area {
  display: flex;
  flex-direction: column;
  row-gap: 20px;
}

.input-area__input {
  display: flex;
  column-gap: 25px;
}
</style>
