<template>
  <div class='page-home'>
    <h1 @click="goLogin">首页</h1>
    <router-link to='classify'>{{string}}</router-link>
  </div>
</template>

<script>
export default {
  name: 'home',
  data () {
    return {
      string: '李志鹏'
    }
  },
  methods: {
    goLogin () {
      this.$router.push('./classify')
    }
  }
}
</script>
