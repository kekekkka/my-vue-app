

<template>
  <header class="no-login" id="header">
    <h1>LET'S SHARE</h1>
    <p>精品文章汇聚(如提交垃圾文章请勿展示在首页)</p>
    <div class="btns">
      <router-link to="/login">
        <el-button>立即登录</el-button>
      </router-link>
      <router-link to="/enroll">
        <el-button>注册账号</el-button>
      </router-link>
      
    </div>
  </header>




  <main class="main" v-for="n in 10">
    <a href="">
      <div><img src="/img/touxiang.jpg" alt="">
      <div class="zhanghao">
        1212245
      </div></div>
      
      <div class="wenzhang">
        <h3>了解一下HTML最常用的标签 <span>30天前</span></h3>
        
        
        <p>在很多网页中，我们可以看到很多十分有趣或者炫酷的动画特效，这些都可以由CSS来实现，只需要一点基础和明白浏览器是如何渲染这些页面的可以帮助我们更好的进行编程。</p>
      </div>

    </a>
  </main>
  <el-pagination class="pagination"
    :page-size="7"
    :pager-count="8"
    layout="prev, pager, next"
    :total="100"
  />
  <footer class="footer">©wangkefan.com 2023</footer>
</template>





<style scoped lang="scss">
.no-login {
  background: #149739;
  text-align: center;
  color: white;
  padding: 40px;

  h1 {

    padding: 20px 0;
    font-size: 40px;
  }

  p {
    padding: 10px 0 40px;
    font-size: 14px;
  }

  .btns {
    button {
      margin: 0 10px;
      padding: 18px;
    }
  }

}

.main {
  padding: 0 0 0 140px;
  margin: 30px 0 54px 100px;
  a {
    display: flex;
    color:#000;

    img {
      width: 60px;
      
    }
    .wenzhang{
     position: relative;
      margin: 0 0 0 36px;
     h3{
    font-size: 16px;
    margin: 0 0 30px;
    span{
      font-weight: normal;
      font-size: 6px;
      color: #999;
    }
     }
     p{
      font-size: 14px;
      white-space:nowrap/*禁止自动换行*/
     }
     .riqi{
      top: 0;
      left: 180px;
      position: absolute;
     }
    }
   .zhanghao{
    font-size: 12px;
    text-align: center;
    color: #999;
   }
  }

}
.pagination{
  justify-content: center;
  padding-bottom: 20px;
}
.footer{
  background:#D7D7D7;
  text-align: center;
  padding: 26px 0;
  font-size: 12px;
  color: #756675;
 
}
</style>