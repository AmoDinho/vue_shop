<template>
  <div id="app">
  <div class="unit" v-for="unit in manifest">
  <Child :item="unit.item" :url="unit.url"> </Child>
   </div>
  </div>
</template>

<script>
import Child from "./components/Child.vue";
export default {
  name: "App",
  components: {
    Child
  },
  data() {
    return {
      manifest: [
        {
          item: "Shoe",
          url: "https://cdn.thesolesupplier.co.uk/2017/11/Yeezy-Boost-350-V2-Semi-Frozen-Yellow-B37572.png"
        },
        {
          item: "T- shirt",
          url: "https://cdn1.uksoccershop.com/images/arsenal-2014-2015-puma-training-shirt-yellow.jpg"
        },
         {
          item: "Sweatshirt",
          url: "https://ae01.alicdn.com/kf/HTB1KJY0ePlxYKJjSZFuq6yYlVXaT/Arsenal-1886-Jackets-Men-Pullover-Hoodie-fashion-Sweatshirts-clothing-gunner-kings-of-north-london-is-red.jpg_640x640.jpg"
        },
      ]
    };
  }
  
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  display:flex;
  justify-content:center;
}
</style>
