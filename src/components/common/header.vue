<template>
  <!-- 顶部导航栏 -->
  <div class="header">
    <!-- 栅格布局 -->
    <a-row>
      <a-col :span="4">
        <!-- 一般一个页面只有一个h标签，logo -->
        <h1>Pully's Blog</h1>
      </a-col>
<!-- input 输入框 -->
      <a-col :span="4">
        <a-input-search placeholder="input search text" style="width: 200px" @search="onSearch"/>
      </a-col>
      <!-- menu导航菜单 -->
      <a-col :span="12">
        <a-menu v-model="current" mode="horizontal" class="menu">
          <a-menu-item key="home">
            <a-icon type="home"/>Home
          </a-menu-item>
          <a-menu-item key="doc">
            <a-icon type="mail"/>Doc
          </a-menu-item>
          <a-menu-item key="tags">
            <a-icon type="mail"/>tags
          </a-menu-item>
          <a-menu-item key="link">
            <a-icon type="mail"/>Link
          </a-menu-item>
        </a-menu>
      </a-col>
      <!-- buttpn 登陆/注册 -->
      <a-col :span="4">
        <div>
          <a-button type="primary">登录</a-button>
          <a-button class="reg">注册</a-button>
        </div>
      </a-col>
    </a-row>
  </div>
</template>

<script>
export default {
  data() {
    return {
      current: ["home"]
    };
  },
  methods: {
    onSearch(value) {
      console.log(value);
    }
  }
};
</script>

<style>
.ant-layout-header {
  background: white !important;
  padding: 0 !important;
}
.ant-menu-horizontal {
  line-height: 62px !important;
  border-bottom: none !important;
}
h1 {
  margin: 0 !important;
  padding: 0;
  font-size: 20px;
  /* 去掉默认加粗 */
  font-weight: normal !important;
  color: #2c3e50;
}
.reg {
  margin-left: 20px;
}
.menu {
  margin-left: 210px !important;
}

</style>
