<script setup>
import { ref } from 'vue'
const abc = ref(0)
</script>
<template>
    <p>current component: C </p>
    <span>abc: {{ abc }}</span>
    <button @click="abc++">+</button>
</template>