<template>
  <div :class="partFive">
    <h3 class="text-center text-top">工作履历</h3>
    <p>
      <a href="javascript:void(0)">万桥信息技术有限公司</a>
      <span class="text-small">| 2018/08 - 2019/12</span>
    </p>
    <p class="text-small">工作内容：日常操作 jQuery 编写活动页、BPM/IBMS系统、Vue + ECharts + Element 报表制作……</p>
    <p class="text-small">项目成就：</p>
    <p class="text-small">
      &emsp;1. 白银旅游移动端。使用Vue + jQueryWeUI相关技术，代码已完成，项目已上线。
      <a
        href="http://wwzhly.travel189.com:9000/bywx/by/index"
        target="_black"
      >项目地址</a>
    </p>
    <p class="text-small">
      &emsp;2. 智游崆峒网。使用jQuery + Bootstrap相关技术，代码已完成，项目已上线。
      <a
        href="http://www.kongtongtour.com/"
        target="_black"
      >项目地址</a>
    </p>
    <p class="text-small">
      &emsp;3. 甘肃省文化产业发展专项资金信息管理平台。使用jQueryMiUI + JSAAS相关技术，代码已完成，项目已上线。
      <a
        href="http://60.165.122.144:9999/login.jsp"
        target="_black"
      >项目地址</a>
    </p>
  </div>
</template>

<script>
export default {
  name: "partFive",
  data() {
    return {
      partFive: "part-five",
      curWidth: 0
    };
  },
  beforeMount() {
    this.curWidth =
      document.documentElement.clientWidth || document.body.clientWidth;
    if (this.curWidth < 1600) {
      this.partFive = "part-five-responsive";
    }
  }
};
</script>

<style scoped>
a {
  color: deepskyblue;
}
a:hover {
  color: rgb(118, 190, 248);
}
.part-five {
  width: 100%;
  height: 310px;
  border: 40px solid transparent;
  border-image: url("~@/./assets/img/border_image.png") 30 30 stretch;
  background: #18202d;
}
.part-five-responsive {
  width: 100%;
  border: 16px solid transparent;
  border-image: url("~@/./assets/img/border_image.png") 30 30 stretch;
  background: #18202d;
}
.text-center {
  text-align: center;
}
.text-small {
  font-size: 0.9em;
  color: rgb(253, 239, 239);
}
</style>