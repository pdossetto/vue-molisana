<template>
  <header>
    <a href="/" class="brand">
      <img src="@/assets/images/logo.png" alt="">
    </a>

    <nav>
      <ul>
        <li v-for="(link, index) in links" :key="index">
          <a :class="(link.current) ? 'active' : null" :href="link.url">
            {{ link.text }}
          </a>
        </li>
      </ul>
    </nav>
  </header>
</template>

<script>
import * as Links from '@/assets/data/Links.js';
export default {
  name: 'Header',

  data() {
    return {
      links: Links.headerLinks
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  @import "../style/mixins";
  @import "../style/vars";

  header {
    text-align: center;

    ul {
      list-style: none;
      @include center();
      
      li a {
        display: inline-block;
        padding: 1rem;
        text-decoration: none;
        font-weight: 600;
        transition: color 0.3s;

        &:hover,
        &.active {
          color: $primary;
        }
      }
    }
  }
</style>
