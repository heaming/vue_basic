<template>
  <header>
    <h1>{{ props }}</h1>
    <button v-on:click="sendEvent">send</button>
  </header>
  <nav>

  </nav>
</template>

<script>
export default {
  name: "AppHeader",
  props: ['props'],
  methods: {
    sendEvent: function() {
      this.$emit('renew');
    }
  }
}
</script>

<style scoped>

</style>