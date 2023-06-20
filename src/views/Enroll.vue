
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
    <main>
        <div class="yonghu ">
            <h5>用户名</h5>
            <el-input class="name" v-model="input" placeholder="用户名" />
        </div>
        <div class="mima">
            <h5>密码</h5>
            <el-input class="password" v-model="input" placeholder="密码" />
        </div>
       
    </main>
    <div class="btn"><el-button>立即注册</el-button></div>
    <p class="xiaozi">已有账号<a href="./#/login" style='color:#6B996B;'>立即登录</a></p>
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

main {
    text-align: center;
    .yonghu {
        h5 {
            margin: 40px 0 10px;
        }
    }
     .mima {
        display:inline-block;
        h5 {
          margin: 16px 0 10px ;
            text-align: left;
        }
    }
    .name, .password {
        width: 300px;
    }
}
.btn{
//   margin: 30px 0 0 484px;
}
.xiaozi{
    text-align: center;
    margin-top: 40px;
    font-size: 12px;
    color: #999;
}
.footer{
    
   margin: 0;
  background:#D7D7D7;
  text-align: center;
  position: fixed;
  padding: 26px  0;
  font-size: 12px;
  color: #756675;
  bottom: 0;
 width: 100%;
}
</style>

<script lang="ts" setup>
import { ref } from 'vue'
const input = ref('')
</script>