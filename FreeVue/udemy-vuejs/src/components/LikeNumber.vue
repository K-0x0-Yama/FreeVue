<template>
  <div>
    <p>ライクナンバーいいね({{ totalNumber }})</p>
    <button @click="increment">+1</button>
  </div>
</template>

<script>
export default {
  props: ["totalNumber"],
  methods: {
    increment: function () {
      this.number += 1;
    }
  }
};
</script>


<style scoped>
div {
  border: 1px solid blue;
}
</style>
