<template>
  <a-layout class="layout">
    <a-layout-header>
      <div class="logo" />
      <div style="font-size: 18px; color: aliceblue">
        超级文本链接分享工具 - 公众号 一个橙子pro
      </div>
    </a-layout-header>
    <a-layout-content>
      <div
        :style="{
          background: '#fff',
          padding: '24px',
          minHeight: 'calc(100vh - 240px)',
          maxWidth: '1200px',
          margin: '0 auto',
        }"
      >
        <router-view />
      </div>
    </a-layout-content>
    <a-layout-footer style="text-align: center">
      <img style="width: 150px" :src="qrcode" />
      <div>
        一个橙子出品,
        上边是我的微信公众号。这个版本提供给网友折腾，请勿用于非法用途.
      </div>
    </a-layout-footer>
  </a-layout>
</template>
<script lang="ts" setup>
import qrcode from "@/assets/da428b3b6d6e058eb738e6b77a08e9b.jpg";
</script>

<style>
.site-layout-content {
  min-height: 280px;
  padding: 24px;
  background: #fff;
}
#components-layout-demo-top .logo {
  float: left;
  width: 120px;
  height: 31px;
  margin: 16px 24px 16px 0;
  background: rgba(255, 255, 255, 0.3);
}
.ant-row-rtl #components-layout-demo-top .logo {
  float: right;
  margin: 16px 0 16px 24px;
}

[data-theme="dark"] .site-layout-content {
  background: #141414;
}
</style>
