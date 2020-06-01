<template>
  <div class="part-one">
    <img class="part-one-image" :src="headImage" alt="头像" />
    <p>姓&emsp;&emsp;名：史雄伟</p>
    <p>学&emsp;&emsp;历：本科</p>
    <p>工作年限：2 年</p>
    <p>年&emsp;&emsp;龄：26</p>
    <p>联系电话：17797592890</p>
    <p>电子邮箱：1109866370@qq.com</p>
    <p>微&emsp;&emsp;信：SXW88O</p>
    <p>
      GitHub：
      <a href="https://github.com/18894010504" target="_blank">18894010504</a>
    </p>
  </div>
</template>

<script>
export default {
  name: "partOne",
  data() {
    return {
      headImage: require("../assets/img/sxw.jpg")
    };
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
p {
  line-height: 30px;
}
.part-one {
  width: 100%;
  height: 500px;
  border: 40px solid transparent;
  border-image: url("~@/./assets/img/border_image.png") 30 30 stretch;
  background: #18202d;
  padding-left: 10px;
}
.part-one-image {
  width: 110px;
  margin: 0 0 10px 20px;
}
</style>