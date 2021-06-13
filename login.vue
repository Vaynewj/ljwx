<template>
  <div>
    <div class="loginBtn">
        <span class="cancel">注册</span>
        <span>取消</span>
    </div>
    <div class="loginWrap">
      <span class="signIn">登录</span>
      <span class="welcome">欢迎来到,矿多多</span>
      <div>
        <input type="text" value="" placeholder="请输入电话号码">
      </div>
      <div>
        <input type="text" value="" placeholder="请输入验证码">
        <i class="getCode" :class="active?'active':''" @click="send">获取验证码</i>
      </div>
      <div class="signInBtn" :class="success?'success':''" @click="signIn">
        登录
      </div>
      <div class="signIb" @click="skip">
        使用密码登录
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'login',
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
    send () {
      this.active = !this.active
    },
    signIn () {
      this.success = !this.success
    },
    skip () {
      this.$router.push('/jpjslfm')
    }
  }
}
</script>
<style scoped lang="less">
.loginBtn{
  margin: 24px 50px;
  span{
    font-size: 28px;
    font-weight: 500;
    color: #737F97;
    display: block;
  }
  .cancel{
    color: #3861FB;
    float: right;
  }
}
.loginWrap{
  margin: 84px 50px 0;
  .signIn{
    font-size: 56px;
    font-weight: 600;
    line-height: 40px;
    color: #000000;
    &::after{
      content: '';
      width: 58px;
      height: 10px;
      background: #3861FB;
      display: block;
      border-radius: 10px;
    }
  }
  .welcome{
    margin: 14px 0 46px;
    font-size: 26px;
    font-weight: 500;
    line-height: 22px;
    color: #C1CBDF;
  }
  div{
    position: relative;
    margin-top: 70px;
    input{
      width: 650px;
      height: 66px;
      font-size: 30px;
      font-weight: 500;
      line-height: 42px;
      color: #000000;
      border: 0;
      border-bottom: 1px solid #F7F6FB;
    }
    .getCode{
      position: absolute;
      top: 14px;
      right: 0;
      width: 140px;
      height: 52px;
      background: #FFFFFF;
      border: 2px solid #3861FB;
      border-radius: 198px;
      font-size: 22px;
      font-weight: 400;
      line-height: 32px;
      color: #3861FB;
      font-style: normal;
      text-align: center;
      line-height: 52px;
    }
    .active{
      background: #3861FB;
      color: #fff;
    }
  }
  .signInBtn{
    width: 650px;
    height: 80px;
    background: #C1CBDF;
    border-radius: 12px;
    text-align: center;
    font-size: 30px;
    font-weight: 500;
    line-height: 42px;
    color: #FFFFFF;
    line-height: 80px;
  }
  .success{
    background: #3861FB;
    color: #fff;
  }
  .signIb{
    margin-top: 34px;
    font-size: 28px;
    font-weight: 400;
    line-height: 40px;
    color: #000000;
    text-align: center;
  }
}
</style>
