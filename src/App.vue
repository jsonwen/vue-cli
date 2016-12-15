<template>
  <div class="container">
    <app-header></app-header>
    <app-servers></app-servers>
    <app-footer></app-footer>
  </div>
</template>

<script>
import Header from './Header.vue';
import Servers from './Servers.vue';
import Footer from './Footer.vue';

export default {
  components: {
    'app-header': Header,
    'app-servers': Servers,
    'app-footer': Footer,
  }
}
</script>
