<template>
  <div class="container">
    <app-header></app-header>
    <div class="row">
      <div class="col-xs-6">
        <app-servers></app-servers>
      </div>
      <div class="col-xs-6">
        <app-server-details></app-server-details>
      </div>
    </div>
    <app-footer></app-footer>
  </div>
</template>

<script>
import Header from './components/Shared/Header.vue';
import Footer from './components/Shared/Footer.vue';

import Servers from './components/Server/Servers.vue';
import ServerDetails from './components/Server/ServerDetails.vue';

export default {
  components: {
    'app-header': Header,
    'app-servers': Servers,
    'app-server-details': ServerDetails,
    'app-footer': Footer,
  },
  data: function() {
    return {
    }
  },
  methods: {

  }
}
</script>
