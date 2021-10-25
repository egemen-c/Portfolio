<template>
<div class="preloader"> <img class="preloader-icon" src="144.gif" alt="My Site Preloader"> </div>
  <div class="container">
    <div class="head">
    <h1>EGEMEN<span class="break">ÇELİK</span></h1>
    </div>
    <div class="alt">
    <h2>JUNİOR FRONT-END DEVELOPER & DESİGNER BASED IN ANKARA</h2>
    </div>
    <ul class="links">
      <li><a href="mailto:egemencelikx@gmail.com">EMAİL</a></li>
      <li><a href="">GİTHUB</a></li>
      <li><a href="">LİNKEDİN</a></li>
      <li><a href="">UPWORKS</a></li>
    </ul>
  </div>
</template>

<script>

export default {
  name: 'App',
  components: {

  },
  mounted () {
    this.pageload()
  },
  methods: {
    pageload () {
      document.querySelector('.preloader').style.display = 'none'
    }
  }
}
</script>
<style>
@import url('https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Open+Sans&family=Unica+One&display=swap');
        .preloader{
            width: 100%;
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            background-color: black;
        }
        .preloader>img>{
            width: 250px;
            z-index: 2;
            height: 250px;
        }
.container{
  width: 100%;
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
}
.alt>h2{
  color:#ccc;
  font-family: 'Unica One', cursive;
  font-size: 1.125em;
  font-weight: 200;
  letter-spacing: .025em;
  transform: scale(1.2);
  }
  .head{
    display: flex;

  }
.head>h1{
  transform: scale(1.2);
  font-size: 6em;
  line-height: 1.6em;
  font-weight: 800;
  font-family: 'Open Sans', sans-serif;
  letter-spacing: .035em;
  color: #eee;
  font-family: 'Open Sans', sans-serif;
}
  body{
        width: 100%;
        height: 100vh;
        background: url("assets/photo4.jpg") center fixed  no-repeat ;
        background-size: cover;
      }
.links{
    position: fixed;
    bottom: 30px;
    left: 40px;
    right: 40px;
    z-index: 2;
    list-style: none;
    margin: 0;
    padding: 0;
    text-align: center;
}
.links>li{
  display: inline-block;
}
.links>li>a{
  padding: 6px 4px;
    font-size: .688em;
    font-weight: 700;
    color: #666;
    text-transform: uppercase;
    text-decoration: none;
}
@media screen and (max-width: 900px) {
  .head>h1{
    transform: scale(1);
  }
  .alt>h2{
    transform: scale(1);
  }
}
@media screen and (max-width: 700px) {
  .break{
    display: block;
    text-align: center;
    margin-top: -0.60em;
  }
  .alt{
    margin-top:0.5em;
  }
    .head>h1{
    transform: scale(0.90);
  }
  .alt>h2{
    transform: scale(0.95);
    text-align: center;
  }
}
</style>
