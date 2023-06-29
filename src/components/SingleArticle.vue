<template>
  <div class="product-box">
    <h2>{{ article.name }}</h2>
    <img 
    :src="article.imageUrl"
    width="400px"
    >
    <div class="content">
      {{ article.text }}
    </div>
  </div>
</template>

<script>
export default {
  name: 'SingleArticle',
  props: ['article'],
  data() {
    return {
      
    };
  },
  methods: {
    
  },
};
</script>

<style lang="scss" scoped>

</style>