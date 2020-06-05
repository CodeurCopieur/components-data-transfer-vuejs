<template>
  <div id="app">
    <List />
  </div>
</template>

<script>

import List from  './components/List'

export default {
  name: 'app',
  components: { List },
  data () {
    return {
     items: ['Dev Front-End', 'Dev Back-End', 'Dev Full Stack']
    }
  }
}
</script>

<style lang="scss">

@import url('./assets/scss/index.scss');

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

</style>
