<template>
    
    <div class="box">
            <div class="bgPic img" style="background: url(../../static/images/1920x1080/02.jpg) no-repeat center center; background-size: cover">
            </div>
            <topBox></topBox>
            <div class="container">
                <div class="leftPart">
                    <h3>最新文章</h3>
                    <ul>
                        <li v-for='n in 7'>
                            <div class="img" style="background-image: url(../../static/images/800x400/01.jpg) no-repeat center center; background-size: cover;">
                            </div>
                            <div class="info">
                                <div class="title">编程的艺术</div>
                                <div class="des">这是一本书</div>
                            </div>
                        </li>
                    </ul>
                </div>
                <div class="rightPart">
                    <div class="mine">
                        <h3>关于我</h3>
                        <p class="name">网名：Benzic</p>
                        <p class="wechat">微信：youmy_love</p>
                        <p class="email">邮箱：690018019@qq.com</p>
                        <p class="job">职业：web前端工程师 | 道格腾</p>
                    </div>
                    <div class="rank">
                        <h3>热度排行</h3>
                        <ul>
                            <li v-for='n in 13'>
                                <a href="">
                                    <span>编程的艺术</span>
                                    <span>热度：1000</span>
                                </a>
                            </li> 
                        </ul>
                    </div>
                </div>
                <div class="demo">
                    <h3>模板和demo分享</h3>
                    <ul>
                        <li v-for='n in 8'>
                            <div class="img" style='background: url(../../static/images/800x400/01.jpg) no-repeat center center; background-size: cover'></div>
                            <p>这是一个什么养的末班牛逼的阿斯顿牛逼的阿斯顿牛逼的阿斯顿牛逼的阿斯顿牛逼38字...</p>
                        </li>
                    </ul>
                    
                </div> 
            </div>
            <div ></div>
            <bottomBox></bottomBox>
    </div>
</template>

<script>
import topBox from '../components/head';
import bottomBox from '../components/footer';
export default {
name: 'index',
    data () {
        return {
        msg: 'Welcome to Your Vue.js App'
        }
    },
    components:{
        topBox,
        bottomBox
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    .container{
        width: 80%;
        height: auto;
        display:flex;
        margin-top: 1rem;
        min-height: 7rem;
        flex-wrap: wrap;
        overflow: hidden;
    }
    li{
        list-style: none;
    }
    .bgPic{
        width: 100%;
        height: 100%;
        position: fixed;
        left: 0;
        top: 0;
        z-index: -1;
        background-position: center center;
        background-size: contain;
        background-repeat: no-repeat;
    }
    .leftPart{
        width: 78%;
        height: 7rem;
        box-shadow: 0.1rem 0.1rem 0.3rem gray;
        border-radius: 0.1rem;
        padding: 0.1rem;
        background: white;
        margin-right: 2%;
        overflow: hidden;
    }
    .leftPart ul li{
        display: flex;
        margin-bottom: 0.1rem;
        text-align: left;
    }
    .leftPart ul li .img{
        margin-right: 0.2rem;
        width: 1.5rem;
        height: 0.75rem;
    }
    .leftPart ul li .title{
        font-size: 0.18rem;
    }
    .leftPart ul li .info{
        display: flex;
        flex-direction:column;
        justify-content: center;
    }
    .leftPart ul li .des{
        font-size: 0.14rem;
    }
    .rightPart{
        width: 20%;
        height: 7rem;
    }
    .mine {
        width: 100%;
        height: 38%;
        box-shadow: 0.1rem 0.1rem 0.3rem gray;
        border-radius: 0.1rem;
        padding: 0.1rem;
        background: white;
        margin-bottom: 0.1rem;
        overflow: hidden;
    }
    .mine p{
        width: 100%;
        text-align: left;
    }
    .rank{
        width: 100%;
        height: 60%;
        box-shadow: 0.1rem 0.1rem 0.3rem gray;
        border-radius: 0.1rem;
        padding: 0.1rem;
        background: white;
        overflow: hidden;
    }
    .rank ul{
        text-align: left;
    }
    .rank li{
        margin-bottom: 0.1rem;
    }
    .rank li a{
        display: flex;
        justify-content: space-between;
        padding: 0 0.1rem;
    }
    .demo{
        width: 100%;
        min-height: 3.5rem;
        background: white;
        margin-top: 10px;
        box-shadow: 0.1rem 0.1rem 0.3rem gray;
        border-radius: 0.1rem;
        padding: 0.1rem;
    }
    .demo ul {
        display: flex;
        justify-content: space-between;
        flex-wrap: wrap;
    }
    .demo .img{
        width: 2rem;
        height: 1.5rem;
    }
    .demo li{
        width: 2rem;
        height: 2.2rem;
        border-radius: 0.1rem;
        box-shadow: 0.1rem 0.1rem 0.1rem gray;
        margin-right: 0.1rem;
        margin-bottom: 0.1rem;
        text-align: center;
        text-overflow: ellipsis;
    }
    @media screen and (max-width: 1200px){
        .container{
            width: 95%;
            min-height: 10rem;
        }
        .leftPart{
            width: 100%;
            margin-right: 0;
            margin-bottom: 0.1rem;
        }
        .rightPart{
            width: 100%;
        }
    }
</style>
      