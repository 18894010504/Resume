<template>
  <div class="app" id="app">
    <div class="banner">
      <img class="banner-pic" :src="banner" alt="banner 图" />
      <div class="title">史雄伟在线简历</div>
    </div>
    <!-- 第一行 -->
    <el-row>
      <el-col :xs="24" :sm="24" :md="5" :lg="6" :xl="5" class="part">
        <router-view name="PartOne" />
      </el-col>
      <el-col :xs="24" :sm="24" :md="12" :lg="12" :xl="8" class="part">
        <router-view name="PartTwo" />
      </el-col>
      <el-col :xs="24" :sm="24" :md="7" :lg="6" :xl="11" class="part">
        <router-view name="PartThree" />
      </el-col>
    </el-row>
    <!-- 第二行 -->
    <el-row>
      <el-col :xs="24" :sm="24" :md="8" :lg="8" :xl="8" class="part">
        <router-view name="PartFour" />
      </el-col>
      <el-col :xs="24" :sm="24" :md="8" :lg="8" :xl="8" class="part">
        <router-view name="PartFive" />
      </el-col>
      <el-col :xs="24" :sm="24" :md="4" :lg="4" :xl="4" class="part">
        <router-view name="PartSix" />
      </el-col>
      <el-col :xs="24" :sm="24" :md="4" :lg="4" :xl="4" class="part">
        <router-view name="PartSeven" />
      </el-col>
    </el-row>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      banner: require("./assets/img/banner.png")
    };
  }
};
</script>

<style>
body {
  background: #011128;
  color: #fff;
}
.app {
  width: 100%;
}
.part {
  padding: 10px;
}
.banner {
  margin-bottom: 10px;
  border-bottom: 1px solid #034493;
}
.banner img {
  width: 100%;
  height: 60px;
}
.title {
  background-color: #034493;
  width: 20%;
  height: 60px;
  position: absolute;
  top: 0;
  left: 7%;
  line-height: 60px;
  font-size: 30px;
  text-align: center;
  letter-spacing: 2px;
}
</style>