<script setup lang="ts">
import Hello from './components/Hello.vue'

window.electron.ipcRenderer.send('message', 'Hello from App.vue!');
</script>

<template>
  <div id="app">
    <Hello/>
  </div>
</template>

<style>
#root, body, html {
  height: 100%;
  background-color: aqua;
}

#app {
  display: flex;
  width: 100%;
  min-height: 100%;
}
</style>