<template >
<div class="navbar">
  <div class="brand">
    <span>BRAND</span>
  </div>
  <ul>
    <li><a href="#"> anasayfa 1</a></li>
    <li><a href="#"> anasayfa 2</a></li>
    <li><a href="#"> anasayfa 3</a></li>
    <li><a href="#"> anasayfa 4</a></li>
  </ul>
  <div class="icon">
  <i class="fas fa-align-justify" style="color:white;"></i>
  </div>
</div>
</template>
<script>
export default {
  methods: {
    /* myFunction(){
            let a = document.getElementById("myTopnav");
            if (a.className === "topnav") {
                a.className += "responsive";
            } else{
                a.className = "topnav";
            }
        } */
  }
}

</script>
<style >
.navbar{
  width: 100%;
  height: 60px;
  background-color: black;
  display: flex;
  justify-content: center;
  align-items: center;
}
.navbar>ul>li{
  float: right;
}
.navbar>ul>li>a{
  padding: 10px;
  font-size: 20px;
  font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
  color: white;
  text-decoration: none;
}
.navbar>ul>li>a:hover{
  background-color: white;
  color: black;
  width: 100%;
  height: 100vh;
}
.brand{
  float: left;
  color: white;
}
@media screen and (max-width:800px){
  .navbar>ul{
    display: none;
  }
}
.icon{
  color: white;
}

</style>
