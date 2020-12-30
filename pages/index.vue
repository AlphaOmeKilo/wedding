<template>
  <div id="home-container" class="screen-container">
    <div id="awreatha-container"  >
      <img :style="`bottom: -${imageOffset}px`" src="~/assets/images/awreatha.png" />
    </div>
    <div id="us-container" class="yellow--bg">
    </div>
  </div>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  data: () => ({
    imageOffset: 160
  }),
  methods: {
    handleScroll (e: any) {
      const newValue = 160 - (e.target.documentElement.scrollTop / 5);
      this.imageOffset = newValue >= 0 ? newValue : 0;
    }
  },
  created() {
    window.addEventListener('scroll', this.handleScroll);
  },
  destroyed () {
    window.removeEventListener('scroll', this.handleScroll);
  },
});
</script>

<style lang="scss" scoped>
#home-container {
  height: 300vh;
}

#awreatha-container {
  position: relative;
  width: 100%;
  text-align: center;
  height: calc(100vh - 80px);
  min-height: 400px;
  padding: 0 60px;

  img {
    position: absolute;
    left: 50%;
    transform: translateX(-50%);
    width: 100%;
    max-width: 600px;
  }
}

#us-container {
  width: 100%;
  height: 600px;
}
</style>
