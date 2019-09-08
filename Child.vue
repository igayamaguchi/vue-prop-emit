<template>
  <button @click="countUp">
    +
  </button>
</template>

<script>
export default {
  name: "Child",
  props: { count: { type: Number, required: true } },
  methods: {
    countUp() {
      this.$emit('set-count', this.count + 1)
    }
  }
}
</script>

<style scoped>

</style>
