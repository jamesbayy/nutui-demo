<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <nut-button>Button 3.0</nut-button>
  <nut-button type="primary">主要按钮</nut-button>
  <nut-button type="info">信息按钮</nut-button>
  <nut-button type="default">默认按钮</nut-button>
  <nut-button type="danger">危险按钮</nut-button>
  <nut-button type="warning">警告按钮</nut-button>
  <nut-button type="success">成功按钮</nut-button>
  <nut-cell title="123123213312">123123</nut-cell>
  <nut-icon name="dongdong"></nut-icon>
  <nut-fixednav :position="{bottom:'70px' }" v-model:visible="visible" :nav-list="navList" />
  <nut-cell title="自定义 Icon 字体">
    <!-- 通过 class-prefix 指定类名为 my-icon -->
    <nut-icon font-class-name="iconfont" class-prefix="icon" name="mianji" />
    <span class="iconfont icon-mianji"></span>
  </nut-cell>

  <HelloWorld msg="Hello Vue 3 + Vite" />
</template>

<script setup>
import HelloWorld from "./components/HelloWorld.vue";
import { ref, reactive } from "vue";
const visible = ref(false);
const navList = reactive([
  {
    id: 1,
    text: "首页",
    icon: "https://img11.360buyimg.com/imagetools/jfs/t1/117646/2/11112/1297/5ef83e95E81d77f05/daf8e3b1c81e3c98.png",
  },
  {
    id: 2,
    text: "分类",
    icon: "https://img12.360buyimg.com/imagetools/jfs/t1/119490/8/9568/1798/5ef83e95E968c69a6/dd029326f7d5042e.png",
  },
  {
    id: 3,
    text: "购物车",
    num: 2,
    icon: "https://img14.360buyimg.com/imagetools/jfs/t1/130725/4/3157/1704/5ef83e95Eb976644f/b36c6cfc1cc1a99d.png",
  },
  {
    id: 4,
    text: "我的",
    icon: "https://img12.360buyimg.com/imagetools/jfs/t1/147573/29/1603/1721/5ef83e94E1393a678/5ddf1695ec989373.png",
  },
]);
// This starter template is using Vue 3 experimental <script setup> SFCs
// Check out https://github.com/vuejs/rfcs/blob/script-setup-2/active-rfcs/0000-script-setup.md
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
