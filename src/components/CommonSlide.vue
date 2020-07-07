<template>
  <div class="slide">
    <div class="title">
      <div class="left">
        <img src="@/images/hot@2x.png" />
        <span class="left_msg">本店热卖</span>
      </div>
      <div class="right">
        <div class="right_msg">综合</div>
        <img src="@/images/icon@2x.png" alt />
      </div>
    </div>
    <div class="wrapper">
      <ul class="content">
        <li class="ka">
          <img src="@/images/image@2x.png" />
          <div>芒果超人面包</div>
          <div>
            <span>¥19.9</span>
            <img src="@/images/add@2x.png" alt="" />
          </div>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
import BScroll from "better-scroll";
// import scrollLock from "scroll-lock";
// import { enablePageScroll } from "scroll-lock";
// import scrollLock from 'scroll-lock';
export default {
  name: "slide",
  data() {
    return {
      soc_1: "",
    };
  },
  mounted() {
    this.$nextTick(() => {
      this.scroll = new BScroll(this.$refs.left, {
        click: true,
      });
      //   const $scrollableElement = document.querySelector(".content");
      //   enablePageScroll($scrollableElement);
    });
    console.log(this.scroll);

    // const wrapper = document.querySelector(".weapper");
    // this.soc_1 = new BScroll(wrapper); // no-unused-vars
  },
};
</script>

<style lang="scss" scoped>
.slide {
  background: #fff;
  padding: 15.75pt 13.75pt;
  position: relative;
  top: -10pt;
  border-radius: 10pt 10pt 0 0;
  .title {
    display: flex;
    justify-content: space-between;
    padding-bottom: 7.75pt;
    ::after {
      content: "  ";
      position: absolute;
      left: 5%;
      bottom: 0;
      width: 90%;
      height: 1px;
      background-color: rgba(238, 237, 233, 1);
      /* 如果不用 background-color, 使用 border-top:1px solid #f00; 效果是一样的*/
      -webkit-transform: scaleY(0.5);
      transform: scaleY(0.5);
    }
    .left {
      display: flex;
      align-items: center;
      .left_msg {
        color: rgba(51, 51, 51, 1);
      }
      img {
        width: 9.25pt;
        height: 11.5pt;
        vertical-align: middle;
        margin-right: 3.25pt;
      }
    }
    .right {
      display: flex;
      align-items: center;
      .right_msg {
        color: rgba(170, 170, 170, 1);
      }
      img {
        width: 9.5pt;
        height: 9.5pt;
        margin-left: 3.25pt;
      }
    }
  }
  .wrapper {
    height: 100pt;
    overflow: hidden;
    .content {
      .ka {
        img {
          width: 63.75pt;
          height: 46.75pt;
        }
      }
      // display: flex;
      //   this.scroll = new BScroll(this.$refs.tabsWrapper, {
      //           scrollX: true,
      //           eventPassthrough: 'vertical',
      //         })
    }
  }
}
</style>
