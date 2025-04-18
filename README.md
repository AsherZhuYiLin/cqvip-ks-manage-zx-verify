# zx-verify

## 图形验证码组件演示地址 [图形验证码组件演示地址](http://mpfhrd48.sanxing.uz7.cn/zx-verify/)

## 完整版演示地址 [图形验证码组件演示地址](http://mpfhrd48.sanxing.uz7.cn/vue-admin-beautiful/#/byui/verify)

## 安装方法

```
cnpm i -S zx-verify

```

## verify 组件 main.js 全局引入

```
import Vue from 'vue'
import ZxVerify from 'zx-verify'
Vue.component('byui-verify', ZxVerify)

```

## template 完整示例

```
<template>
  <div id="app">
    <byui-verify
      ref="slideDiv"
      :w="350"
      :slider-text="text"
      :h="175"
      @success="handleSuccess"
      @fail="handleError"
    ></byui-verify>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      text: "向右滑动",
    };
  },
  created() {},
  mounted() {},
  methods: {
    handleSuccess() {
      alert("校验成功");
    },
    handleError() {
      alert("校验失败");
    },
  },
};
</script>

<style>
body {
  margin: 0;
  padding: 0;
}

#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
</style>


```
