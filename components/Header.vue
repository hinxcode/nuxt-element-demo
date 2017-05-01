<template>
  <div>
    <el-menu theme="dark" :default-active="homeUrl" :router=true mode="horizontal">
      <el-menu-item index="/">首頁</el-menu-item>
      <el-menu-item index="/about">關於我們</el-menu-item>
    </el-menu>
  </div>
</template>

<script>
  export default {
    data () {
      return {
        homeUrl: '/',
        aboutUs: '/about'
      }
    }
  }
</script>
