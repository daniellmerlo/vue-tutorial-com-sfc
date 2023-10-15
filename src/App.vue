<script setup>
import {ref, reactive} from 'vue'

const message = ref('Hello World!')
const counter = reactive({
  count:0
})

console.log(message.value)
message.value = 'Changed'

console.log(counter.count)
counter.count++

</script>
<template>
  <h1>{{ message }}</h1>
  <p>count is: {{ counter.count }}</p>
  <h1>{{ message.split('').reverse().join() }}</h1>
</template>