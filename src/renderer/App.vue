<template>
  <div id="app">
    <router-view></router-view>
  </div>
</template>

<script>
  // import { electron } from 'electron'
  export default {
    name: 'vue-electron',
    mounted () {
      // var alertOnlineStatus = function () {
      //   ipc.send('online-status-changed', navigator.onLine ? 'online' : 'offline')
      //   // window.alert(navigator.onLine ? 'online' : 'offline')
      // }
      // window.addEventListener('online', alertOnlineStatus)
      // window.addEventListener('offline', alertOnlineStatus)
      // alertOnlineStatus()
      const fs = require('fs')

      const root = fs.readdirSync('/')

      // 这会打印出磁盘根级别的所有文件
      // 同时包含'/'和'C:\'。
      console.log(root)
    }
  }
</script>

<style>
  /* CSS */
</style>
