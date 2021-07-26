<template>
  <p>Result is {{ score }}ms</p>
  <div v-if="score < 250">
    <p>Your too fast</p>
  </div>
  <div v-else-if="score > 250 && score < 500">
    <p>Your Normal</p>
  </div>
  <div v-else>
    <p>Your are to slow.Try Again</p>
  </div>
</template>

<script>
export default {
  props: ["score"],
};
</script>

<style>
</style>