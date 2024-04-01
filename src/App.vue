<script setup>
import { shallowRef } from 'vue'
import CompA from './components/CompA.vue'
import CompB from './components/CompB.vue'
import CompC from './components/CompC.vue'

const current = shallowRef(CompA)

</script>

<template>

<div class="demo">
  <label><input type="radio" v-model="current" :value="CompA"></label>
  <label><input type="radio" v-model="current" :value="CompB"></label>
  <label><input type="radio" v-model="current" :value="CompC"></label>
  <keep-alive>
    <component :is="current"></component>
  </keep-alive>
</div>

</template>

<style>

</style>
