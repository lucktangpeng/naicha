<template>
  <div class="all_nav">
    <div class="nav">
      <div class="back">
        <img src="@/images/back@2x.png" />
      </div>
      <div class="seach">
        <img class="search" src="@/images/search@2x.png" />
        <img class="star" src="@/images/star@2x.png" />
      </div>
    </div>
    <div class="title">
      <div class="title_img">
        <img src="@/images/head@2x.png" />
        <div class="title_msg">
          <div class="msg">安和yAng的面包</div>
          <div class="address">智图南路888号</div>
        </div>
      </div>

      <div class="grade">4.0</div>
    </div>
    <div class="classify">
      <div>点餐</div>
      <div>评论 (3896)</div>
      <div>商家</div>
    </div>
  </div>
</template>

<script>
export default {
  name: "top"
};
</script>

<style lang="scss" scoped>
.all_nav {
  //   background: linear-gradient(to bottom, #ff6900 0%, #ff7e00 56%);
  background: #faae6b;
  padding: 36.25pt 11.75pt 22.5pt 11.75pt;
  .nav {
    display: flex;
    justify-content: space-between;
    // margin-top: 36.25pt;
    .back {
      img {
        width: 8.25pt;
        height: 15.25pt;
      }
    }
    .seach {
      .search {
        width: 15.25pt;
        height: 15.25pt;
        margin-right: 12.25pt;
      }
      .star {
        width: 16pt;
        height: 15.25pt;
      }
    }
  }
  .title {
    display: flex;
    justify-content: space-between;
    margin-top: 14pt;
    .title_img {
      display: flex;

      img {
        // width: 108.5pt;
        width: length(108.5);
        height: 58.75pt;
        margin-right: 15.75pt;
      }
      .title_msg {
        margin-top: 8pt;
        .msg {
          font-size: 13.75pt;
          color: #000;
          font-weight: 700;
        }
        .address {
          display: inline-block;
          font-size: 5.485pt;
          border-radius: 6.15pt;
          padding: 3.5pt 11.5pt 3.5pt 11.5pt;
          margin-top: 6.25pt;
          background: rgba(255, 255, 255, 0.32);
          color: rgba(116, 115, 141, 1);
        }
      }
    }

    .grade {
      width: 31pt;
      height: 32.25pt;
      line-height: 32.25pt;
      font-size: 10pt;
      text-align: center;
      background-image: url("../images/bg@2x.png");
      background-size: 31pt 32.25pt;
      color: #fff;
      // float: right;
    }
  }
  .classify {
    display: flex;
    justify-content: space-around;
    margin-top: 18.25pt;
    font-size: 9.5pt;
    color: rgba(189, 94, 31, 1);
  }
}
</style>