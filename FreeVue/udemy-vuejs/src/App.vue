<template>
  <div>
    <LikeHeader></LikeHeader>
    <h2>{{number}}</h2>
    <LikeNumber :totalNumber="number"></LikeNumber>
    <LikeNumber :total-number="number"></LikeNumber>
  </div>
</template>

<script>
import LikeHeader from "./components/LikeHeader"

export default {
  data: function(){
    return {
      number: 20
    };
  },
  components: {
    LikeHeader: LikeHeader
  }
}
</script>


<style>
div {
  border: 1px solid red;
}
</style>