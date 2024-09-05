<template>
  <section>
    <Sections />
    <div>
      <Card />
    </div>
  </section>
</template>
<script>
import Sections from "../components/sections.vue";
import Card from "../components/card.vue";

export default {
  props: ["products"],
  components: {
    Sections,
    Card,
  },
  mounted() {
    this.$emit("to-parent", "Hey parent, from child");

    this.products.forEach((product) => {
      console.log(product.name);
    });
  },
};
</script>
<style></style>
