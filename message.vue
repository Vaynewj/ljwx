<template>
  <div>
    <div class="messageBtn">
      <span class="messageTop">消息</span>
    </div>
    <div class="messageOn">
      <div class="imgS">
        <img class="messageImg" src="../assets/09.png" alt="">
      </div>
      <div class="imgA">
        <span class="message1">站内信</span>
        <i class="message2">暂无最新消息</i>
      </div>
    </div>
    <div>
      <div class="imgB">
        <div class="imgC">
          <img class="imgD" src="../assets/10.png" alt="">
        </div>
        <div class="img1">
          <span class="imgE">
          客服: Kris
          <i class="imgF">您好，关于订单的咨询请在下单之后询问</i>
        </span>
        </div>
      </div>
      <div class="imgB">
        <div class="imgC">
          <img class="imgD" src="../assets/10.png" alt="">
        </div>
        <div class="img1">
          <span class="imgE">
          客服: Ameber
          <i class="imgF">您好，关于订单的咨询请在下单之后询问</i>
        </span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'message',
  components: {

  },
  data () {
    return {

    }
  },
  mounted () {
  },
  methods: {

  }
}
</script>
<style scoped lang="less">
.messageBtn{
  width: 750px;
  height: 88px;
  background: #FFFFFF;
  .messageTop{
    margin: 24px 344px 22px 346px;
    font-size: 30px;
    font-weight: 500;
    line-height: 42px;
    color: #000000;
    text-align: center;
  }
}
.messageOn{
  display: flex;
  width: 750px;
  height: 112px;
  background: #FFFFFF;
  .imgS{
    .messageImg{
    margin: 22px 28px 18px 30px;
    width: 72px;
    height: 72px;
    }
  }
  .imgA{
     .message1{
      font-size: 28px;
      font-weight: 500;
      line-height: 40px;
      color: #000000;
  }
    .message2{
      display: block;
      font-size: 24px;
      font-weight: 500;
      line-height: 34px;
      color: #B1B1B1;
      font-style: normal;
   }
  }
}
.imgB{
  display: flex;
  .imgC{
    .imgD{
      margin: 38px 38px;
      width: 72px;
      height: 72px;
      background: #3396FC;
      border-radius: 50%;
      line-height: 72px;
    }
  }
  .img1{
    margin: 15px;
    .imgE{
    font-size: 28px;
    font-weight: 500;
    line-height: 40px;
    color: #000000;
    .imgF{
      display: block;
      font-size: 24px;
      font-weight: 400;
      line-height: 34px;
      color: #8E8E8E;
      font-style: normal;
    }
    }
  }
}
</style>
