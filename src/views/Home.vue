<template>
  <div class="sk">
    <div class="sk__wrapper">
      <h1 class="sk__h1">Онлайн-школа Skysmart</h1>
      <ul class="sk__list">
        <li class="sk__block sk__block--green">
          <p class="sk__block-txt sk__block-txt--green">Подготовиться к школе и весело провести время</p>
        </li>

        <li class="sk__block sk__block--blue">
          <p class="sk__block-txt sk__block-txt--blue">Понять сложный предмет и хорошо сдать экзамены</p>
        </li>

        <li class="sk__block sk__block--yellow">
          <p class="sk__block-txt sk__block-txt--yellow">Найти классное хобби, которое пригодится в жизни</p>
        </li>
      </ul>

      <div class="sk__link-item">
        <a href="#" class="sk__link">Бесплатный <br> вводный урок</a>
      </div>

      <section class="sk__section">
        <h2 class="sk__h2">Как проходят занятия</h2>
        <ul class="sk__list-link">
          <li class="sk__item-link active">
            <a href="" class="sk__link-ls">Вводный урок</a>
          </li>
          <li class="sk__item-link">
            <a href="" class="sk__link-ls">Английский язык</a>
          </li>
          <li class="sk__item-link">
            <a href="" class="sk__link-ls">Математика</a>
          </li>
        </ul>
      </section>
      <div class="sk__video-wrapper">
        <video class="sk__video" autoplay loop>
          <source src="../assets/img/Video_01.mp4" type="video/mp4">
        </video>
      </div>

      <section class="sk__section sk__section--mb">
        <h2 class="sk__h2">Поможем понять, что делает ребенка счастливым, и будем применять это в обучении</h2>
      </section>

      <section class="sk__section sk__section--mb">
        <div class="sk__img-block">
          <img src="../assets/img/bg_figure.png" alt="figure" class="sk__img-figure">
        </div>
        <h2 class="sk__h2">Чтобы записаться на вводный урок, покормите Эла</h2>
      </section>

    </div>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'Home',
  components: {

  }
}
</script>
