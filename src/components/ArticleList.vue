<template>
    <div>
      <SingleArticle
      v-for="(article, index) in articles"
      :key="index"
      :article="article"
      />
    </div>
</template>

<script>
import SingleArticle from "@/components/SingleArticle.vue";

export default {
  name: 'ArticleList',
  props: ['articles'],
  components: {
    SingleArticle
  },
  data() {
    return {
     
    }
  },

  methods: {
    
  },
};
</script>

<style lang="scss" scoped>

</style>