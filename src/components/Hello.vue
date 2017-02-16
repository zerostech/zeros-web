<template>
  <div id="top-bar">
    <div id="logo">
      <img id="nav-logo" src="../../static/img/logo.png">
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
      <img src="../../static/img/tel_logo.png">
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
    top: 0;
    z-index: 999;
    padding: 0;
    height: 4.25rem;
    background: white;
    /*filter:alpha(Opacity=60);-moz-opacity:0.6;opacity: 0.6;*/
  }

  #logo {
    float: left;
    /*width: 10%;*/
    padding-left: 17%;
  }

  #logo img {
    width: 75%;
    height: 75%;
    position: relative;
    margin-top: 8%;
  }

  #nav {
    width: 40%;
    position: absolute;
    top: 0;
    left: 30%;
  }

  #tel {
    float: right;
    padding-right: 32%;
    /*width: 10%;*/
    /*height: 75%;*/
    /*padding-top: 10%;*/
  }

  #tel img {
    width: 75%;
    height: 75%;
    position: relative;
    margin-top: 13%;
  }

  a {
    text-decoration: none;
  }

  #nav ul {
    /*width:100%;*/
    /*height:35px;*/
    top: 0;
    display: inline;
  }

  #nav ul li {
    width: 20%;
    height: 100%;
    float: left;
    list-style: none;
    text-align: center;
  }

  #nav ul li a {
    display: block;
    /*text-indent: 30px;*/
    height: 100%;
    line-height: 4.25rem;
    color: #000;
    font-size: 1vw;
    font-family: "Helvetica", "Tahoma", "Arial", "PingFang SC", "Microsoft JhengHei", "SimSun", "sans-serif";
    font-weight: 500;
  }

  #nav ul li a:hover {
    color: #ff0000;
  }
</style>
