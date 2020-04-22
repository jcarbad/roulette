<template>
  <div class="bg-green-600">
    <div class="bg-gray-200 flex">
      <numbers></numbers>
    </div>
  </div>
</template>

<script>
import Numbers from '../molecules/Numbers.vue';
export default {
  name: "Board",
  components: { Numbers }
};
</script>