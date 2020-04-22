<template>
  <div id="app" class="flex justify-center bg-gray-200 h-screen">
    <div class="block">
      <Title></Title>
      <Roulette></Roulette>
      <Board></Board>
    </div>
  </div>
</template>

<script>
import Title from "./components/atoms/Title.vue";
import Roulette from './components/organisms/Roulette.vue';
import Board from './components/organisms/Board.vue';

export default {
  name: "App",
  components: {
    Title,
    Roulette,
    Board
  }
};
</script>

