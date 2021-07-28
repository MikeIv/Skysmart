<template>
  <header id="nav" class="header">
    <div class="header__wrapper">
      <div class="header__logo">
        <img src="../assets/img/skysmart-logo.svg" alt="logo" class="header__logo-img">
      </div>

      <a href="#" class="header__nav-link">Записаться</a>

      <button class="header__mob-menu-btn" @click="menuShow = !menuShow">
        <svg class="header__mob-menu-icon" role="presentation">
          <use xlink:href="#icon-menu"></use>
        </svg>
      </button>

      <nav class="header__list header__list--dt" v-for="link in links" :key="link.title">
        <router-link :to="link.url" :title="link.title" class="header_app__item">{{ link.title }}</router-link>
      </nav>


      <!--   Mobile menu   -->
      <section class="header__mob-nav" v-show="menuShow">
        <h2 class="v-hidden">Навигация</h2>
        <ul class="header__mob-nav-list">
          <li class="header__mob-nav-item">
            <a href="#" class="header__mob-nav-link">Все предметы</a>
          </li>
          <li class="header__mob-nav-item">
            <a href="#" class="header__mob-nav-link">О школе</a>
          </li>
          <li class="header__mob-nav-item">
            <a href="#" class="header__mob-nav-link">Летняя программа</a>
          </li>
          <li class="header__mob-nav-item">
            <a href="#" class="header__mob-nav-link">Записаться на урок</a>
          </li>
        </ul>

        <button class="header__mob-menu-btn header__mob-menu-btn--close" @click="menuShow = false">
          <svg class="header__mob-menu-icon" role="presentation">-->
            <use xlink:href="#icon-close"></use>
          </svg>
        </button>

      </section>

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
    },

  },
  data: () => ({
    menuShow: false,
  })
}
</script>

<style scoped>

</style>