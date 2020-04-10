<template>
  <div class="hello">
    <h1>{{ title }}</h1>
    <h2>{{ text }}</h2>
    <h3>{{ todoList }}</h3>
    <h3>{{ doneList }}</h3>
    <h4 v-show="showText">{{ showSampleText }}</h4>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  data() {
    return {
      title: "Vue.js",
      text: "文法テスト編",
      todoList: "v-if, v-for, v-bind, v-on, v-model, methods, computed, watch",
      doneList: "マスタッシュ記法, data",
      showText: false,
      showSampleText: "見えていますか？"
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
