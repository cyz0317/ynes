<template>
  <div id="app">
    <div class="top">
      <div class="head">
        <div class="head-1">
          <img src="./assets/shuslogo.png" alt="" />
          <div class="topright">
            <span class="trs-1">首页</span>
            <span class="trs-2">招聘信息</span>
            <span class="trs-2">关于我们</span>
          </div>
        </div>
      </div>
      <span class="trs-3">企业数字化转型最佳 技术合作伙伴！ </span>
      <span class="trs-4"
        >致力于成为企业数字化转型的最佳长期技术伙伴，
        为企业建设数字化经营操作系统</span
      >
      <div class="xuanfu">
        <div class="xuanfu-1">
          <img src="./assets/xuanfu.png" alt="" />
          <div class="suss">
            <span class="xuanfu-3">数势科技</span>
            <span class="suss-2">愿景：</span>
            <span class="xuanfu-2">
              成为企业建设数字化经营操作系统的最佳长期技术伙伴，推动企业数字化转型，创造新的增长动力，实现数据价值普惠化
            </span>
            <span class="suss-2">使命：</span>
            <span class="xuanfu-2"
              >为客户数字化经营提供更易用、更高效的技术服务</span
            >
            <span class="xuanfu-4"></span>
          </div>
        </div>
      </div>
    </div>
    <div class="mid-1">
      <div class="mid-11">
        <div class="mid-111">
          <img src="./assets/advantages/advantagelogo.png" alt="" />
          <span class="mid-1111">我们的优势</span>
        </div>
        <img src="./assets/advantages/advantage10.png" alt="" class="midimg1" />
      </div>
      <div class="mid-12">
        <div
          class="mid-121"
          v-for="ad in advantages"
          :key="ad.index"
          :style="{ backgroundImage: 'url(' + ad.pic + ')' }"
        >
          <span class="mid-1211" :class="ad.sty">{{ ad.title }}</span>
          <span class="mid-1212">{{ ad.content }}</span>
        </div>
      </div>
      <img src="./assets/advantages/advantage9.png" alt="" class="midimg2" />
    </div>
    <div class="mid-2">
      <div class="mid-21">
        <div class="mid-211">
          <img src="./assets/corevalue1.png" alt="" />
          <span class="mid-212">给客户带来的核心价值</span>
        </div>
      </div>
      <div class="mid-22">
        <div class="corevaldiv" v-for="cd in corevaldiv" :key="cd.index">
          <img :src="cd.pic" alt="" />
          <span class="corevaldivfs">{{ cd.title }}</span>
          <span class="corevaldivss"></span>
          <span class="corevaldivts">{{ cd.content }}</span>
        </div>
      </div>
    </div>
    <div class="mid-3">
      <div class="midtf">
        <div class="midtftop">
          <div class="midtff">
            <img src="./assets/digitizationpic1.png" alt="" />
            <span class="midtff-1">数字化技术服务</span>
          </div>
        </div>
        <div class="midtfbottom">
          <div class="midtfl">
            <div class="midtfl-1">
              <div>
                <span class="midtfl-3"> </span>
                <span class="midtfl-2">数字化经营解决方案</span>
              </div>
              <div
                v-for="dz in digitization"
                :key="dz.index"
                class="middleground"
              >
                <img :src="dz.pic" alt="" class="icon5" />
                <span class="midts-21">
                  <span class="suss-2">{{ dz.title }}</span>
                  <span class="suss-3">{{ dz.content }}</span>
                </span>
              </div>
            </div>
          </div>
          <div class="midtfr"></div>
        </div>
      </div>
      <div class="midts">
        <div class="midts-1"></div>
        <div class="midts-2">
          <div>
            <span class="midtstf"> </span>
            <span class="midtsts">数据中台建设</span>
          </div>
          <div v-for="md in middleground" :key="md.index" class="middleground">
            <img :src="md.pic" alt="" class="icon5" />
            <span class="midts-21">
              <span class="suss-2">{{ md.title }}</span>
              <span class="suss-3">{{ md.content }}</span>
            </span>
          </div>
        </div>
      </div>
    </div>
    <div class="bottom">
      <div class="bottom-1">
        <div class="bottom-3">
          <span class="bts">
            <img src="./assets/shuslogo1.png" alt="" />
          </span>
          <div class="bottom-5">
            <div class="bfs">联系我们</div>
            <span>联系方式:157846732117</span>
            <span>合作邮箱:XXXXXXX@XX.com</span>
            <span>地址：北京市海淀区知春路3号致真大厦A座805</span>
          </div>
        </div>
        <div class="bottom-4"></div>
      </div>
      <div class="bottom-2">Copyright © 2019-2020 DigitForce.com 版权所有</div>
    </div>
  </div>
</template>

<style>
@import "assets/styles/font.css";
#app {
  /* width:1920px; */
  width: 1920px;
  height: auto;
  background: rgba(255, 255, 255, 1);
  letter-spacing: 0.8px;
}
.topright {
  width: 1290px;
  display: flex;
  justify-content: flex-end;
}
.topright span {
  text-align: center;
  height: 78px;
  line-height: 81px;
  display: inline-block;
  font-size: 20px;
  font-family: ssc;
}
.trs-1 {
  display: inline-block;
  cursor: pointer;
  width: 70px;
  border-bottom: 3px solid #48f9c8;
}
.trs-1:hover {
  color: aqua;
}
.trs-2 {
  display: inline-block;
  width: 148px;
}
.trs-3 {
  display: inline-block;
  width: 576px;
  height: 137px;
  font-size: 60px;
  position: absolute;
  top: 287px;
  left: 228px;
  font-family: "digital";
}
.trs-4 {
  display: inline-block;
  position: absolute;
  top: 484px;
  left: 231px;
  width: 596px;
  height: 69px;
  font-size: 26px;
  font-family: "ssc";
}
.xuanfu-2 {
  width: 818px;
  height: auto;
  font-size: 20px;
  font-family: digital;
  font-weight: 400;
  color: rgba(51, 51, 57, 1);
  line-height: 30px;
  opacity: 0.7;
  margin-bottom: 20px;
}
.xuanfu-3 {
  width: 142px;
  height: 38px;
  font-size: 34px;
  font-family: PingFang-SC-Semibold;
  font-weight: 600;
  color: rgba(0, 5, 20, 1);
  line-height: 48px;
  margin-bottom: 30px;
}
.suss {
  height: auto;
  width: 924px;
  padding-left: 49px;
  padding-top: 15px;
  display: flex;
  flex-direction: column;
}
.suss span {
  display: inline-block;
}
.suss-1 {
  font-size: 34px;
  color: #000514;
  line-height: 48px;
  font-family: PingFang-SC-Semibold;
  font-weight: 600;
  letter-spacing: 80;
}
.suss-2 {
  font-size: 24px;
  color: #333339;
  letter-spacing: 80;
  font-family: Medium;
  line-height: 48px;
  /* font-weight: 600; */
}
.suss-3 {
  color: #333339;
  font-size: 16px;
  letter-spacing: 80;
  line-height: 30px;
  font-weight: 300;
  display: inline-block;
  width: 620px;
  height: auto;
}
.top {
  width: 1920px;
  height: 910px;
  color: #ffffff;
  background: url("assets/top.png") no-repeat;
}
.head {
  width: 1920px;
  height: 81px;
  border-bottom: solid 1px #ffffff;
  color: #ffffff;
}
.head-1 {
  width: 1470px;
  height: 81px;
  margin: auto auto;
  display: flex;
  justify-content: space-between;
}
.head-1 img {
  width: 174px;
  height: 52px;
  display: inline-block;
  margin-top: 14px;
}
.bottom {
  width: 1920px;
  height: 388px;
  background: url("assets/bottom.png") no-repeat;
}
.bottom-1 {
  width: 1200px;
  height: 273px;
  margin: auto auto;
}
.bottom-2 {
  /* width:373px; */
  height: 16px;
  font-size: 14px;
  font-family: ssc;
  font-weight: 300;
  color: rgba(255, 255, 255, 1);
  line-height: 11px;
  position: relative;
  left: 360px;
  bottom: -30px;
  /* letter-spacing:0.1em; */
}
.bottom-3 {
  display: flex;
  height: 145px;
  width: 1200px;
  position: relative;
  top: 87px;
}
.bts {
  height: 145px;
  width: 269px;
  display: inline-block;
}
.bts img {
  width: 202px;
  height: 61.9px;
  margin-top: 47px;
}
.bottom-5 {
  display: flex;
  flex-direction: column;
  border-left: rgba(255, 255, 255, 1) 1px solid;
  height: 145px;
  width: 931px;
}
.bottom-5 span {
  margin-left: 59px;
  padding-bottom: 10px;
  font-size: 14px;
  font-family: ssc;
  font-weight: 300;
  color: rgba(255, 255, 255, 1);
}
.bfs {
  margin-left: 59px;
  font-size: 20px;
  margin-bottom: 30px;
  font-weight: bold;
  color: rgba(255, 255, 255, 1);
}
.bottom-4 {
  width: 1200px;
  height: 1px;
  background: linear-gradient(
    90deg,
    rgba(60, 140, 255, 1) 0%,
    rgba(0, 255, 255, 1) 100%
  );
  opacity: 0.6;
  position: relative;
  top: 130px;
}
.xuanfu {
  width: 1618px;
  height: 656px;
  background: url("assets/suspension.png") no-repeat;
  margin-top: 676px;
  margin-left: 150px;
}
.xuanfu-1 {
  display: flex;
  height: 396px;
  width: 1492px;
  margin-left: 126px;
  padding-top: 117px;
}
.xuanfu-4 {
  width: 148px;
  height: 8px;
  background: #0069ff;
  margin-top: 30px;
}
.mid-1 {
  width: 1920px;
  height: 1812px;
}
.mid-11 {
  width: 1920px;
  height: 786px;
}
.midimg1 {
  margin-top: -80px;
  margin-left: 1614px;
}
.midimg2 {
  margin-top: 31px;
  margin-left: 35px;
}
.mid-111 {
  display: flex;
  width: 362px;
  height: 104px;
  padding-top: 605px;
  margin: auto;
}
.mid-1111 {
  display: inline-block;
  width: 252px;
  height: 45px;
  font-size: 48px;
  font-family: PingFang-SC-Semibold;
  font-weight: 600;
  color: rgba(51, 51, 51, 1);
  line-height: 90px;
}
.mid-12 {
  display: flex;
  flex-wrap: wrap;
  margin: auto auto;
  width: 1300px;
  height: 847px;
}
.mid-121 {
  display: flex;
  flex-direction: column;
  width: 298px;
  height: 412px;
  margin-right: 13px;
}
.mid-1211 {
  display: inline-block;
  /* width:132px;
  height:23px; */
  font-size: 24px;
  font-family: PingFang-SC-Semibold;
  font-weight: 600;
  color: rgba(255, 255, 255, 1);
  line-height: 48px;
  margin-top: 86px;
}
.you1 {
  width: 132px;
  height: 23px;
  margin-left: 75px;
}
.you2 {
  width: 105px;
  height: 23px;
  margin-left: 84px;
}
.you3 {
  width: 178px;
  height: 51px;
  margin-left: 53px;
}
.you4 {
  width: 104px;
  height: 23px;
  margin-left: 86px;
}
.you5 {
  width: 242px;
  height: 23px;
  margin-left: 21px;
}
.you6 {
  width: 159px;
  height: 23px;
  margin-left: 67px;
}
.you7 {
  width: 215px;
  height: 23px;
  margin-left: 34px;
}
.mid-1212 {
  width: 192px;
  height: 90px;
  font-size: 18px;
  font-family: PingFang SC;
  font-weight: 400;
  color: rgba(255, 255, 255, 1);
  line-height: 30px;
  margin-top: 67px;
  margin-left: 50px;
}
.mid-2 {
  width: 1920px;
  height: 944px;
  background: url("assets/mid2bgpic.png") no-repeat;
}
.mid-21 {
  width: 1920px;
  height: 313px;
}
.mid-211 {
  margin: auto;
  width: 620px;
  height: 104px;
  padding-top: 132px;
  display: flex;
}
.mid-212 {
  display: inline-block;
  width: 511px;
  height: 46px;
  font-size: 48px;
  font-family: PingFang-SC-Semibold;
  font-weight: 600;
  color: rgba(51, 51, 51, 1);
  line-height: 1.8;
}
.mid-22 {
  display: flex;
  width: 1243px;
  height: 631px;
  margin: auto;
  justify-content: space-between;
}
.corevaldiv {
  display: flex;
  flex-direction: column;
  width: 353px;
  height: 491px;
  background: rgba(255, 255, 255, 1);
  box-shadow: 0px 24px 38px 0px rgba(0, 3, 12, 0.08);
  border-radius: 10px;
  padding-left: 41px;
}
.corevaldiv img {
  height: 64px;
  width: 58px;
  margin-top: 48px;
}
.corevaldivfs {
  display: inline-block;
  width: 148px;
  height: 36px;
  font-size: 28px;
  font-family: PingFang-SC-Semibold;
  font-weight: 600;
  color: rgba(51, 51, 51, 1);
  line-height: 48px;
  margin-top: 28px;
}
.corevaldivss {
  width: 55px;
  height: 4px;
  background: rgba(0, 211, 255, 1);
  margin-top: 20px;
}
.corevaldivts {
  width: 309px;
  height: 196px;
  font-size: 16px;
  font-family: digital;
  font-weight: 400;
  color: rgba(51, 51, 51, 1);
  line-height: 30px;
  margin-top: 55px;
}
.mid-3 {
  width: 1920px;
  height: 1940px;
}
.midtf {
  width: 1920px;
  height: 910px;
}
.midtftop {
  height: 352px;
  width: 1920px;
}
.midtfbottom {
  width: 1272px;
  height: auto;
  display: flex;
  margin-left: 342px;
}
.midtff {
  margin: auto;
  width: 453px;
  height: 104px;
  padding-top: 172px;
  display: flex;
}
.midtff-1 {
  display: inline-block;
  width: 357px;
  height: 46px;
  font-size: 48px;
  font-family: PingFang-SC-Semibold;
  font-weight: 600;
  color: rgba(51, 51, 51, 1);
  line-height: 1.8;
}
.midtfl {
  width: 680px;
  height: 600px;
}
.midtfl-1 {
  width: 706px;
  height: 600px;
  display: flex;
  flex-direction: column;
}
.midtfl-1 div {
  display: flex;
  width: 706px;
  height: 100px;
}
.midtfl-2 {
  width: 306px;
  height: 31px;
  font-size: 32px;
  font-family: PingFang SC;
  font-weight: 600;
  color: rgba(23, 217, 237, 1);
  line-height: 48px;
  margin-left: 37px;
}
.midtfl-3 {
  width: 6px;
  height: 48px;
  background: rgba(0, 211, 255, 1);
}
.midtfr {
  margin-top: 90px;
  width: 572px;
  height: 572px;
  background: url("assets/digitizationpic2.png") no-repeat;
}
.midts {
  width: 1920px;
  height: 1027px;
  background: url("assets/mid3bgpic.png") no-repeat;
  display: flex;
}
.midts-1 {
  margin-left: 276px;
  width: 570px;
  height: 430px;
  background: url("assets/midts-1.png") no-repeat;
  margin-top: 339px;
  margin-right: 30px;
}
.midts-2 {
  width: 706px;
  height: 500px;
  margin-top: 287px;
  display: flex;
  flex-direction: column;
}
.midts-2 div {
  display: flex;
  width: 706px;
  height: 100px;
}
.midtstf {
  display: inline-block;
  width: 6px;
  height: 48px;
  background: rgba(25, 121, 254, 1);
}
.midtsts {
  display: inline-block;
  width: 203px;
  height: 48px;
  font-size: 32px;
  font-family: PingFang-SC-Semibold;
  font-weight: 600;
  color: rgba(0, 97, 235, 1);
  line-height: 48px;
  margin-left: 40px;
}
.icon5 {
  display: inline-block;
  height: 46px;
  width: 46px;
  margin-right: 19px;
  margin-top: 10px;
}
.middleground {
  margin-top: 20px;
  position: relative;
  right: 20px;
}
.midts-21 {
  display: flex;
  flex-direction: column;
}
</style>
<script>
export default {
  name: "app",
  data() {
    return {
      middleground: [
        {
          pic: require("./assets/icon5.png"),
          title: "数据资产管理解决方案",
          content:
            "一站式数据资产管理解决方案，建立统一高效的数据采、存、算、汇、管、用机制"
        },
        {
          pic: require("./assets/icon6.png"),
          title: "数据可视化解决方案",
          content:
            "一站式数据可视化解决方案，统一数据指标口径，提供场景化和自助式的配置模板，满足业务多场景的看数和分析需求，小时级完成个性化报表"
        },
        {
          pic: require("./assets/icon7.png"),
          title: "数据BI建模解决方案",
          content:
            "规一站式、智能化的建模平台，数仓全局规划、数据接入、规范管理、模型构建、模型服务的全流程建模能力"
        },
        {
          pic: require("./assets/icon8.png"),
          title: "数据标签建模解决方案",
          content:
            "配置化的标签生产工具，业务人员无需开发能力即可生成个性化的标签以满足快速变化的业务需求"
        }
      ],
      digitization: [
        {
          pic: require("./assets/icon1.png"),
          title: "全场景用户运营平台",
          content:
            "统一会员管理，根据会员画像，通过客户全生命周期的触达与权益管理，提升顾客忠诚度、复购率与生命周期价值"
        },
        {
          pic: require("./assets/icon2.png"),
          title: "全渠道精准营销",
          content:
            "覆盖线上线下营销的全程触点，针对目标群体精准投放，通过实时监控、漏斗分析、AB测试等方式实现自动化精准营销"
        },
        {
          pic: require("./assets/icon3.png"),
          title: "全流程业务智能",
          content:
            "业务经营全程触点，通过数据清洗、加工形成整合化的数字经营资产，为业务的全流程从产品开发、选品决策、销售客服等服务，以可视化的实时BI指导业务作战"
        },
        {
          pic: require("./assets/icon4.png"),
          title: "全域业务中台",
          content:
            "提供线上线下全域交易能力，实现线上线下交易互通、库存共享、权益一致，打通不同场景和不同业务域的统一交易能力（商品通/订单通/库存通/会员通/营销通/权益通/支付通/服务通）"
        }
      ],
      corevaldiv: [
        {
          pic: require("./assets/corevalue2.png"),
          title: "数据资产化",
          content:
            "通过数据集成的能力（Auto Modeling，Work Dispatch， Monitor&Control，Data Assembling），打通客户散落于各系统的数据，辅助客户建立从数据采集到融合应用的标准流程，并基于业务逻辑建立标准统一的数据资源模型体系 - 实现数据资源标准化、资产化"
        },
        {
          pic: require("./assets/corevalue3.png"),
          title: "数据可视化",
          content:
            "通过商业智能分析工具（Data Max, Mobile Analysis, BI），为客户提供快捷好用的数据看板和数据分析服务， 数据口径指标统一，数据top-down & bottom-up可视化分析 - 实现数据分析实时可视化、智能化"
        },
        {
          pic: require("./assets/corevalue4.png"),
          title: "数字化经营",
          content:
            "通过数据建模、数据开发和算法应用平台，在研发-生产-营销-销售-用户运营等环节，为客户提供多维度的数据平台产品和服务（例如数字化用户运营），并直接对接客户的前端业务应用系统 - 搭建数字化经营操作系统，实现业务经营的数据驱动"
        }
      ],
      advantages: [
        {
          sty: "you1",
          pic: require("./assets/advantages/advantage1.png"),
          title: "成熟的技术",
          content: "经过618、双11海量流量考验的技术系统能力"
        },
        {
          sty: "you2",
          pic: require("./assets/advantages/advantage2.png"),
          title: "共创共建",
          content: "与客户技术团队深度协作，开放共创，授之以渔"
        },
        {
          sty: "you3",
          pic: require("./assets/advantages/advantage3.png"),
          title: "科技+零售行业 Know-how",
          content: "深耕大消费大零售，行业领先的线上线下全渠道运营经验"
        },
        {
          sty: "you4",
          pic: require("./assets/advantages/advantage4.png"),
          title: "简单易用",
          content: "智能易用的产品和技术平台，提供一站式服务"
        },
        {
          sty: "you5",
          pic: require("./assets/advantages/advantage5.png"),
          title: "数字化转型实战经验",
          content: "深耕大消费大零售，行业领先的线上线下全渠道运营经验"
        },
        {
          sty: "you6",
          pic: require("./assets/advantages/advantage6.png"),
          title: "成功案例众多",
          content: "对内服务3k采销，对内对外赋能多个零售客户，收效显著"
        },
        {
          sty: "you7",
          pic: require("./assets/advantages/advantage7.png"),
          title: "专业且敬业的团队",
          content: "核心团队均来自京东/百度/阿里/微软/华为等顶级技术团队"
        },
        {
          sty: "you1",
          pic: require("./assets/advantages/advantage8.png"),
          title: "",
          content: ""
        }
      ]
    };
  }
};
</script>
