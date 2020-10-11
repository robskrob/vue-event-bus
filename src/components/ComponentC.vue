<template>
  <div>C: {{ message }}</div>
</template>

<script>
const EventBus = require('../bus');

module.exports = {
  data: function () {
    EventBus.$on('say-hello', () => {
      this.message = 'Hello from Component A';
    });

    return {
      message: 'Lonely Component Here!'
    }
  },


}
</script>
