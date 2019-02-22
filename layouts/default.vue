<template>
  <div>
    <header style="background-color:pink;padding:10px 0;">
      <Logo></Logo>
      <ul class="nav">
        <li><nuxt-link to="/" exact>home</nuxt-link></li>
        <li><nuxt-link to="/artical/1" exact>artical</nuxt-link></li>
        <li><nuxt-link to="/about">about</nuxt-link></li>
      </ul>
    </header>
    <nuxt />
  </div>
</template>
<script>
import Logo from '@/components/Logo.vue'
export default {
  components:{
    Logo
  }
}
</script>
<style>
.nav{
    width:400px;
    margin:10px auto;
    overflow:hidden;
    
  }
  .nav li{
    width:100px;
    list-style:none;
    float:left;
  }
html {
  font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
  text-align:center;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}

.button--green {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #3b8070;
  color: #3b8070;
  text-decoration: none;
  padding: 10px 30px;
}

.button--green:hover {
  color: #fff;
  background-color: #3b8070;
}

.button--grey {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #35495e;
  color: #35495e;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 15px;
}

.button--grey:hover {
  color: #fff;
  background-color: #35495e;
}
</style>
