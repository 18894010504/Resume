<template>
  <div :class="partSix">
    <h3 class="text-center">编程技能</h3>
    <p class="font-small">
      <span class="font-bold">前端：</span>HTML/HTML5、CSS/CSS3、JS/ES6、jQuery、Vue、React……
    </p>
    <p class="font-small">
      <span class="font-bold">工程化：</span>Gulp、Webpack
    </p>
    <p class="font-small">
      <span class="font-bold">后端：</span>Node、Java
    </p>
    <p class="font-small"></p>
    <p class="font-small">
      <span class="font-bold">版本控制：</span>Git、SVN
    </p>
    <p class="font-small">
      <span class="font-bold">其他：</span>MongoDB、MySQL
    </p>
  </div>
</template>

<script>
export default {
  name: "partSix",
  data() {
    return {
      partSix: "part-six",
      curWidth: 0
    };
  },
  beforeMount() {
    this.curWidth =
      document.documentElement.clientWidth || document.body.clientWidth;
    if (this.curWidth < 1600) {
      this.partSix = "part-six-responsive";
    }
  }
};
</script>

<style scoped>
.part-six {
  width: 100%;
  height: 310px;
  border: 40px solid transparent;
  border-image: url("~@/./assets/img/border_image.png") 30 30 stretch;
  background: #18202d;
}
.part-six-responsive {
  width: 100%;
  border: 35px solid transparent;
  border-image: url("~@/./assets/img/border_image.png") 30 30 stretch;
  background: #18202d;
}
.text-center {
  text-align: center;
}
.font-small {
  font-size: 0.9em;
}
.font-bold {
  font-weight: bold;
  color: deepskyblue;
}
</style>