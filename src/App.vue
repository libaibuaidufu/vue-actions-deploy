<template>
  <div  class="markdown-body">
     <VueMarkdown :source="mdData" v-highlight></VueMarkdown>
  </div>
</template>

<script>
import "highlight.js/styles/github.css";
import "github-markdown-css";
import VueMarkdown from 'vue-markdown';
import Good from "./docs/xx.md";
export default {
  components: {
    VueMarkdown
  },
  data() {
    return {
      mdData: Good
    }
  },
}

</script>

<style>

</style>
