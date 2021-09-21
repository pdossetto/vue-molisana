<template>
  <div id="app">
    <Header />

    <main>
      <Products />
    </main>
    

    <Footer />
  </div>
</template>

<script>
// La @ ci porta direttamente nella cartella src del progetto
import Header from '@/components/Header.vue'
import Products from '@/components/Products.vue'
import Footer from '@/components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Products,
    Footer
  }
}
</script>

<style lang="scss">

@import "./style/generals";
@import "./style/vars";

h1,
h2,
h3 {
  color: $primary;
}

#app {
  text-align: center;
}


</style>
