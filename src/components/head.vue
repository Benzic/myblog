<template>
    <header class="header navbar-fixed-top" >
        <!-- Navbar -->
        <nav class="navbar" role="navigation">
            <div class="container">
                <!-- Brand and toggle get grouped for better mobile display -->
                <div class="menu-container js_nav-item">
                    <button type="button" class="navbar-toggle" data-toggle="collapse" data-target=".nav-collapse">
                        <span class="sr-only">Toggle navigation</span>
                        <span class="toggle-icon"></span>
                    </button>
    
                    <!-- Logo -->
                    <div class="logo">
                        <a class="logo-wrap" href="#body">
                            <img class="logo-img logo-img-main" src="../../static/images/logo.png" alt="Asentus Logo">
                            <img class="logo-img logo-img-active" src="../../static/images/logo-dark.png" alt="Asentus Logo">
                        </a>
                    </div>
                    <!-- End Logo -->
                </div>
    
                <!-- Collect the nav links, forms, and other content for toggling -->
                <div class="collapse navbar-collapse nav-collapse">
                    <div class="menu-container">
                        <ul class="nav navbar-nav navbar-nav-right">
                            <li class="nav-item"><a class="nav-item-child nav-item-hover">主页</a></li>
                            <li class="nav-item"><a class="nav-item-child nav-item-hover">文章</a></li>
                            <li class="nav-item"><a class="nav-item-child nav-item-hover">关于我</a></li>
                            <li class="nav-item"><a class="nav-item-child nav-item-hover">模板与demo分享</a></li>
                            <li class="nav-item"><a class="nav-item-child nav-item-hover">留言</a></li>
                            <li class="nav-item"><a class="nav-item-child nav-item-hover">登录</a></li>
                            <!-- <li class="js_nav-item nav-item"><a class="nav-item-child nav-item-hover" href="#body">主页</a></li>
                            <li class="js_nav-item nav-item"><a class="nav-item-child nav-item-hover" href="#about">文章</a></li>
                            <li class="js_nav-item nav-item"><a class="nav-item-child nav-item-hover" href="#experience">关于我</a></li>
                            <li class="js_nav-item nav-item"><a class="nav-item-child nav-item-hover" href="#work">模板与demo分享</a></li>
                            <li class="js_nav-item nav-item"><a class="nav-item-child nav-item-hover" href="#contact">留言</a></li>
                            <li class="js_nav-item nav-item"><a class="nav-item-child nav-item-hover" href="#work">登录</a></li> -->
                        </ul>
                    </div>
                </div>
            </div>
        </nav>
    </header>  
  </template>
  
  <script>
  export default {
    name: 'topBox',
    data () {
      return {
        msg: 'Welcome to Your Vue.js App'
      }
    }
  }
  </script>
  <style scoped>
      .nav-item-child{
          color: black;
      }
      header{
          background: #f1f1f1;
      }
  </style>
  