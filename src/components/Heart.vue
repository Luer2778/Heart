<template>
  <div class="heart-container" :style="{ width: size + 'px', height: size + 'px' }">
    <!-- <link type="image/svg+xml" href="./public/heart.svg" /> -->
    <img src="../../public/heart.svg"> </img>
  </div>
</template>

<script>
export default {
  data() {
    return {
      size: 200,
      filled: false,
    };
  },
  methods: {
    toggleHeart() {
      this.filled = !this.filled;
    },
  },
};
</script>
