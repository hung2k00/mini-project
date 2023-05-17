<template>
  <div class="screen">
    <h1>This is Interact Screen</h1>
    <card-flip />
  </div>
</template>

<script>
import CardFlip from "./Card.vue";
export default {
  procs: {
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
