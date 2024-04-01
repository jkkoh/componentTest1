<script setup>
import { ref } from 'vue'

const count = ref(0)

</script>
<template>
    <button @click="count++">you clicked me {{ count }} times</button>
    <button @click="count = 0"> reset </button>
</template>