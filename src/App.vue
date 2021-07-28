<template>
  <div id="app">

    <headertop :links="links" />

    <router-view/>
  </div>
</template>


<script>
import headertop from '@/components/Header.vue'

export default {
  components: {
    headertop
  },
  data: () => ({
    links: [
      { title: '', url: '/' },
      { title: 'Все предметы', url: '/subject' },
      { title: 'О школе', url: '/school' },
    ]
  })
}
</script>


<style lang="scss">


  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
</style>
