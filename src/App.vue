<template>
  <div class="container">
    <app-header></app-header>
    <app-servers></app-servers>
    <app-footer></app-footer>
  </div>
</template>

<script>
import Header from './components/Shared/Header.vue';
import Servers from './components/Server/Servers.vue';
import Footer from './components/Shared/Footer.vue';

export default {
  components: {
    'app-header': Header,
    'app-servers': Servers,
    'app-footer': Footer,
  }
}
</script>
