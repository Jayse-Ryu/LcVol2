<template>
  <div class="main_role" id="main_role"
       :style="this.$parent.$data.mix_data.slide_mover"
       @click="$parent.$options.methods.only_close">

    <input type="hidden" v-bind:value="where_am_i = 7">

    <img class="main_image" src="../assets/pages/recruit/recruit.jpg" alt="page background image">

    <section class="section_0">
      <h2 class="section_0_title">
        <p>엘씨벤처스에 지원해주세요.</p>
      </h2>
    </section>

    <section class="section_1">

      <div class="test_img_wrap">

        <ul class="img_box">
          <li class="img_1" style="background-color: slateblue"></li>
          <li class="img_2" style="background-color: darkblue"></li>
          <li class="img_3" style="background-color: darkkhaki"></li>
        </ul>

        <ul class="img_nav">
          <li class="prev"><</li>
          <li class="next">></li>
        </ul>

      </div>

    </section>

  </div>
</template>

<script>
  export default {
    name: "recruit"
  }
</script>

<style lang="scss" scoped>
  .section_1 {
    display: block;
    perspective: 1000px;
  }

  .test_img_wrap {
    position: relative;
    background-color: #fff;
    perspective: 1000px;
  }

  .img_box {
    position: relative;
    z-index: 40;
    display: block;
    width: 200px;
    height: 200px;
    li {
      position: absolute;
      display: block;
      width: 200px;
      height: 200px;
      top: 0;
      left: 0;
      float: left;
      border-radius: 500px;
      transform-origin: 10px -10px;
      z-index: 400;
      transition: all ease 2s;
      &:hover {
        transform: rotateY(-90deg);
      }
    }
    &:after {
      clear: both;
      display: block;
      content: '';
    }
  }

  .img_nav {
    position: relative;
    top: -120px;
    z-index: 50;
    width: 200px;
    .prev, .next {
      display: block;
      width: 50px;
      height: 50px;
      float: left;
      font-size: 35px;
      line-height: 50px;
      text-align: center;
    }
    .next {
      float: right;
    }
    &:after {
      display: block;
      content: '';
      clear: both;
    }
  }





</style>
