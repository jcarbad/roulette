<template>
  <div class="inline bg-green-700 p-1">
    <div class="flex" v-for="n in 12" :key="n">
      <cell class="m-1" :color="(3 * n - 2) % 2 == 0 ? 'red' : 'black'">{{ 3 * n - 2 }}</cell>
      <cell class="m-1" :color="(3 * n - 1) % 2 == 0 ? 'red' : 'black'">{{ 3 * n - 1 }}</cell>
      <cell class="m-1" :color="(3 * n) % 2 == 0 ? 'red' : 'black'">{{ 3 * n }}</cell>
    </div>
  </div>
</template>

<script>
import Cell from "../atoms/Cell.vue";
export default {
  name: "Numbers",
  components: { Cell },
  methods: {
      showClick(val) {
          console.log(`Clicked cell #${ val }`)
      }
  }
};
</script>