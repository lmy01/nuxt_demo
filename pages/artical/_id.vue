<template>
  <div style="margin-top:30px;">
    <div>pages-artical-child---{{id}}</div>
  </div>
</template>

<script>
  export default {
    name: '',
    validate ({ params }) {
      // 必须是number类型
      console.log("验证id");
      return /^\d+$/.test(params.id)
    },
    data() {
      return {
        id:$nuxt.$route.params.id
      }
    }
  }
</script>

<style scoped>
  
</style>