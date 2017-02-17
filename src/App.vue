<template>
  <!--<div id="app">-->
  <div id="fullpage">
    <div class="section pg1">
      <hello></hello>
    </div>
    <div class="section pg2"></div>
    <div class="section">
      <div class="slide tm_slide" id="pg3_1">
        <span class="slide_detail">
          <a href="http://www.jianianle.com/" target="_blank">进入详情 ></a>
        </span>
      </div>
      <div class="slide tm_slide" id="pg3_2">
        <span class="slide_detail">
          <a href="http://sj.qq.com/myapp/detail.htm?apkName=com.diisuu.huita" target="_blank">进入详情 ></a>
        </span>
      </div>
    </div>
    <div class="section pg4">
      <div id="bottom_mobile"><img src="../static/img/line_01.jpg"><span>15658132456</span></div>
      <div id="bottom_qq"><img src="../static/img/line_02.jpg"><span>617405347</span></div>
    </div>
  </div>
  <!--</div>-->
</template>

<script>
  import Hello from './components/Hello'
  import $ from 'jquery'
  import jqueryEasing from 'jquery.easing'
  import fullPage from 'fullpage.js'

  $(document).ready(function () {
    $('#fullpage').fullpage({
      sectionsColor: ['black', 'white', 'gray', '#1e1b1e'],
      controlArrows: false,
      resize: true,
      scrollingSpeed: 1000,
      anchors: ['page1', 'page2', 'page3', 'page4'],
      recordHistory: false,
//      menu: '#nav',
      navigation: true,
      navigationPosition: 'right',
      slidesNavigation: true,
      navigationColor: '#fff',
      slidesNavPosition: 'bottom'
    });
  });

    setInterval(function () {
      $.fn.fullpage.moveSlideRight();
    }, 10000);

  export default {
    name: 'app',
    components: {
      Hello
    }
  }
</script>

<style>
  @import "assets/lib/css/jquery.fullPage.min.css";

  #fp-nav ul li a span, .fp-slidesNav ul li a span {
    background-color: white;
  }

  a {
    text-decoration: none;
  }

  .section {
    background-repeat: no-repeat;
    background-size: cover;
    background-position: center;
  }

  div .pg1 {
    background-image: url(../static/img/pg_01.png);
    /*background-size: cover;*/
  }

  div .pg2 {
    background-image: url(../static/img/pg_02.png);

  }

  div .pg4 {
    background-image: url(../static/img/pg_04.png);
    background-size: contain;
    background-position: top;
  }

  #bottom_mobile {
    position: absolute;
    top: 75%;
    left: 25%;
    height: 100%;
    width: 100%;
  }

  #bottom_qq {
    position: absolute;
    top: 75%;
    left: 55%;
    height: 100%;
    width: 100%;
  }

  .pg4 div span {
    color: white;
    font-size: 2.5vw;
    display: inline-block;
    position: absolute;
    margin: 0 auto;
    padding-left: 1%;
    padding-top: 1%;
  }

  #pg3_1 {
    background-image: url(../static/img/pg_03_01.png);
    background-size: cover;
    background-position: center;
  }

  #pg3_2 {
    background-image: url(../static/img/pg_03_02.png);
    background-size: cover;
    background-position: center;
  }

  .slide_detail {
    width: 15%;
    display: block;
    position: relative;
    left: 23%;
    top: 24%;

  }

  .slide_detail a {
    color: white;
    font-size: 1.5rem;
  }
  .slide_detail a:hover {
    color: #ff0000;
  }
</style>
