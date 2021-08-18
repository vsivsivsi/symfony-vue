<template>

  <div>
    <title-component :text="title"></title-component>

    <product-list-component :products="pruducts"></product-list-component>
  </div>
</template>

<script>
  import TitleComponent from '@/components/title';
  import ProductListComponent from "./ProductList";

  export default {
    name: "Catalog",
    components: {
      TitleComponent,
      ProductListComponent
    },
    data: () => (
        {
          title: 'Product list',
          pruducts: [
            {
              name: 'Product 1',
            },
            {
              name: 'Product 2',
            },
            {
              name: 'Product 3',
            },
          ]
        }
    )
  }
</script>

<style scoped>

</style>