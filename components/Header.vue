<template>
  <header class="screen-container aok-flex justify-end align-center">
    <transition name="slide-fade" mode="out-in">
      <template v-if="mobile">
        <div class="hamburger" key="mobile-menu">
          <div></div>
          <div></div>
          <div></div>
        </div>
      </template>
      <template v-else>
        <div key="menu">
          <button class="primary text mr-10 bold">Our Story</button>
          <button class="primary text mr-10 bold">The Proposal</button>
          <button class="primary text mr-10 bold">The Venue</button>
          <button class="primary text mr-10 bold">Gryff's Toughts</button>
          <button class="primary text mr-10 bold">Order of the day</button>
          <button class="primary bold">RSVP</button>
        </div>
      </template>
    </transition>
  </header>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  data: () => ({
    width: 0,
  }),
  methods: {
    handleResize() {
      this.width = window.innerWidth;
    },
  },
  computed: {
    mobile() {
      return this.width < 760;
    },
  },
  created() {
    window.addEventListener("resize", this.handleResize);
    this.handleResize();
  },
  destroyed() {
    window.removeEventListener("resize", this.handleResize);
  },
});
</script>

<style lang="scss" scoped>
header {
  height: 80px;
  padding: 0 60px;
}

.hamburger {
  position: relative;
  height: 40px;

  div {
    position: absolute;
    left: 0;
    height: 2px;
    width: 40px;
    background-color: var(--aok-cornflower);

    &:first-of-type {
      top: 0;
    }

    &:nth-of-type(1) {
      top: 19px;
    }

    &:last-of-type {
      bottom: 0;
    }
  }
}
</style>