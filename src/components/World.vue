<template>
  <component :is="svg" />
</template>

<script>
export default {
  name: "World",
  props: {
    name: {
      type: String,
      required: true
    }
  },
  computed: {
    svg() {
      return () => import(`../assets/svg/${this.name}.svg`);
    }
  }
};
</script>
