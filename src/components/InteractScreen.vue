<template>
  <div class="screen">
    <h1>This is Interact Screen</h1>
    <card-flip v-for="(card, index) in cardsContext" :key="index" />
  </div>
</template>

<script>
import CardFlip from "./Card.vue";
export default {
  props: {
    cardsContext: {
      type: Array,
      default: function () {
        return [];
      },
    },
  },
  components: {
    CardFlip,
  },
};
</script>
