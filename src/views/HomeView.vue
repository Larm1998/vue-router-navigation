<script>
export default {
  data() {
    return {
      username: '',
    }
  },
  methods: {
    begin() {
      this.$router.push('/chats')
    }
  }
}
</script>

<template>
  <main>
    <h3>Enter your username {{ username }}</h3>
    <input placeholder="username" v-model="username"/>
    <button @click="begin">Login</button>
  </main>
</template>
