<template>
  <div class="col">
    <div class="card p-3">
      <img
        :src="product.image"
        class="card-img-top"
        alt="..."
      />
      <div class="card-body">
        <h5 class="card-title">{{ product.name }}</h5>
        <div class="card-type">{{ product.type }}</div>
        <h6 class="card-price">{{ product.price + " kr"}}</h6>

        <router-link :to="{name: 'ProductInfo', params: {id: product._id}}" type="button" class="btn btn-info">Show Product</router-link>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ProductCard',
  props: ['product']
}
</script>

<style>
  .card-type{
    color: grey;
    margin-bottom: 18px;
  }
</style>