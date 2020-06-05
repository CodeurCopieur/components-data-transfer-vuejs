<template>
  <nav>
    <h1>Component List item</h1>
    <ul>
      <li v-for="(data, index) in listdata" :key="index" @click="$emit('clickedItem', data)">{{ data }}</li>
    </ul>
  </nav>
</template>

<script>


export default {
  name: 'List',
  props: {
    listdata:{
      type: Array
    }
  }  
}
</script>

<style lang="scss">

nav {

  display: flex;
  flex-direction: column;

  h1 {
    margin-bottom: 2em;
  }

  ul {
    li {
      margin: 2em 0;
      cursor: pointer;
    }
  }
}
  
</style>
