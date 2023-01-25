<template>
  <div>
    <h1>Hello {{ userName }}</h1>
    <p>{{ message }}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      userName: 'wkd',
      message: 'Welcome Vue 3.0',
      arr: [],
      obj: {}
    }
  }
}
</script>

<style scoped>
.text-red {
  color: red;
}
</style>
