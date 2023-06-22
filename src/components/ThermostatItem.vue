<template>
  <div>
    <h1 v-html="data.name" />
    <div v-html="data.currentTemp" />
    <div v-html="data.destTemp" />
    <meter :value="data.currentTemp" min="40" max="100" />

  </div>
</template>

<script setup>
defineProps({
  data: {
    type: Object,
    required: true
  }
});
</script>

<style lang="scss" scoped>

</style>