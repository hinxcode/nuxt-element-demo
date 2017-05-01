<template>
  <div style="text-align:center;">
    <div class="block">
        <el-carousel height="400px">
          <el-carousel-item v-for="(item, key) in 3" v-bind:key="key">
            <img :src="item.image" alt="" style="width:100%;height:100%">
          </el-carousel-item>
        </el-carousel>
      </div>
  </div>
</template>

<style lang="scss">
  $oddBgColor: #d3dce6;
  $evenBgColor: #d2e6de;

  .el-carousel__item {
    h3 {
      color: #475669;
      font-size: 14px;
      opacity: 0.75;
      line-height: 150px;
      margin: 0;
    }
  }
  .el-carousel__item:nth-child(2n) {
     background-color: $evenBgColor;
  }
  .el-carousel__item:nth-child(2n+1) {
     background-color: $oddBgColor;
  }
</style>

<script>
  export default {
    data () {
      return {
        roll: []
      }
    },
    methods: {
      btnClick: function () {
        this.$message.success('ok')
      }
    },
    mounted: function () {
    }
  }
</script>
