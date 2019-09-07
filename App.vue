<template>
  <Child :count="count" @set-count="handleSetCount" />
</template>

<script>
import Child from "./Child";
export default {
  components: { Child },
  data() {
    return { count: 0 }
  },
  methods: {
    handleSetCount(newCount) {
      this.count = newCount;
    }
  }
};
</script>
