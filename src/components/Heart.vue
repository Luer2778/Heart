<template>
  <div class="heart-container" :style="{ width: size + 'px', height: size + 'px' }">
    <svg
  class="heart"
  xmlns="http://www.w3.org/2000/svg"
  viewBox="0 0 24 24"
  fill="red"
  width="100px"
  height="100px"
>
  <path
    d="M12 21.35l-1.45-1.32C5.4 15.36 2 12.28 2 8.5 2 5.42 4.42 3 7.5 3c1.74 0 3.41.81 4.5 2.09C13.09 3.81 14.76 3 16.5 3 19.58 3 22 5.42 22 8.5c0 3.78-3.4 6.86-8.55 11.54L12 21.35z"
  />
</svg>

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

<style>
.heart-container {
  display: flex;
  justify-content: center;
  align-items: center;
  cursor: pointer;
}

.heart {
  transition: fill 0.3s ease;
}

.heart:hover {
  fill: #e53935;
}
</style>
