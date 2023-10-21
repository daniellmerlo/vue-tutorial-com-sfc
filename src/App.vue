<script setup>
import { ref } from 'vue'
import ChildComp from './ChildComp.vue'

const greetings = ref('Hello from parent')
</script>
<template>
  <ChildComp :msg="greetings" />
</template>
