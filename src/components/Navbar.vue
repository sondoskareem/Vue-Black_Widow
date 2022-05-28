<template>
  <div class="nav-container">
    <div class="left-side">

      <div class="logo">LOOP</div>

      <div class="nav">
        <ul>
          <li><a href="#">Home</a></li>
          <li><a href="#">About</a></li>
          <li><a href="#">Series</a></li>
          <li><a href="#">My list</a></li>
          <li><a href="#">Blog</a></li>
        </ul>
      </div>

    </div>

    <div class="right-side">
        <div class="search">
            <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-search" viewBox="0 0 16 16">
                <path d="M11.742 10.344a6.5 6.5 0 1 0-1.397 1.398h-.001c.03.04.062.078.098.115l3.85 3.85a1 1 0 0 0 1.415-1.414l-3.85-3.85a1.007 1.007 0 0 0-.115-.1zM12 6.5a5.5 5.5 0 1 1-11 0 5.5 5.5 0 0 1 11 0z"/>
            </svg>
            <input type ="text" placeholder="Search For Movies...">
        </div>
        <div class="notifications">
            <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-bell-fill" viewBox="0 0 16 16">
                <path d="M8 16a2 2 0 0 0 2-2H6a2 2 0 0 0 2 2zm.995-14.901a1 1 0 1 0-1.99 0A5.002 5.002 0 0 0 3 6c0 1.098-.5 6-2 7h14c-1.5-1-2-5.902-2-7 0-2.42-1.72-4.44-4.005-4.901z"/>
            </svg>
            <span class="count"><span>8</span></span>
        </div>
        <div class="profile">
            <img src="./../assets/profile.jpg" height="50" width="50" alt="">
            <span>Walter Mellon</span>
            <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-caret-down-fill" viewBox="0 0 16 16">
                <path d="M7.247 11.14 2.451 5.658C1.885 5.013 2.345 4 3.204 4h9.592a1 1 0 0 1 .753 1.659l-4.796 5.48a1 1 0 0 1-1.506 0z"/>
            </svg>
        </div>
    </div>

  </div>
</template>
<script>
export default {
  name: "Navbar",
};
</script>

<style scoped>
.nav-container{
    margin-top: 1rem;
}
.nav-container,.left-side , .right-side,.profile{
    display: flex;
    justify-content: space-around;
    align-items: center;
}
.left-side> .logo{
    color: yellow;
    font-weight: bold;
    letter-spacing: 2px;
}
.logo{
    margin-right: 2rem;
}
.nav{
    display: flex;
}
.nav>ul li{
   list-style: none;
    display: inline-block;
    margin: 0 1rem;
    position: relative;

}
.nav>ul li a{
    color: #ccc;
    text-decoration: none;
    font-size: .7rem;
    font-weight: 100;
    transition: 0.5s;

}
.nav>ul li a:hover{
    color: #fff;
   
}
.right-side>.search>svg{
color: white;
margin-right: 1rem;
cursor: pointer;

}
.right-side>.search>input{
    background: transparent;
    border: none;
    color: white;
}
.search>input:focus{
    outline: none;
}
.search{
    display: flex;
    justify-content: space-between;
    align-items: center;
}
.notifications{
    color: rgb(255, 255, 255); 
    font-weight: 900;
    font-size: 20px;
    margin-right: 20px;
    position: relative;
    cursor: pointer;
}
.count{
    position: absolute;
    width:1px;
    height: 10px;
    top: -10px;
    right: -10px;
    padding: 5px 10px;
    border-radius: 50%;
    background: red;
    color: white;
    text-align: center;
}
.count span{
    font-size: 10px;
    color: white;
    position: absolute;
    top: 24%;
    left: 40%;
    

}
.profile{
    margin-left: 2rem;
}
.profile * {
    margin-left: .5rem;
}

.profile>img{
    border-radius: 50px;
    border: 1px solid white;
    cursor: pointer;
}
.profile>span{
  display: block;
  width: 80px;
  overflow: hidden;
  white-space: nowrap;
  text-overflow: ellipsis;
}

.profile>span , .profile>svg{
   font-size: .8rem;
   color: white;
   cursor: pointer;
}
</style>
