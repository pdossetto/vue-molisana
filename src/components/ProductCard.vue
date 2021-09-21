<template>
  <div class="product-card">
    <h1>{{ prod.titolo }}</h1>
    <h2>Cottura: {{ prod.cottura }} minuti</h2>
    <img :src="prod.src" :alt="prod.titolo">
    <br/>
  </div>
</template>

<script>
export default {
  name: 'ProductCard',
  props: ['prod']
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>
