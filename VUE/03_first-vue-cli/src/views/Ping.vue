<template>
  <div>
    <h1>Ping</h1>
    <input @keyup.enter="sendToPong" v-model="inputText" type="text">

  </div>
</template>

<script>
export default {
  name: 'Ping',
  data: function () {
    return { 
      inputText: '',
    }
  },
  methods: {
    sendToPong: function () {
      this.$router.push({name:'Pong', query: {message: this.inputText}})
      // this.$router.push(`pong?message=${this.inputText}`)
    }
  }
}
</script>

<style>

</style>
