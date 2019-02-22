<template>
  <div style="margin-top:30px;">
    <div>pages-artical</div>
    <ul>
      <li v-for="(item,index) in list" :key="index">
        <span>{{item.title}}</span>
        <nuxt-link :to="'/artical/'+(index+1)">详情</nuxt-link>
      </li>
    </ul>
    <nuxt-child />
  </div>
</template>

<script>
  export default {
    name: '',
    data() {
      return {
        list:[
          {
            title:'新闻111'
          },
          {
            title:'新闻222'
          },
          {
            title:'新闻333'
          }
        ]
      }
    }
  }
</script>

<style scoped>
  
</style>