<template>
  <div class="dingdan-main">
    <div class="dingdan-pane">
      <div class="dingdan-name">购买者：{{ everyone.name }}</div>
      <div class="dingdan-tele">联系方式：{{ everyone.tele }}</div>
      <div class="dingdan-ttype">门票类型：{{ everyone.ttype }}</div>
      <div class="dingdan-num">门票张数：{{ everyone.num }}张</div>
      <div class="dingdan-money">门票价格：{{ everyone.money }}</div>
    </div>
  </div>
</template>

<script>
  export default {
    name: "dingdan",
    props: {
      everyone: {
        type: Object,
        default: () => ({})
      }
    }
  };
</script>

<style scoped>
  .dingdan-main {
    margin-bottom: 25px;
  }
  .dingdan-pane {
    margin: 10px;
    margin-left: 30px;
    height: 80px;
    border: 3px solid slategray;
    border-radius: 8px;
    font-family: "YouYuan", "KaiTi";
  }
  .dingdan-name {
    float: left;
    position: absolute;
    margin-left: 40px;
    font-size: 18px;
  }
  .dingdan-tele {
    float: right;
    position: absolute;
    margin-left: 360px;
    font-size: 18px;
  }
  .dingdan-ttype {
    float: right;
    position: absolute;
    margin-top: 40px;
    margin-left: 40px;
    font-size: 18px;
  }
  .dingdan-num {
    float: left;
    position: absolute;
    margin-left: 250px;
    margin-top: 40px;
    font-size: 18px;
  }
  .dingdan-money {
    float: left;
    position: absolute;
    margin-left: 400px;
    margin-top: 40px;
    font-size: 18px;
  }
</style>
