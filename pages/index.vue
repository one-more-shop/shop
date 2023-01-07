<template>
  <div class="home">
    <v-row>
      <v-col>
        <product-card />
      </v-col>
    </v-row>
  </div>
</template>

<script>
import ProductCard from '@/components/ProductCard.vue';

export default {
  name: "IndexPage",
  components() {
    ProductCard;
  },
};
</script>

<style scoped>
.home {
  padding: 2em;
}
</style>
