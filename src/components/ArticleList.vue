<template>
  <div class="articles" width="500px">
    <h1>Сортировка статей по тэгам</h1>
    <input type="checkbox" id="check1" value="1" v-model="categories">
        <label for="check1">Kitchen</label>
        <input type="checkbox" id="check2" value="2" v-model="categories">
        <label for="check2">Bedroom</label>
        <input type="checkbox" id="check3" value="3" v-model="categories">
        <label for="check3">Building</label>
        <input type="checkbox" id="check4" value="4" v-model="categories">
        <label for="check4">Architecture</label>
        <input type="checkbox" id="check5" value="5" v-model="categories">
        <label for="check5">Kitchen planning</label>
        <hr>
        <div v-for="(product, index) in products"
        :key="index">
          <MyComp 
            :name="product.name"
            :imageUrl="product.imageUrl"
            :text="product.text"
          />
        </div>
        
  </div>
</template>

<script>
import MyComp from './MyComp.vue'

export default {
  name: 'ArticleList',
  components: {
    MyComp 
  },
  data() {
    return {
      products: [{
                    id: 1,
                    name: 'Kitchen design',
                    imageUrl: require("@/assets/product.jpg"),
                    text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Reiciendis harum odit mollitia facere porro adipisci eos! Quae natus perferendis doloremque.',
                    category: '1'
                }, {
                    id: 2,
                    name: 'Bedroom design better',
                    imageUrl: require("@/assets/product.jpg"),
                    text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Reiciendis harum odit mollitia facere porro adipisci eos! Quae natus perferendis doloremque.',
                    category: '2'
                }, {
                    id: 3,
                    name: 'Kitchen design',
                    imageUrl: require("@/assets/product.jpg"),
                    text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Reiciendis harum odit mollitia facere porro adipisci eos! Quae natus perferendis doloremque.',
                    category: '1'
                }, {
                    id: 4,
                    name: 'Buildings design the best',
                    imageUrl: require("@/assets/product.jpg"),
                    text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Reiciendis harum odit mollitia facere porro adipisci eos! Quae natus perferendis doloremque.',
                    category: '3'
                }, {
                    id: 5,
                    name: 'Bedroom design better',
                    imageUrl: require("@/assets/product.jpg"),
                    text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Reiciendis harum odit mollitia facere porro adipisci eos! Quae natus perferendis doloremque.',
                    category: '2'
                }, {
                    id: 6,
                    name: 'Buildings design the best',
                    imageUrl: require("@/assets/product.jpg"),
                    text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Reiciendis harum odit mollitia facere porro adipisci eos! Quae natus perferendis doloremque.',
                    category: '3'
                }, {
                    id: 7,
                    name: 'New Architecture',
                    imageUrl: require("@/assets/product.jpg"),
                    text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Reiciendis harum odit mollitia facere porro adipisci eos! Quae natus perferendis doloremque.',
                    category: '4'
                }, {
                    id: 8,
                    name: 'Kitchen planning design',
                    imageUrl: require("@/assets/product.jpg"),
                    text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Reiciendis harum odit mollitia facere porro adipisci eos! Quae natus perferendis doloremque.',
                    category: '5'
                }, {
                    id: 9,
                    name: 'New Architecture',
                    imageUrl: require("@/assets/product.jpg"),
                    text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Reiciendis harum odit mollitia facere porro adipisci eos! Quae natus perferendis doloremque.',
                    category: '4'
                }, {
                    id: 10,
                    name: 'Bedroom design better',
                    imageUrl: require("@/assets/product.jpg"),
                    text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Reiciendis harum odit mollitia facere porro adipisci eos! Quae natus perferendis doloremque.',
                    category: '2'
                }, {
                    id: 11,
                    name: 'Kitchen planning design',
                    imageUrl: require("@/assets/product.jpg"),
                    text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Reiciendis harum odit mollitia facere porro adipisci eos! Quae natus perferendis doloremque.',
                    category: '5'
                }]
    };
  },

  methods: {
    chooseCategory() {
      
    }
  },
};
</script>

<style lang="scss" scoped>

</style>