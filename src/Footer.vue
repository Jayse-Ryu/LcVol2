<template>
  <footer class="footer"
          :style="this.$parent.$data.mix_data.slide_mover"
          @click="$parent.$options.methods.only_close">
    <div class="footer_wrap"><!--for make without padding-->

      <div class="logo_tap">
        <div class="footer_logo">
          LC Ventures
        </div>
      </div>

      <div class="info_tap">
        <ul>
          <li>법인명: (주)엘씨벤처스 | 대표자명: 권용무 | 사업자등록번호: 220-88-91971</li>
          <li>사업장 소재지 주소: 서울 성동구 뚝섬로 1길 25 한라에코밸리 206호</li>
          <li>회사전화: 070-8855-8390 | E-mail: biz@lcventures.co.kr</li>
        </ul>
      </div>

    </div><!--Footer wrap-->

  </footer>
</template>

<script>
  export default {
    name: "app-footer"
  }
</script>

<style lang="scss" scoped>
  .footer {
    position: relative;
    width: 100%;
    padding: 30px 0;
    background-color: #efefef;
    transition: all 350ms cubic-bezier(.83,.01,.46,.86);

    .footer_wrap {
      text-align: center;
      .logo_tap {
        display: inline-block;
        margin: 0;
        vertical-align: top;
        .footer_logo {
          font-family: Impact, sans-serif;
          font-size: 35px;
          font-weight: bold;
          padding: 0 30px;
        }
      }

      .info_tap {
        display: inline-block;
        margin: 0;
        vertical-align: top;
        font-family: 'NanumSquare', Impact, sans-serif;
        font-size: 14px;
        color: #212121;
        text-align: left;
      }
    }/* Footer wrap */

  }/*Footer*/


  /*
  ===============================================
  Media query
  ===============================================
  */
  @media (max-width: 650px) {
    .footer{
      .footer_wrap {
        .logo_tap {
          display: block;
        }

        .info_tap {
          display: block;
          margin-top: 10px;
          font-size: 12px;
          text-align: center;
        }
      }
    }
  }
</style>
