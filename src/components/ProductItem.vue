<template>
  <div>
    <h3>{{ product.name }}</h3>
    <p>{{ product.description }}</p>
    <p>Price: {{ product.price }}</p>
    <hr>
  </div>
</template>

<script>
export default {
  props: {
    product: {
      type: Object,
      required: true
    }
  }
}
</script>
