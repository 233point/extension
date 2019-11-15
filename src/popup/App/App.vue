<template>
  <el-card class="box-card">
    <div
      slot="header"
      class="clearfix"
    >
      <span>233次元</span>
      <a
        href="//calamus.xyz"
        style="float: right; padding: 3px 0;color:pink"
        type="text"
      >主站</a>
    </div>
    <div
      v-for="o in controlList"
      :key="o.key"
      class="text item"
    >
      {{o.name }}
    </div>
  </el-card>
</template>

<script>
export default {
  name: 'app',
  data(){
    return {
      controlList:[
        {
          name:'番剧',
          key:'anime'
        },{
          name:'图片',
          key:'picture'
        },{
          name:'漫画',
          key:'manka'
        }
      ]
    }
  }
}
</script>

<style>
.box-card {
  width: 300px;
}
</style>
