<template>
  <div id="app">
    <Heart />
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import Heart from './components/Heart.vue';

export default {
  components: {
    Heart,
  }
};
</script>

<style>
#app {
  font-family: Arial, Helvetica, sans-serif;
  display: flex;
  justify-content: center;
  align-items: center;
  /* min-height: 100vh; */
  /* background-color: ; */
}
</style>
