<template>
  <div id="app">
    <keep-alive>
      <component :is="component"></component>
    </keep-alive>
  </div>
</template>
<script>
import Question from './components/Question.vue';

export default {
  name: 'app',
  components: {
    Question
  },
  data() {
    return {
      component: 'question'
    }
  },
  computed: {
    getQuests() {
      return getQuests();
    }
  }
}

function getQuests() {
  return [{
      type: 'radio',
      title: 'Какой тег задает ссылку?',
      answers: [
        'a',
        'div',
        'span',
        'img'
      ]
    },
    {
      type: 'checkbox',
      title: 'Какие из этих тегов строчные?',
      answers: [
        'a',
        'div',
        'span',
        'img'
      ]
    }
  ];
}
</script>
<style>
body {
  color: #000;
}
</style>