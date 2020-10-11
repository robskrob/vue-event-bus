<template>
  <div>{{ message }}

    <component-c></component-c>
  </div>
</template>

<script>
const ComponentC = require('./ComponentC');
const EventBus = require('../bus');

module.exports = {
  components: {
    ComponentC,
  },

  data: function () {
    EventBus.$on('say-hello', () => {
      this.message = 'Hello from Component A';
    });

    return {
      message: 'Lonely Component Here!'
    }
  }
}
</script>
