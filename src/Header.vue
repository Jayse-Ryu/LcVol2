<template>
  <!-- Header + Top Buttons -->
  <header class="header"
          :style="this.$parent.$data.mix_data.slide_mover" id="header">

    <!-- Logo Area -->
    <div class="head_logo">
      <router-link class="head_logo_inner" to="/">LC Ventures</router-link>
    </div>

    <!-- Top Buttons (Simple nav button) -->
    <div v-if="windowWidth > 650" class="middle_menu">
      <div class="button_middle" @click="$parent.$options.methods.navi_delay">
        <router-link class="button_middle_inner"  to="/recruit">RECRUIT</router-link>
      </div>
      <div class="button_middle" @click="$parent.$options.methods.navi_delay">
        <router-link class="button_middle_inner"  to="/people">PEOPLE</router-link>
      </div>
      <div class="button_middle" @click="$parent.$options.methods.navi_delay">
        <router-link class="button_middle_inner"  to="/projects">PROJECT</router-link>
      </div>
      <div class="button_middle" @click="$parent.$options.methods.navi_delay">
        <router-link class="button_middle_inner" to="/about">COMPANY</router-link>
      </div>
    </div>
    <!--Top button - middle menu-->

    <!-- Hamburger Menu Button -->
    <div v-else class="button_menu" id="button_menu" @click="$parent.$options.methods.slide_nav"></div>

  </header>
</template>

<script>
  export default {
    name: "app-header",
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
  }/*export*/
</script>

<style lang="scss" scoped>
  /* Header Start (logo, button) */
  .header {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 1px;
    padding: 25px;
    margin-bottom: -50px;
    transition: all 350ms cubic-bezier(.83,.01,.46,.86);
    overflow: visible;
  }

  .head_logo {
    position: fixed;
    width: 150px;
    height: 45px;
    float: left;
    vertical-align: top;
    line-height: 45px;
    text-align: center;
    font-size: 25px;
    color: #fdfdfd;
    z-index: 5000;
    border-radius: 4px;
    transition: all 350ms cubic-bezier(.83,.01,.46,.86);
    &:hover {
      background-color: rgba(25, 25, 25, 0.6);
    }
  }
  .head_logo_inner {
    display: block;
    width: 100%;
    height: 100%;
    color: #fdfdfd;
  }

  /* Center buttons */
  .button_middle {
    position: relative;
    width: 100px;
    height: 50px;
    line-height: 53px;
    text-align: center;
    float: right;
    color: #fff68f;
    z-index: 5000;
    right: 25px;
  }

  .button_middle_inner {
    color: #fdfdfd;
    font-weight: bold;
    transition: all 350ms cubic-bezier(.83,.01,.46,.86);
    &:hover {
      color: #aeaeae;
    }
  }

  /* Hamburger Menu button */
  .button_menu:before {
    width: 100%;
    height: 100%;
    content: '\2630';
    font-size: 35px;
    line-height: 53px;
    color: #002778;
  }
  .button_menu {
    position: fixed;
    width: 50px;
    height: 50px;
    vertical-align: top;
    text-align: center;
    cursor: pointer;
    margin-left: calc(100% - 100px);
    z-index: 5000;
    &:hover:before {
      color: #d60c47;
    }
  }

  header:after {
    content: '';
    display: block;
    clear: both;
  }
  /* Header End and Clear float */

  /*
  ===============================================
  Media query
  ===============================================
  */

</style>
