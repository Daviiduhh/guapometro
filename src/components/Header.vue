<template>
  <header class="header finisher-header">
    <h3 class="header__logo">
      Guapometro
    </h3>
    <div class="header__counter">
      <CircleProgress
      class="circleProgress"
      :size="40"
      :border-width="5"
      :border-bg-width="0"
      :fill-color="'#0b1d44'"
      :color="'#0b1d44'"
      :percent="70"
      :show-percent="true"
      />
    </div>
    <div class="header__hero">
      <h1 class="header__hero__texto">Descubre tu belleza</h1>
      <h4 class="header__hero__texto">Elige una de las siguientes opciones</h4>
    </div>
  </header>
</template>

<script>
import "vue3-circle-progress/dist/circle-progress.css";
import CircleProgress from "vue3-circle-progress";

export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  components: {
    CircleProgress
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
.header {
  margin-top: 10px;
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  justify-content: space-between;
  align-items: center;
}

.header__logo {
  margin: 0;
}
.header__counter p {
  font-weight: 600;
}

.vue3-circular-progressbar {
  margin: 0 auto;
}

.header__hero {
  grid-column: 1 / 3;
  padding: 40px 0 30px 0;
}
</style>