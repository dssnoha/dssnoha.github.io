<script setup lang="ts">
import { ref } from 'vue'

const projects = ref([])

const skills = ref([
  'Software Development (Vue.js, c#, TypeScript)',
  'Business Management & E-commerce (Shopify)',
  'Marketing & Online Advertising',
])
function gottopage() {
  window.location.href = 'https://github.com/dssnoha'
}
function emailme() {
  window.location.href = 'mailto:dssnoha@gmail.com'
}
</script>
<template>
  <div>
    <h1>my Hobbies</h1>
  </div>
</template>
