<template>
  <Header></Header>
  <Options />
</template>

<script>
import Header from "./components/Header.vue";
import Options from "./components/Options.vue";

export default {
  name: "App",
  components: {
    Header,
    Options,
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Lato:wght@300;400;700&family=Poppins:wght@300;400;600;900&display=swap");

#app {
  font-family: "Poppins", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #0b1d44;

  min-height: 100vh;
  max-width: 600px;
  margin: 0 auto;
  display: flex;
  flex-direction: column;
}

body {
  margin: 0;
  /* Gradient */
  background-color: #8EC5FC;
  background-image: linear-gradient(62deg, #8EC5FC 0%, #E0C3FC 100%);
  /* Glass */
  box-shadow: 0 8px 32px 0 rgba(31, 38, 135, 0.37);
  backdrop-filter: blur(20px);
  -webkit-backdrop-filter: blur(20px);
  background-size: cover;
  background-repeat: no-repeat;
}

h1,
h2,
h3,
h4,
h5,
h6 {
  font-family: "Lato", sans-serif;
}

.btn {
  -webkit-tap-highlight-color: transparent;
}

.btn:active {
  transform: scale(0.9);
}
</style>
