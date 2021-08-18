<template>
  <div>
    <p v-for="product in products" :key="product">{{ product.name }}</p>
  </div>
</template>

<script>
  export default {
    name: "ProductList",
    props: {
      products: {
        type: Array,
      }
    }
  }
</script>

<style scoped>

</style>