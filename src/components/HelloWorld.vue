<template>
  <div class="hello">
    <h1>{{ title }}</h1>
    <h2>{{ text }}</h2>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  data() {
    return {
      title: "Vue.js",
      text: "文法テスト編"
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1,
h2 {
  font-weight: normal;
}
</style>
