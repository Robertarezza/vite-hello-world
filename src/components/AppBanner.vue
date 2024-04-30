<script>
export default {
    data() {
      return {
        image: "hero.png",
      };
    },
    methods: {
      getImagePath(imageName) {
        return new URL(`../assets/${imageName}`, import.meta.url).href;
      },
    },
  };
  </script>
  
  <template>
     
      <img :src="getImagePath(image)" alt="" />

  </template>
  
  <style>
 
  
   img {
    width: 100%;
  }
  
  
  </style>