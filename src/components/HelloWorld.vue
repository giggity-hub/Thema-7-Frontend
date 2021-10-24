<script setup>
import { ref } from 'vue'
import Form from './Form.vue';

defineProps({
  msg: String
})

const count = ref(0)
</script>

<template>
  <!-- <h1>{{ msg }}</h1> -->

  <div class="bg-orange">
    <Form/>
  </div>

  <!-- reddit -->
  <!-- twitter -->
  <!-- discord -->
  <!-- email -->


</template>

<style scoped>

</style>
