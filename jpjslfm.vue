<template>
  <div>
    <div class="btn">
      <span class="register">注册</span>
      <span>取消</span>
    </div>
    <div class="hi">
      Hi,Kris <br> 欢迎回来！
    </div>
    <div class="signIn">
      <input class="sr" type="text" value="" placeholder="请输入您的账号">
    </div>
    <div class="signIn">
      <input class="sr sr1" :type="active?'text':'password'" value="" placeholder="请输入您的密码">
      <img class="getTp" src="../assets/images/ims.png" alt=""  @click="toggle">
    </div>
    <div class="signInB" :class="success?'success':''" @click="toggle1">
      登录
    </div>
    <div class="land" @click="skip">
      使用验证码登录
    </div>
  </div>
</template>

<script>
export default {
  name: 'jpjslfm',
  components: {

  },
  data () {
    return {
      active: false,
      success: false
    }
  },
  mounted () {
  },
  methods: {
    toggle () {
      this.active = !this.active
    },
    toggle1 () {
      this.success = !this.success
    },
    skip () {
      this.$router.push('/login')
    }
  }
}
</script>
<style scoped lang="less">
.btn{
  margin: 24px 50px;
  span{
  font-size: 28px;
  font-weight: 500;
  line-height: 22px;
  color: #737F97;
  display: block;
  }
  .register{
    color: #3861FB;
    float: right;
  }
}
.hi{
    margin: 84px 50px 0;
    font-size: 56px;
    font-weight: 600;
    line-height: 80px;
    color: #000000;
}
.signIn{
  position: relative;
  .sr{
    margin: 74px auto 14px;
    width: 650px;
    height: 66px;
    font-size: 30px;
    font-weight: 500;
    line-height: 42px;
    color: #000000;
    border: 0;
    border-bottom: 1px solid #F7F6FB;
    display: block;
  }
  .sr1{
      margin-top: 70px;
  }
  .getTp{
    position: absolute;
    top: 16px;
    right: 25px;
    width: 32px;
    height: 32px;
    background: #FFFFFF;
  }
}
.signInB{
  margin: 80px 50px 0;
  width: 650px;
  height: 80px;
  background: #3861fb;
  border-radius: 12px;
  font-size: 30px;
  font-weight: 500;
  line-height: 42px;
  color: #FFFFFF;
  text-align: center;
  line-height: 80px;
}
.success{
  background: #FFC1CBDF;
  color: #fff;
}
.land{
  margin-top: 34px;
  font-size: 28px;
  font-weight: 400;
  line-height: 40px;
  color: #000000;
  text-align: center;
}
</style>
