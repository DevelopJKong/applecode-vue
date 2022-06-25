<template>
  <div>
    <h4>XX 원룸</h4>
    <p>{{ price1 }} 만원</p>
  </div>

  <div>
    <h4>XX 원룸</h4>
    <p>{{ price2 }} 만원</p>
  </div>
  <div v-for="product in products" v-bind:key="product.id">
    {{ product }}
  </div>
</template>

<script>

export default {
  el:"#product",
  data() {
    return {
      price1: 60,
      price2: 70,
      products:['역삼동 원룸','천호동 원룸','마포구 원룸']
    }
  },

}
</script>

<style>

</style>
