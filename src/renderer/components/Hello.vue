<script setup lang="ts">
const msg = 'Electron + Vue3 template';
</script>

<template>
  <a-layout class="layout">
    <a-layout-header id="header">
      <p style="color:white">Header</p>
    </a-layout-header>
    <a-layout-content>
        <webview src="https://baidu.com" style="height: 100%; width: 100%;"/>
    </a-layout-content>
    <a-layout-footer>
      Footer
    </a-layout-footer>
  </a-layout>
</template>

<style scoped>
</style>
