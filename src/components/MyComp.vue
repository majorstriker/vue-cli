<template>
  <div class="product-card">
    <h2>{{ name }}</h2>
    <img 
    :src="imageUrl"
    width="300px"
    >
    <div class="content">
      {{ text }}
    </div>
  </div>
</template>

<script>
export default {
  name: 'MyComp',
  props: ['id', 'name', 'imageUrl', 'text', 'category'],
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