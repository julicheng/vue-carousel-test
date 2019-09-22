<template>
  <div id="app">
    <Header v-bind:title="title" />
    <Carousel v-bind:productData="productData" />
    <!-- <div v-for="data in productData">{{data}}</div> -->
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Carousel from "./components/Carousel.vue";
import json from "./data.json";

export default {
  name: "app",
  components: {
    Header,
    Carousel
  },
  data() {
    return {
      productData: json.carouselData,
      title: "Related Items"
    };
  }
};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css?family=Roboto&display=swap");

* {
  font-family: Roboto;
  width: 900px;
  margin: 0 auto;
}
</style>
