<template @click="$emit('customevent', {})">
  <div>
    <h3>{{title.split('')}}</h3>
    <p>{{text}}</p>
  </div>
</template>

<script>
export default {
  name: "NewsItem",
  props: {
    title: {
      type: String,
      default: "...",
      required: true,
    },
  },
  data() {
    return {
      text: "",
    };
  },
};
</script>

<style lang="scss" scoped>
</style>