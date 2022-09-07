<script setup>
import { ref } from 'vue'
import { useRouter } from 'vue-router'
const username = ref()

const router = useRouter()

function initialize() {
  router.push({ name: 'about' })
}
</script>

<template>
  <main>
    <h3>Enter your username {{ username }}</h3>
    <input placeholder="username" v-model="username"/>
    <button @click="begin">Login</button>
  </main>
</template>
