<template>
  <div>
    <p>increment:ライクナンバー({{ totalNumber / 2 }})</p>
    <p>half:ライクナンバー({{ halfNumber / 2 }})</p>
    <button @click="increment">+1</button>
  </div>
</template>

<script>
export default {
  props: {
    totalNumber: {
      type: Number,
      required: true
    }
  },
  computed: {
    halfNumber: function () {
      return this.totalNumber / 2;
    }
  },
  methods: {
    increment() {
      this.totalNumber += 1;
    }
  }
};
</script>


<style scoped>
div {
  border: 1px solid blue;
}
</style>
