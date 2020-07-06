<template>
  <div id="app">
    <div class="top">
      <common-top></common-top>
    </div>
    <div class="bottom">
      <div class="left">
        <common-left></common-left>
      </div>
      <div class="right">
        <common-right></common-right>
      </div>
    </div>
  </div>
</template>
<script>
import CommonLeft from "./components/CommonLeft.vue";
import CommonTop from "./components/CommonTop.vue";
// import CommonRight from "./components/CommonRight.vue";
import CommonRight from "./components/CommonRight.vue";
export default {
  name: "app",
  components: {
    CommonLeft,
    CommonTop,
    CommonRight
  }
};
</script>
<style lang="scss">
</style>
