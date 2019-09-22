<template>
  <Product />
</template>

<script>
import Product from "./Product";
export default {
  name: "Carousel",
  components: { Product },
  props: {
    productData: []
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
</style>
