<template>
  <div class="test">
    <h1>{{ title }}</h1>
    <h2>{{ text }}</h2>
    <h3>{{ todoList }}</h3>
    <h3>{{ doneList }}</h3>
    <h4 v-show="showText">{{ showSampleText }}</h4>
    <button v-on:click="toggle">隠しボタン *絶対に押さないでね！*</button>

    <h1>あなたの会員ランク</h1>
    <p v-if="isMember && isPremier">「 あなたはプレミアム会員です 」</p>
    <p v-else-if="isMember && !isPremier">「 あなたは一般会員です 」</p>
    <p v-else-if="!isMember && !isPremier">「 あなたは会員ではありません 」</p>
    <p v-else>不正なユーザーです</p>
  </div>
</template>

<script>
export default {
  name: "test",
  data() {
    return {
      title: "Vue.js",
      text: "文法テスト編",
      todoList: "v-for, v-bind, v-model, computed, watch",
      doneList: "マスタッシュ記法, data, v-on, methods, v-if, ",
      showText: false,
      showSampleText: "いやん///",
      isMember: true,
      isPremier: true
    };
  },
  methods: {
    toggle: function() {
      this.showText = !this.showText;
    }
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
