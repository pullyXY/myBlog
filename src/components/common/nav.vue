<template>
  <!-- 内容，左边部分-->
  <div class="nav">
    <!-- 头像 -->
    <div>
      <a-avatar
        :size="120"
        src="http://img5.duitang.com/uploads/item/201406/28/20140628145613_VWnXL.jpeg"
      />
    </div>
    <!-- user->pully -->
    <div class="user">
      <span>Pully</span>
    </div>
    <!-- 个签 -->
    <div class="tips">醉里插花花莫笑，可怜春似人将老</div>
    <!-- github/wechat 入口 icon -->
    <div class="media">
      <div class="nav_left_icon">
        <a-icon type="github"/>
        <span class="nav_left_icon_name">github</span>
      </div>
      <div class="nav_left_icon" style="margin-left: 10px">
        <a-icon type="wechat"/>
        <span class="nav_left_icon_name">wechat</span>
      </div>
    </div>
    <!-- 最近文章 -->
    <a-divider orientation="left" class="recently">最近文章</a-divider>
    <div class="artical">
      <ul>
        <li>1醉里插花花莫笑，可怜醉里插花花莫笑，可怜春似人将老醉里插花花莫笑，可怜春似人将老</li>
        <li>2醉里插花花莫笑，可怜</li>
        <li>3醉里插花花莫笑，可怜</li>
        <li>1醉里插花花莫笑，可怜醉里插花花莫笑，可怜春似人将老醉里插花花莫笑，可怜春似人将老</li>
        <li>2醉里插花花莫笑，可怜</li>
        <li>3醉里插花花莫笑，可怜</li>
        <li>1醉里插花花莫笑，可怜醉里插花花莫笑，可怜春似人将老醉里插花花莫笑，可怜春似人将老</li>
        <li>2醉里插花花莫笑，可怜</li>
        <li>3醉里插花花莫笑，可怜</li>
      </ul>
    </div>
    <!-- 左下标签 tag-->
    <a-divider orientation="left" class="recently">标签</a-divider>
    <div>
      <a-tag class="tages" color="pink">pink</a-tag>
      <a-tag class="tages" color="red">red</a-tag>
      <a-tag class="tages" color="orange">orange</a-tag>
      <a-tag class="tages" color="green">green</a-tag>
      <a-tag class="tages" color="cyan">cyan</a-tag>
      <a-tag class="tages" color="blue">blue</a-tag>
      <a-tag class="tages" color="purple">purple</a-tag>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  }
};
</script>

<style>
.nav {
  /* 左边部分内容的边框.右 */
  border-right: 1px solid rgb(232, 232, 232);
 
}
.user {
  margin-top: 20px;
  font-size: 20px;
  font-weight: bold;
}
.tips {
  margin-top: 10px;
  font-size: 13px;
}
.recently {
  box-sizing: border-box;
  padding-left: 20px !important;
  padding-right: 20px !important;
}
.nav_left_icon {
  display: inline-block;
}
.media {
  margin-top: 10px;
  padding-bottom: 20px;
}
.nav_left_icon_name {
  margin-left: 2px;
}
.artical > ul {
  padding-left: 20px;
}
.artical > ul > li {
  /* 溢出... start */
  overflow: hidden;
  text-overflow: ellipsis;
  white-space: nowrap;
  /* 溢出... end */

  /* 文字居中 ：行高等于高*/
  line-height: 28px;
  height: 28px;

  color: #8590a6;
  text-align: left;
}
.artical > ul > li:hover {
/* 鼠标悬浮字体和背景变色 */
  color: black;
  background: #eee;
  
}
.tages {
  margin-top: 6px !important;
  margin-bottom: 6px !important;
}
</style>
