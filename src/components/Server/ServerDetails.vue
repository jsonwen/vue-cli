<template>
  <div>
    <div v-if="!server">
      Select server
    </div>
    <div v-else>
      <div>Server #{{ server.id }}</div>
      <div>Status: {{ server.status }}</div>
      <button @click="resetStatus">Fix</button>
    </div>
  </div>
</template>

<script>
import { serverBus } from '../../main';
export default {
  data: function() {
    return {
      server: null
    }
  },
  created() {
    serverBus.$on('serverSelected', (server) => {
      this.server = server;
    });
  },
  methods: {
    resetStatus() {
      this.server.status = 'Normal'
    }
  }
}
</script>
