<template>
  <div class="hello">
    <h1>{{ title }}</h1>
    <h2>{{ text }}</h2>
    <h3>{{ ToDoList }}</h3>
    <h3>{{ DoneList }}</h3>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  data() {
    return {
      title: "Vue.js",
      text: "文法テスト編",
      ToDoList: "v-if, v-for, v-bind, v-on, v-model, methods, computed, watch",
      DoneList: "マスタッシュ記法, data"
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
