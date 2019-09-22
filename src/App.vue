<template>
  <div id="app">
    <Header v-bind:title="title" />
    <carousel>
      <slide>Slide 1 Content</slide>
      <slide>Slide 2 Content</slide>
    </carousel>
    <!-- <div v-for="data in productData">{{data}}</div> -->
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import { Carousel, Slide } from "vue-carousel";
import json from "./data.json";

export default {
  name: "app",
  components: {
    Header,
    Carousel,
    Slide
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
