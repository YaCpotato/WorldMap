<template>
  <div class="home">
    <World :name="svgFileName" />
  </div>
</template>

<script>
import World from "../components/World.vue";
export default {
  name: "Home",
  components: { World },
  data() {
    return {
      svgFileName: "world"
    };
  }
};
</script>
