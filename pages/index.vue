<template>
  <div class="main">
    <div class="profile">
      <img class="profile-img" src="~/assets/hoshi.jpg" alt="">
      <ul class="profile-text">
        <li>星 昂一郎 17才</li>
        <li>N高等学校在籍3年生</li>
        <li>e-Sportsが好き</li>
      </ul>
    </div>
    <div class="skills">
      使える技術
      <ul class="lang">
        言語
        <li class="lang-name">javascript</li>
      </ul>
      <ul class="lang">
        フレームワーク、ライブラリ
        <li class="lang-name">JQuery</li>
      </ul>
    </div>
  <div class="skills">
      勉強中
      <ul class="lang">
        言語
        <li class="lang-name">Golang</li>
      </ul>
      <ul class="lang">
        フレームワーク、ライブラリ
        <li class="lang-name">Vue.js</li>
      </ul>
    </div>
    <div class="product">
      作品一覧
      <div class="product-frame">
        <nuxt-link to="./nuxt_netlify">
        <ul  class="product-name">
          Nuxt.js + NetlifyでSPA
          <li class="product-info">Nuxt.jsとNetlifyを使ってポートフォリオ用サイトのSPAを作りました</li>
        </ul>
        </nuxt-link>
      </div>
    </div>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  }
}
</script>

<style>
body{
  margin: 0;
  font-family: 'TsukuARdGothic-Regular','Hiragino Kaku Gothic ProN','ヒラギノ角ゴ ProN W3','ＭＳ 明朝', 'MS Mincho',sans-serif;
  font: 'TsukuARdGothic-Regular','Hiragino Kaku Gothic ProN','ヒラギノ角ゴ ProN W3','ＭＳ 明朝', 'MS Mincho';
  color: #707070;
}
li{
  list-style: none;
}
ul{
  list-style: none;
}
.lang-name{
  font-size: 20px;
  padding-left: 35px;
}
.skills{
  font-size: 30px;
  width: 600px;
  margin: auto;
  text-align: left;
}
.main{
  max-width:1240px;
  margin:0px auto;
  text-align: center;
}
.profile{
  margin: 30px;
  display:inline-flex;
}
.profile-img{
  border: 1px solid #707070;
  height: 250px;
  width: 250px;
  border-radius: 125px;
}
.profile-text{
  margin-top: 50px;
  font-size: 35px;
}
.product-frame{
  transition: 0.3s ease-in-out;
  margin: 0 auto;
  width: 80%;
  height: 120px;
  border: #707070 solid 0.5px;
}
.product{
  text-align: left;
  font-size: 30px;
  text-align: center;
  margin: 0 auto;
}
.product-frame:hover{
  background-color: #e6e6e6;
}
.product-name{
  color: #707070;
  text-decoration:none;
  padding-left: 10px;
  padding-top: 5px;
  text-align: left;
  font-size: 20px;
}
.product-info{
  color:#707070;
  padding-left: 20px;
  padding-top: 10px;
  text-align: left;
  font-size: 15px;
}
a{
  text-decoration: none;
}

</style>
