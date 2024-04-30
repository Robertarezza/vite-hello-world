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
     <div>
      <img :src="getImagePath(image)" alt="" />
     </div>
  </template>
  
  <style>
 div {
    text-align: center;
 }
  
   img {
    width: 60%;
  }
  
  
  </style>