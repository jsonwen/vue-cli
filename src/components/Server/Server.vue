<template>
    <li
      class="list-group-item"
      @click="serverSelected"

    >
      Server #{{ server.id }}:
      Status {{ server.status }}
    </li>
</template>

<script>
import { serverBus } from '../../main';

export default {
  props: ['server'],
  methods: {
    serverSelected() {
      serverBus.$emit('serverSelected', this.server);
    }
  }
}
</script>
