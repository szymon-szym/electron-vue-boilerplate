<template>
  <div class="mainView">
    <h1>{{ test }}</h1>
    <v-btn @click="testLog">button</v-btn>
  </div>
</template>

<script>
const log = require('electron-log')
export default {
  name: 'MainView',
  data() {
    return {
      test: 'test'
    }
  },
  methods: {
    testLog() {
      log.info('hello log')
      log.debug('debug msg')
      log.warn('warn')
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
