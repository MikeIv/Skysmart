<template>
  <header id="nav" class="header">
    <div class="header__wrapper">
      <div class="header__logo">
        <img src="../assets/img/skysmart-logo.svg" alt="logo" class="header__logo-img">
      </div>

      <nav class="header_app__list header_app__list--dt" v-for="link in links" :key="link.title">
        <router-link :to="link.url" :title="link.title" class="header_app__item">{{ link.title }}</router-link>
      </nav>


<!--   Mobile menu   -->

    </div>
  </header>
</template>

<script>
export default {
  name: "Header",
  props: {
    links: {
      type: Array,
      requred: true
    }
  }
}
</script>

<style scoped>

</style>