<script setup>
import { ref } from 'vue'
const msg = ref('')
</script>

<template>
    <p>current component : B </p>
    <span>Message is : {{ msg }}</span>
    <input v-model="msg">
</template>
