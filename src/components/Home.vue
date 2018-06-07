<template>
  <!-- Video Area Started -->
  <main class="main_role" id="main_role"
        :style="this.$parent.$data.mix_data.slide_mover"
        @click="$parent.$options.methods.only_close">

    <div class="video_wrap" id="video_wrap">
      <div class="video_basket" id="video_basket">

        <!--
        <iframe type="text/html"
                src="https://www.youtube.com/embed/K0lL1HysGMc?&version=3&autoplay=1&loop=1&playlist=K0lL1HysGMc&showinfo=0&fs=0&disablekb=1&vq=auto&controls=0&rel=0&end=75"
                frameborder="0" volume="0" allowfullscreen webkitallowfullscreen mozallowfullscreen>
        </iframe>
        -->

        <iframe v-if="windowWidth > 750" class="video" id="video"
                src="https://player.vimeo.com/video/221257502?autoplay=1&loop=1&color=ffffff&background=1&title=0&byline=0&portrait=0&controls=0"
                width="100%" height="100%" frameborder="0" volume="0" webkitallowfullscreen mozallowfullscreen allowfullscreen>
        </iframe>

        <img v-else class="video_cover" src="../assets/pages/home/unsplash2.jpg" alt="Main Cover Image" />

      </div>
    </div>

    <!-- Main Context on video wrap -->
    <div class="main_title" >
      <h2>OPEN MIND</h2>
      <h3>우리는 개방적입니다</h3>
      <div class="division_bar"></div>
      <p>복층으로 이루어진 색다른 회사 공간에서</p>
      <p>우리는 서로의 의견을 자유롭게 이야기하고, 각 부서간 원활하게 소통하며 일합니다.</p>
      <div class="guide_to_scroll">
        <img class="down_img" src="../assets/common/down.png">
      </div>
    </div>

    <section class="section_1"><!--make ul list-->

      <div class="culture">Culture</div>

      <div class="culture_wrap">
        <div class="culture_img_wrap">
          <div class="culture_img">
            <ul>
              <li class="li_1"></li>
              <li class="li_2" style="background-color: darkblue"></li>
            </ul>
            <div class="img_nav">
              <button class="prev_button">
                <img src="../assets/pages/home/arrow_left.png" alt="Left button">
              </button>
              <button class="next_button">
                <img src="../assets/pages/home/arrow_right.png" alt="Right button">
              </button>
            </div>
            <div class="img_position">
              <p>1/10</p>
            </div>
          </div>
          <div class="img_border"></div>
        </div>
        <div class="culture_text">
          <div class="inner_title">
            <h4>RESPECT</h4>
            <p>우리는 존중합니다</p>
          </div>
          <div class="division_bar_small"></div>
          <div class="inner_content">
            <p>나이와 직급에 상관없이</p>
            <p>모두에게 존댓말과 높임말을 사용합니다.</p>
            <p>동등한 위치에서 자신의 생각을 말하지만,</p>
            <p>스스로가 내린 결정의 책임감을 가지고 일합니다.</p>
          </div>
        </div>
        <div class="side_text">
          <p>Have sense of responsibility</p>
        </div>
      </div>

    </section>
    <!--section 1-->

    <section class="section_2">

      <div class="culture_wrap">
        <div class="culture_img_wrap">
          <div class="culture_img">
            <ul>
              <li class="li_1"></li>
              <li class="li_2" style="background-color: darkcyan"></li>
            </ul>
            <div class="img_nav">
              <button class="prev_button">
                <img src="../assets/pages/home/arrow_left.png" alt="Left button">
              </button>
              <button class="next_button">
                <img src="../assets/pages/home/arrow_right.png" alt="Right button">
              </button>
            </div>
            <div class="img_position">
              <p>1/10</p>
            </div>
          </div>
          <div class="img_border"></div>
        </div>
        <div class="culture_text">
          <div class="inner_title">
            <h4>ENJOY</h4>
            <p>우리는 즐겁습니다</p>
          </div>
          <div class="division_bar_small"></div>
          <div class="inner_content">
            <p>날이 좋은 날에는,</p>
            <p>직원들과 함께 즉흥적으로 소풍을 떠납니다.</p>
            <p>벚꽃이 만개할 때는, 다같이 벚꽅놀이를 갑니다.</p>
            <p>연말에는 송년회를 열어</p>
            <p>한 해의 격려와 응원을 보내줍니다.</p>
          </div>
        </div>
        <div class="side_text">
          <p>Give encouragement to each other</p>
        </div>
      </div>

    </section>
    <!--section 2-->

    <section class="section_3">

      <div class="culture_wrap">
        <div class="culture_img_wrap">
          <div class="culture_img">
            <ul>
              <li class="li_1"></li>
              <li class="li_2"></li>
            </ul>
            <div class="img_nav">
              <button class="prev_button">
                <img src="../assets/pages/home/arrow_left.png" alt="Left button">
              </button>
              <button class="next_button">
                <img src="../assets/pages/home/arrow_right.png" alt="Right button">
              </button>
            </div>
            <div class="img_position">
              <p>1/10</p>
            </div>
          </div>
          <div class="img_border"></div>
        </div>
        <div class="culture_text">
          <div class="inner_title">
            <h4>FREEDOM</h4>
            <p>우리는 자유롭습니다</p>
          </div>
          <div class="division_bar_small"></div>
          <div class="inner_content">
            <p>공식 업무 시간은 오전 9시30분으로</p>
            <p>여유롭게 아침을 시작합니다.</p>
            <p>업무 중 피곤함이 몰려올 때는,</p>
            <p>잠깐의 티타임으로 에너지를 얻습니다.</p>
            <p>우리는 매년 하계 휴가를 통해</p>
            <p>재충전의 시간을 보냅니다.</p>
          </div>
        </div>
        <div class="side_text">
          <p>Have time of recharge</p>
        </div>
      </div>

    </section>
    <!--section 3-->

  </main>
</template>

<script>
  export default {
    name: "home",
    data: function() {
      return {
        windowWidth: window.innerWidth
      }
    },
    mounted() {
      let that = this;
      this.$nextTick(function() {
        window.addEventListener('resize', function(e) {
          that.windowWidth = window.innerWidth
        });
      });
    }
  }
</script>

<style lang="scss" scoped>
  /*
  ===============================================
    Main page, Video Start
  ===============================================
  */

  /* Video wrap -> Video basket -> Video(iFrame) */
  .video_wrap {
    position: absolute;
    width: 100%;
    height: 100vh;
    background: #000;
    top: 0; right: 0; bottom: 0; left: 0;
    overflow: hidden;
    z-index: 10;
  }

  .video_basket {
    position: relative;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    pointer-events: none;
    background-color: black;
    opacity: 0.4;
    z-index: 30;
  }

  .video {
    position: relative;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    pointer-events: none;
    z-index: 20;
  }

  .video_cover {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    z-index: 30;
    object-fit: cover;
  }

  /* Stretch Video */
  @media (min-aspect-ratio: 16/9) {
    .video_basket {
      height: 300%;
      top: -100%;
    }
  }/*=*/
  @media (max-aspect-ratio: 16/9) {
    .video_basket {
      width: 300%;
      left: -100%;
    }
  }/*=*/

  /*
  ===============================================
    Video End
  ===============================================
  */

  /* Main Text on Video */
  .main_title {
    position: relative;
    top: 0;
    left: 0;
    z-index: 500;
    width: 100%;
    height: 100vh;
    padding-top: calc(50vh - 65px);
    color: #fdfdfd;
    text-align: center;
    word-break: keep-all;
    white-space: pre-line;
    overflow: hidden;
    font-family: Impact, sans-serif;
    h2 {
      font-size: 55px;
      font-weight: bold;
      margin: 0;
    }
    h3 {
      font-family: 'NanumSquare', sans-serif;
      font-size: 30px;
      font-weight: normal;
      margin: 0;
    }
    .division_bar {
      width: 70px;
      height: 3px;
      background-color: #fdfdfd;
      margin: 12px auto 20px;
    }
    p {
      font-family: 'NanumSquare', sans-serif;
      font-size: 16px;
    }
  }/* Main title area end */

  /* Change Text size belongs to Web width */
  @media (max-width: 650px) {
    .main_title {
      h2 {
        font-size: 40px;
      }
      h3 {
        font-size: 25px;
      }
      p {
        font-size: 14px;
      }
    }
  }/*=*/

  /* Section Part */

  .section_1, .section_2, .section_3 {
    width: 100%;
    padding: 50px 0;
    background-color: #ffffff;
    text-align: center;
    color: #515151;
    font-family: Impact, sans-serif;
  }

  .culture {
    width: 100px;
    height: 25px;
    line-height: 25px;
    font-weight: bold;
    color: #fefefe;
    background-color: darkblue;
    margin: 0 auto 40px;
  }

  .culture_wrap {
    width: 100%;
    max-width: 1200px;
    padding: 0 20px;
    margin: 0 auto;
    text-align: center;
    &:after {
      content: '';
      clear: both;
      display: block;
    }
  }

  .culture_img_wrap {
    width: 60%;
    text-align: center;
    float: left;
    &:after {
      content: '';
      clear: both;
      display: block;
    }
    .culture_img {
      position: relative;
      width: 85%;
      height: 0;
      padding-bottom: 83%;
      border-radius: 120%;
      overflow: hidden;
      float: left;
      z-index: 400;
      border: 8px solid #d60c47;
      ul {
        width: 100%;
        padding-bottom: 100%;
        background-color: #ffffff;
        li {
          position: absolute;
          top: 0;
          width: 100%;
          height: 100%;
          background-color: azure;
        }
      }
      .img_nav {
        position: absolute;
        width: 100%;
        height: 0;
        padding: 0 25px;
        top: calc(50% - 15px);
        &:after {
          content: '';
          clear: both;
          display: block;
        }
        .prev_button, .next_button {
          width: 40px;
          height: 40px;
          background-color: #f0f0f0;
          border: 3px solid #ffffff;
          border-radius: 100%;
          opacity: 0.5;
          img {
            width: 100%;
            height: 100%;
            transform: scale(0.8);
          }
          &:focus {
            outline: none;
          }
          &:hover {
            opacity: 1;
          }
        }
        .prev_button {
          float: left;
        }
        .next_button {
          float: right;
        }
      }
      .img_position {
        position: absolute;
        width: 100%;
        height: 30px;
        bottom: 5px;
        text-align: center;
        p {
          width: 60px;
          height: 30px;
          margin: 0 auto;
          line-height: 30px;
          font-size: 25px;
          color: #fefefe;
          background-color: rgba(50, 50, 50, 0.5);
          border-radius: 10px;
        }
      }
    }
    .img_border {
      position: relative;
      width: 50%;
      padding-bottom: 50%;
      border-radius: 120%;
      background-image: linear-gradient(
          135deg, #002778 25%, #ffffff 25%, #ffffff 50%, #002778 50%, #002778 75%, #ffffff 75%, #ffffff 100%
      );
      background-size: 20px 20px;
      right: -48%;
      margin-top: 38%;
      z-index: 300;
    }
  }

  .culture_text {
    width: 35%;
    float: left;
    text-align: left;
    padding-left: 2%;
    .inner_title {
      h4 {
        font-size: 55px;
        font-weight: bold;
        margin: 38px 0 3px;
        color: #d60c47;
      }
      p {
        font-family: 'NanumSquare', sans-serif;
        font-size: 23px;
        padding: 0 2px;
      }
    }
    .division_bar_small {
      width: 50px;
      height: 2px;
      background-color: #212121;
      margin: 8px 4px 15px;
    }
    .inner_content {
      p {
        font-family: 'NanumSquare', sans-serif;
        font-size: 14px;
      }
    }
  }

  .side_text {
    width: 5%;
    float: left;
    font-size: 34px;
    font-weight: bold;
    padding-top: 45px;
    color: #000;
    p {
      transform: rotate(90deg);
      word-break: keep-all;
      white-space: nowrap;
    }
  }
  /* section 1 end */

  .section_2 {
    .culture_wrap {
      &:after {
        content: '';
        clear: both;
        display: block;
      }
      .culture_img_wrap {
        float: right;
        .culture_img {
          float: right;
          border: 8px solid #002778;
        }
        .img_border {
          background-image: linear-gradient(
              45deg, #d60c47 25%, #ffffff 25%, #ffffff 50%, #d60c47 50%, #d60c47 75%, #ffffff 75%, #ffffff 100%
          );
          right: 0;
        }
      }
      .culture_text {
        float: right;
        .inner_title {
          h4 {
            color: #002778;
          }
        }
      }
      .side_text {
        float: right;
      }
    }
  }/* section 2 end */


  .section_3 {

  }/* Section 3 ended */


  /*
  ===============================================
  Media query
  ===============================================
  */
  @media (max-width: 835px) {
    .culture_img_wrap {
      width: 100%;
    }
    .culture_text {
      width: 100%;
    }
    .side_text {
      display: none;
    }
  }


</style>
