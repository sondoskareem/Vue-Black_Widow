<template>
    <div class="hero">
        <h1>Black Widow</h1>
        <div class="icons">

          <div class="icons-group">
            <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-star" viewBox="0 0 16 16">
              <path d="M2.866 14.85c-.078.444.36.791.746.593l4.39-2.256 4.389 2.256c.386.198.824-.149.746-.592l-.83-4.73 3.522-3.356c.33-.314.16-.888-.282-.95l-4.898-.696L8.465.792a.513.513 0 0 0-.927 0L5.354 5.12l-4.898.696c-.441.062-.612.636-.283.95l3.523 3.356-.83 4.73zm4.905-2.767-3.686 1.894.694-3.957a.565.565 0 0 0-.163-.505L1.71 6.745l4.052-.576a.525.525 0 0 0 .393-.288L8 2.223l1.847 3.658a.525.525 0 0 0 .393.288l4.052.575-2.906 2.77a.565.565 0 0 0-.163.506l.694 3.957-3.686-1.894a.503.503 0 0 0-.461 0z"/>
            </svg>
            <span> IMDB:7.4</span>
          </div>

          <div class="icons-group">
            <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-stopwatch" viewBox="0 0 16 16">
              <path d="M8.5 5.6a.5.5 0 1 0-1 0v2.9h-3a.5.5 0 0 0 0 1H8a.5.5 0 0 0 .5-.5V5.6z"/>
              <path d="M6.5 1A.5.5 0 0 1 7 .5h2a.5.5 0 0 1 0 1v.57c1.36.196 2.594.78 3.584 1.64a.715.715 0 0 1 .012-.013l.354-.354-.354-.353a.5.5 0 0 1 .707-.708l1.414 1.415a.5.5 0 1 1-.707.707l-.353-.354-.354.354a.512.512 0 0 1-.013.012A7 7 0 1 1 7 2.071V1.5a.5.5 0 0 1-.5-.5zM8 3a6 6 0 1 0 .001 12A6 6 0 0 0 8 3z"/>
            </svg>
            <span> DURATION:1H 58MIN</span>
          </div>

          <div class="icons-group">
           <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-calendar3" viewBox="0 0 16 16">
            <path d="M14 0H2a2 2 0 0 0-2 2v12a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V2a2 2 0 0 0-2-2zM1 3.857C1 3.384 1.448 3 2 3h12c.552 0 1 .384 1 .857v10.286c0 .473-.448.857-1 .857H2c-.552 0-1-.384-1-.857V3.857z"/>
            <path d="M6.5 7a1 1 0 1 0 0-2 1 1 0 0 0 0 2zm3 0a1 1 0 1 0 0-2 1 1 0 0 0 0 2zm3 0a1 1 0 1 0 0-2 1 1 0 0 0 0 2zm-9 3a1 1 0 1 0 0-2 1 1 0 0 0 0 2zm3 0a1 1 0 1 0 0-2 1 1 0 0 0 0 2zm3 0a1 1 0 1 0 0-2 1 1 0 0 0 0 2zm3 0a1 1 0 1 0 0-2 1 1 0 0 0 0 2zm-9 3a1 1 0 1 0 0-2 1 1 0 0 0 0 2zm3 0a1 1 0 1 0 0-2 1 1 0 0 0 0 2zm3 0a1 1 0 1 0 0-2 1 1 0 0 0 0 2z"/>
          </svg>
            <span> YEAR:2020</span>
          </div>
         
        </div>

        <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Nulla accusamus debitis ad, tenetur quis distinctio rerum delectus, eaque consequatur hic neque autem voluptate provident numquam quasi ducimus excepturi eveniet a.</p>

        <div class="buttons">
           
            <button class="btn btn-yellow">
               <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-caret-right-fill" viewBox="0 0 16 16">
                <path d="m12.14 8.753-5.482 4.796c-.646.566-1.658.106-1.658-.753V3.204a1 1 0 0 1 1.659-.753l5.48 4.796a1 1 0 0 1 0 1.506z"/>
              </svg>
              Watch Trailer
            </button>
           
            <button class="btn btn-light">
               <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-plus" viewBox="0 0 16 16">
                <path d="M8 4a.5.5 0 0 1 .5.5v3h3a.5.5 0 0 1 0 1h-3v3a.5.5 0 0 1-1 0v-3h-3a.5.5 0 0 1 0-1h3v-3A.5.5 0 0 1 8 4z"/>
              </svg>
              Add list
            </button>

        </div>
    
    </div>
</template>

<script>
export default {
  name: "Hero",
};
</script>
<style scoped>
.hero{
  width: 100%;
  position: absolute;
  top: 50%;
  left: 60%;
  transform: translate(-50% , -50%);
}
.hero>*{
  margin-bottom: 1rem;
}
.hero>h1{
  font-size: 2rem;
  color: white;
  letter-spacing: 4px;
}
.icons{
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 70%;
}
.icons-group{
  display: flex;
  justify-content: space-between;
  align-items: center;
  font-size: 1rem;
  font-size: .6rem;
  font-weight: 700;

}
.icons-group > *:first-child{
  margin-right: .7rem;
}
.icons-group>svg{
  color: yellow;

}
.icons-group>span , .hero>p{
  color: #ccc;

}

.hero>p{
  font-size: .6rem;
  word-spacing: 5px;
  line-height: 1rem;
  font-weight: 500;
  
}
.buttons{
  display: flex;
  align-items: center;
}

.btn{
  padding: .7rem 1.7rem;
  margin-right: 1rem;
  border-radius: 3rem;
  display: flex;
  align-items: center;
  justify-content: space-around;
  cursor: pointer;
}


.btn>svg{
  margin-right:5px ;
  border: none;
}
.btn-yellow{
  background-color: yellow;
}

</style>