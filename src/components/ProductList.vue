<template>
  <div>
    <h2>Product List</h2>
    <div v-if="products.length > 0">
      <ProductItem v-for="product in products" :key="product.id" :product="product" />
    </div>
    <div v-else>
      <p>No products available.</p>
    </div>
  </div>
</template>

<script>
import ProductItem from './ProductItem.vue'; // Import the ProductItem component

export default {
  components: {
    ProductItem
  },
  data() {
    return {
      products: [
        { id: 1, name: 'Product A', description: 'Description A', price: '$10' },
        { id: 2, name: 'Product B', description: 'Description B', price: '$20' },
        { id: 3, name: 'Product C', description: 'Description C', price: '$30' }
      ]
    };
  }
}
</script>
