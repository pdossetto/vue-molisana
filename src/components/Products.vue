<template>
  <div>
    <!-- <ul>
      <li v-for="(product, index) in products" :key="index">
        {{product.titolo}}
      </li>
    </ul> -->

    <ProductCard 
      v-for="(product, index) in products" 
      :key="index"
      :prod="product"
    />

  </div>
</template>

<script>
import ProductCard from '@/components/ProductCard.vue'
import ProdItems from '@/data/ProdItems.js'
export default {
  name: 'Products',
  components: {
    ProductCard
  },
  data() {
    return {
      products: ProdItems
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>
