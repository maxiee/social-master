<script lang="ts">
export default {
  mounted() {
    const webview1 = document.querySelector('#webview1');
    // setTimeout(() => webview1.openDevTools(), 3000);
  }
}
</script>

<template>
  <a-layout class="layout">
    <a-layout-header id="header">
      <p style="color:white">Social Master</p>
    </a-layout-header>
    <a-layout-content>
      <a-row style="height: 100%">
        <a-col :span="12">
          <webview
            id="webview1"
            src="https://m.weibo.cn" 
            style="height: 100%; width: 100%;"/>
        </a-col>
        <a-col :span="12">
          <webview 
            src="https://twitter.com" 
            style="height: 100%; width: 100%;"/>
        </a-col>
      </a-row> 
    </a-layout-content>
    <a-layout-footer>
      Footer
    </a-layout-footer>
  </a-layout>
</template>

<style scoped>
</style>
