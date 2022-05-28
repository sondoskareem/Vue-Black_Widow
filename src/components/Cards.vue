<template>
    <div class="cards">x
        <Card v-for="(movie,index) in movies.slice(0, 2)" :key="index" :movie="movie"></Card>

    </div>
</template>

<script>
import Card from "./Card.vue";

export default {
  name: "cards",
   data () {
    return {
      movies: []
    }
  },
  components:{
    Card
  },
  mounted () {
    this.axios.get('https://api.themoviedb.org/3/movie/157336/recommendations?api_key=c4249db136e1d20de39d702aa5db9c12&limit=2').then((response) => {
      this.movies = response.data.results
      console.log(this.movies)

    })
    
  }
};
</script>
<style scoped>
.cards{
  position: absolute;
  top: 10%;
  right: 0;
  /* transform: translate(-50% , -50%); */
}
</style>