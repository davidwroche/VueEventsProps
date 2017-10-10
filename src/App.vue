<template>
  <div id="app">
    <span><h1>App Root</h1></span>
    <parentpanel></parentpanel>
  </div>
</template>

<script>
import ParentPanel from './components/ParentPanel.vue';
export default {
  components: {
      parentpanel: ParentPanel,
    },
}
</script>

<style>
#app {
  background-color: yellow;
}
</style>
