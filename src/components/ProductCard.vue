<template>
  <div>
    <h1>{{ msg }}</h1>
    {{ prod.titolo }}
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
