<template>
  <div class="body1">
    <div class="searchBtn">
      <div>
        <img class="menuBtn" src="../assets/02.png" alt="">
      </div>
      <div class="search">
        <img class="searchImg" src="../assets/search.png" alt="">
        <input class="searchBt" type="text" value="" placeholder="搜索您关心的币种">
      </div>
      <img class="Imgs"  src="../assets/01.png" alt="">
    </div>
    <div class="swiper-container">
      <div class="swiper-wrapper">
        <div class="swiper-slide">
          <img src="https://ss0.bdstatic.com/70cFvHSh_Q1YnxGkpoWK1HF6hhy/it/u=102338098,1020664778&fm=26&gp=0.jpg" alt="">
        </div>
        <div class="swiper-slide">
          <img src="https://ss1.bdstatic.com/70cFvXSh_Q1YnxGkpoWK1HF6hhy/it/u=1204362579,1611455122&fm=26&gp=0.jpg" alt="">
        </div>
        <div class="swiper-slide">
          <img src="https://gimg2.baidu.com/image_search/src=http%3A%2F%2Fbpic.588ku.com%2Fback_pic%2F04%2F95%2F89%2F895927db3b76ff2.jpg&refer=http%3A%2F%2Fbpic.588ku.com&app=2002&size=f9999,10000&q=a80&n=0&g=0n&fmt=jpeg?sec=1626160320&t=3f3a23cf90efbde8bc0fdc6eeaf6e0b5" alt="">
        </div>
    </div>
    <!-- 如果需要分页器 -->
    <div class="swiper-pagination"></div>

    <!-- 如果需要导航按钮 -->
    <div class="swiper-button-prev"></div>
    <div class="swiper-button-next"></div>

    <!-- 如果需要滚动条 -->
    <div class="swiper-scrollbar"></div>
    </div>
    <div class="text">
      <img class="iMg" src="../assets/02.png" alt="">
      <span class="textBtn">MineMore将于3月1日开启“IOST锁仓赚币”活动</span>
      <img class="iMgs" src="../assets/04.png" alt="">
    </div>
    <div class="show">
       <div class="sbox">
         <div class="Id">
         ETH/USDT
         <i class="rateBtn">-4.76%</i>
       </div>
       <div class="rate">
         1215.55
       </div>
       <div class="faceValue">
         ￥7785.59
       </div>
       </div>
        <div class="bbox">
           <div class="Id">
          HT/USDT
          <i class="rateBtn">-2.04%</i>
          </div>
          <div class="rate">
          5.2810
          </div>
          <div class="faceValue">
          ￥33.82
           </div>
        </div>
       <div>
         <div class="Id">
         USDT/HUSD
         <i class="rateBn"> +0.03%</i>
       </div>
       <div class="rate">
         0.9997
       </div>
       <div class="faceValue">
         ￥6.40
       </div>
       </div>
    </div>
    <div class="click">
      <div class="easy">
        <img class="imG" src="../assets/05.png" alt="">
        <div class="buy">快捷买币</div>
      </div>
      <div class="easy">
        <img class="imG" src="../assets/06.png" alt="">
        <div class="buy">新手指南</div>
      </div>
      <div class="easy">
        <img class="imG" src="../assets/07.png" alt="">
        <div class="buy">分享福利</div>
      </div>
      <div class="easy">
        <img class="imG" src="../assets/08.png" alt="">
        <div class="buy">联系客服</div>
      </div>
    </div>
    <div class="choose">
      <div class="recommend">
      <span class="gmrecommend">官方推荐,收益可见</span>
      <span class="mrecommend">MineMore精品推荐</span>
      </div>
      <div class="selected">
        <span class="selectedBtn">稳健精选</span>
        <span class="more">更多</span>
      </div>
      <div class="safe">
        安稳可靠,安心持有不操心
      </div>
      <div class="cbox">
        <div class="abox">
        <div class="lease">
        <div class="model">租赁型矿机-云池1</div>
        <div class="fValue">0.68954510 BTC</div>
        <div class="timeBtn">理论产出(年)</div>
        <div class="year">6000.00000 USDT</div>
      </div>
      </div>
      <div class="abox">
        <div class="lease">
        <div class="model">租赁型矿机-云池2</div>
        <div class="fValue">0.68954510 BTC</div>
        <div class="timeBtn">理论产出(年)</div>
        <div class="year">6000.00000 USDT</div>
      </div>
      </div>
      </div>
    </div>
  </div>
</template>

<script>
import Swiper from 'swiper'
export default {
  name: 'index',
  components: {

  },
  data () {
    return {

    }
  },
  mounted () {
    /* eslint-disable-next-line */
    new Swiper('.swiper-container', {
      autoplay: {
        dely: 2000
      },
      loop: true,
      // 分页器
      pagination: '.swiper-pagination',
      // 前进后退
      nextButton: 'swiper-button-next',
      prevButton: 'swiper-button-prev',
      // 滚动条
      scrollbar: '.swiper-scrollbar'
    })
  },
  methods: {

  }
}
</script>
<style scoped lang="less">
.body1{
  background: #F7F6FB;
  .searchBtn{
  display: flex;
  justify-content: space-evenly;
  .menuBtn{
    width: 52px;
    height: 52px;
    border-radius: 50%
  }
  .search{
    width: 570px;
    height: 52px;
    background: #F0F1F3;
    border-radius: 198px;
    display: flex;
    align-items: center;
    .searchImg{
      margin-left: 15px;
      float: left;
      width: 28px;
      height: 29px;
    }
    .searchBt{
      float: left;
      border: 0;
      width: 400px;
      height: 40px;
      font-size: 22px;
      font-weight: 400;
      line-height: 32px;
      color: #969DA4;
      background: #F0F1F3;
      text-align: left;
    }
  }
  .Imgs{
    width: 48px;
    height: 48px;
  }
}
.swiper-container{
      margin: 10px 20px 24px;
      width: 710px;
      height: 280px;
      background: rgba(0, 0, 0, 0);
      border-radius: 20px;
  .swiper-wrapper{
    .swiper-slide{
    }
  }
}
.text{
  line-height: 22px;
  vertical-align: middle;
  height: 22px;
  margin: 24px 20px;
  background: #FFFFFF;
  .textBtn{
    font-size: 22px;
    font-weight: 500;
    line-height: 32px;
    color: #000000;
    float: left;
    padding: 5px;
  }
  .iMg{
    width: 40px;
    height: 40px;
    float: left;
    line-height: 22px;
  }
  .iMgs{
    line-height: 22px;
    width: 32px;
    height: 24px;
    float: right;
  }
}
.show{
  display: flex;
  margin: 16px 20px 60px 34px;
  align-items: center;
  justify-content: space-evenly;
  background: #FFFFFF;
  .Id{
    font-size: 22px;
    font-weight: 600;
    line-height: 32px;
    color: #000000;
    .rateBtn{
      font-size: 20px;
      font-weight: 400;
      line-height: 28px;
      color: #E53A43;
      font-style: normal;
    }
    .rateBn{
    font-size: 20px;
    font-weight: 400;
    line-height: 28px;
    color: #51CCB0;
    font-style: normal;
    }
  }
  .rate{
    font-size: 36px;
    font-weight: 600;
    line-height: 50px;
    color: #E53A43;
  }
  .faceValue{
    font-size: 20px;
    font-weight: 400;
    line-height: 28px;
    color: #969DA4;
  }
}
.click{
  margin: 20px 20px;
  display: flex;
  justify-content: space-around;
  align-items: center;
  width: 710px;
  height: 148px;
  background: #FFFFFF;
  border-radius: 20px;
  .easy{
    text-align: center;
    .imG{
      width: 44px;
      height: 44px;
    }
    .buy{
      font-size: 22px;
      font-weight: 400;
      line-height: 32px;
      color: #000000;
    }
  }
}
.choose{
  margin: 20px 20px 0;
  width: 710px;
  height: 704px;
  background: #FFFFFF;
  border-radius: 20px;
 .recommend{
  line-height: 44px;
  width: 710px;
  height: 80px;
  background: #38c4fb;
  border-radius: 20px 20px 0px 0px;
  padding: 20px;

    .mrecommend{
      display: block;
      line-height: 44px;
      font-size: 26px;
      font-weight: 600;
      color: #000000;
      &::after{
        width: 36px;
        height: 8px;
        color: #fb3838;
        display: block;
        border-radius: 10px;
      }
    }
    .gmrecommend{
      display: block;
      line-height: 44px;
      float: right;
      font-size: 20px;
      font-weight: 400;
      color: #737F97;
    }
  }
  .selected{
    .selectedBtn{
      font-size: 28px;
      font-weight: 500;
      line-height: 40px;
      color: #000000;
    }
    .more{
      font-size: 26px;
      font-weight: 400;
      line-height: 36px;
      color: #B1B1B1;
      float: right;
    }
  }
  .safe{
    font-size: 20px;
    font-weight: 400;
    line-height: 28px;
    color: #B1B1B1;
  }
  .cbox{
    display: flex;
    justify-content: space-evenly;
    margin: 26px 26px 24px 24px;
    .abox{
    .lease{
    .model{
      font-size: 26px;
      font-weight: 600;
      line-height: 36px;
      color: #000000;
    }
    .fValue{
      font-size: 36px;
      font-weight: 600;
      line-height: 50px;
      color: #3861FB;
    }
    .timeBtn{
      font-size: 22px;
      font-weight: 400;
      line-height: 32px;
      color: #B1B1B1;
    }
    .year{
      font-size: 30px;
      font-weight: 600;
      line-height: 42px;
      color: #000000;
    }
   }
  }
  }
}
}
</style>
