<template>
  <div class="container">
   <div class="home">
     <Navbar/>
     <div class="header">
       <div class="left">
         <Hero></Hero>
       </div>
       <div class="right">
         <Cards/>
       </div>
     </div>
   </div>
  </div>
</template>

<script>
// @ is an alias to /src
import Navbar from "./../components/Navbar.vue";
import Hero from "./../components/Hero.vue";
import Cards from "./../components/Cards.vue";

export default {
  name: 'Home',
  components: {
    Navbar,
    Hero,
    Cards,
  },
  
}
</script>
<style scoped>
.container{
  height: 100vh;
  width: 100vw;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%,-50%);
  background-image: linear-gradient(rgba(44, 52, 83, 0.7) , rgba(22, 66, 59, 0.7)),
  url("./../assets/img3.jpeg");
}
.home{
  height: 90%;
  width: 90%;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%,-50%);
  background-image: linear-gradient(rgba(20, 33, 83, 0.7) , rgba(4, 8, 22, 0.7)),
  url("./../assets/img2.jpeg");
  background-position: top;
  background-size: cover;
}

.header{
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 90%;
  /* width: 90%; */
}
.left , .right{
  position: relative;
  width: 50%;
  height: 100%;
  
}

</style>
