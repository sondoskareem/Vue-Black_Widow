<template>
    <div class="card">
        <div class="film-container">
         <img :src="'https://image.tmdb.org/t/p/original/'+movie.poster_path" width="150" height="200" alt="">
         <div class="img-details"  :style="{ 'background-image': 'linear-gradient(rgba(58, 66, 102, 0.7) , rgba(40, 88, 78, 0.7)),url(' + 'https://image.tmdb.org/t/p/original/'+movie.poster_path + ')' }">
           <h5>{{movie.title}}</h5>
           <p>{{movie.overview.substring(0, 100)}} ...</p>
           <div class="film-btn-group">
              <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-caret-right-fill" viewBox="0 0 16 16">
                <path d="m12.14 8.753-5.482 4.796c-.646.566-1.658.106-1.658-.753V3.204a1 1 0 0 1 1.659-.753l5.48 4.796a1 1 0 0 1 0 1.506z"/>
              </svg>
              <span>Watch Trailer</span>
           
              <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-plus" viewBox="0 0 16 16">
                <path d="M8 4a.5.5 0 0 1 .5.5v3h3a.5.5 0 0 1 0 1h-3v3a.5.5 0 0 1-1 0v-3h-3a.5.5 0 0 1 0-1h3v-3A.5.5 0 0 1 8 4z"/>
              </svg>
              <span>Add list</span>
              
           </div>
         </div>
        </div>
    </div>
</template>

<script>
export default {
  name: "Card",
  props: ['movie'],
};
</script>
<style scoped>
.card{
  /* position: absolute;
  top: 50%;
  right: 0;
  transform: translate(-50% , -50%); */
  margin-bottom: 2rem;
}
.film-container{
  display: flex;
  align-items: end;
}
.film-container>img{
border-radius: 10px;
}
.img-details{
  height: 6rem;
  width: 12rem;
  padding: .7rem;
  background-position: center;
  background-size: 300px;

}

.img-details *{
  padding-bottom:10px ;
}
.img-details>h5{
  color: white;

}

.img-details>p{
  color: #ccc;
  font-size: .6rem;
  word-spacing: 5px;
  line-height: 1rem;

}

.film-btn-group{
  width: 100%;
  display: flex;
  align-items: center;
}

.film-btn-group>*{
  color: #ccc;
  margin-right: .5rem;
}
.film-btn-group>svg{
  color: yellow;

}
.film-btn-group>span{
font-size: .6rem;
font-weight: 900;
}
</style>