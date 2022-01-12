<template>
  <div class="options">
    <Card
      v-for="(option, index) in options"
      :key="option.id"
      :index="index"
      :message="option.message"
    />
  </div>

  <div class="button">
    <button class="button__button btn">
      Next
    </button>
  </div>
</template>

<script>
import Card from "./Card.vue";

export default {
  data() {
    return {
      options: [
        { message: "❤" },
        { message: "🧡" },
        { message: "💛" },
        { message: "💚" },
        { message: "💙" },
        { message: "💜" },
      ],
    };
  },
  components: {
    Card,
  },
};
</script>

<style scoped>
.options {
  margin: 0 auto;
  width: 90%;
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  justify-content: center;
  align-items: center;
  gap: 20px;
}

.button {
  margin: 20px 0;
}

.button__button {
  width: 90%;
  height: 60px;
  cursor: pointer;
  font-family: "Lato", sans-serif;
  font-weight: 700;
  font-size: 20px;
  /* Glass */
  background: rgba(255, 255, 255, 0.25);
  box-shadow: 0 8px 32px 0 rgba(31, 38, 135, 0.37);
  backdrop-filter: blur(4px);
  -webkit-backdrop-filter: blur(4px);
  border-radius: 10px;
  border: 1px solid rgba(255, 255, 255, 0.18);
}

.button__button:active {
  transform: scale(0.9);
}
</style>