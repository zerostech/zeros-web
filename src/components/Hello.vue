<template>
  <div id="top-bar">
    <div id="head-bar">
      <div id="logo">
        <a href="../../index.html"><img id="nav-logo" src="static/img/logo.png"></a>
      </div>
      <div id="nav">
        <ul>
          <li data-menuanchor="page1" class="active"><a href="#page1">首页</a></li>
          <li data-menuanchor="page2"><a href="#page2">团队名介绍</a></li>
          <li data-menuanchor="page3"><a href="#page3">优秀项目</a></li>
          <li data-menuanchor="page4"><a href="#page4">成功案例</a></li>
        </ul>
      </div>
      <div id="tel">
        <a href="#page4"><img src="static/img/tel_logo.png"></a>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'hello'
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

  #top-bar {
    width: 100%;
    position: fixed;
    top: 0px;
    z-index: 999;
    /*padding: 0;*/
    height: 70px;
    background: white;
    padding: 0;
    /*filter:alpha(Opacity=60);-moz-opacity:0.6;opacity: 0.6;*/
  }
#head-bar{
  width: 1226px;
  height: 70px;
  margin: 0px;
  position: relative;
  display: block;
  /*background-color: red;*/
  margin: 0 auto;
  /*padding: 0;*/
}
  #logo {
    height: 50px;
    position: absolute;
    display: block;
    margin-top: 10px;
    margin-left: 200px;

  }
  #logo a{
    height: inherit;
  }
  #logo a img {
    height: inherit;
  }

  #nav {
    width: 600px;
    position: absolute;
    padding-top: 25px;
    top: 0;
    left: 350px;
  }

  #nav ul {
    -webkit-margin-before: 0;
    -webkit-margin-after: 0;
    -webkit-margin-start: 0;
    -webkit-margin-end: 0;
    -webkit-padding-start: 0;
  }

  #nav ul li {
    width: 125px;
    float: left;
    list-style: none;
    text-align: center;
  }

  #nav ul li a {
    display: block;
    color: #000;
    font-family: "Helvetica", "Tahoma", "Arial", "PingFang SC", "Microsoft JhengHei", "SimSun", "sans-serif";
  }

  #nav ul li a:hover {
    color: #ff0000;
  }

  #tel {
    position: relative;
    left: -250px;
    padding-top: 10px;
    float: right;
    display: block;
  }

  #tel img {

    height: 50px;

  }

</style>
