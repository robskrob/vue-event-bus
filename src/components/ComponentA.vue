<template>
  <button
    class="p-4 border bg-gray-100 rounded-lg mb-12"
    @click.prevent="sayHello"
  >
    Say Hello to Component B and C!
  </button>
</template>

<script>
import EventBus from '../bus';

export default {
  methods: {
    sayHello: function () {
      EventBus.$emit('say-hello');
    },
  },
};
</script>
