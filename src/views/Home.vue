<template>
  <div class="home">
    <b-navbar-brand href="/login">로그인</b-navbar-brand>
    <b-navbar-brand href="/signup">회원가입</b-navbar-brand>
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>




<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld
  }
}
</script>
