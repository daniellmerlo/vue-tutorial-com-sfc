<script setup>
import { ref } from 'vue'
import ChildComp from './ChildComp.vue'

const childMsg = ref('No child message yet')
</script>
<template>
  <ChildComp @response="(msg) => childMsg = msg" />
  {{ childMsg }}
</template>
