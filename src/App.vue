<template>
  <div id="app">
    <div id="components-layout-demo-basic">
      <a-layout>
        <!-- 顶部导航栏 -->
        <a-layout-header>
          <Header></Header>
        </a-layout-header>
        <!-- 内容 -->
        <a-layout-content>
          <div class="content">
            <!-- 分左右两块 -->
            <a-row>
              <a-col :span="5" class="leftNav"><Nav></Nav></a-col>
              <!-- position:fixed;脱离文档流 ，在写一个一样大小的占位 -->
              <a-col :span="5"></a-col>
              <a-col :span="19" class="home"><Home></Home></a-col>
            </a-row>
          </div>
        </a-layout-content>
      </a-layout>
    </div>
  </div>
</template>

<script>
// 引公共Header，Nav
import Header from "./components/common/header.vue";
import Nav from './components/common/nav'
import Home from './components/page/home'
export default {
  name: "app",
  components: {
    Header,
    Nav,
    Home
  },
  data() {
    return {
      current: ["mail"]
    };
  }
};
</script>

<style>
.leftNav {
  position: fixed!important;
  top: 115px;
  left: 0;
  height: calc(100vh - 135px);
  overflow: auto;
}

#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
#components-layout-demo-basic {
  text-align: center;
}
#components-layout-demo-basic .ant-layout-header{
  margin-bottom: 1px!important;
  /* color: #fff; */
}
#components-layout-demo-basic .ant-layout-footer {
  line-height: 1.5;
}
#components-layout-demo-basic .ant-layout-sider {
  background: #3ba0e9;
  /* color: #fff; */
  /* line-height: 120px; */
}
#components-layout-demo-basic .ant-layout-content {
  /* background: rgba(16, 142, 233, 1); */
  /* color: #fff; */
  min-height: 120px;
  /* line-height: 120px; */
}
#components-layout-demo-basic > .ant-layout {
  margin-bottom: 48px;
}
#components-layout-demo-basic > .ant-layout:last-child {
  margin: 0;
}
.content {
  padding-top: 50px;
  background: white;
}
</style>
