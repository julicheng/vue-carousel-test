<template>
  <header>
    <h1>{{title}}</h1>
  </header>
</template>

<script>
export default {
  name: "Header",
  props: {
    title: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
header {
  background: black;
  color: white;
  text-align: center;
  h1 {
    padding: 20px;
    font-size: 30px;
  }
}
</style>
