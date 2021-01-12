<template>
  <div class="pb-10">
    <div id="home-container" class="screen-container">
      <div id="awreatha-container">
        <div class="aok-flex justify-center">
          <h2 class="calligraphy timedate black--text">
            30 May 2021 | The Castle Hotel
          </h2>
        </div>
        <div class="aok-flex justify-center mt-7">
          <button class="primary lsbold">Watch the ceremony here</button>
        </div>
        <div id="awreatha" :style="`bottom: -${imageOffset}px`">
          <img src="~/assets/images/awreatha.png" />
          <div id="alex" class="calligraphy">A</div>
          <div id="and" class="calligraphy">&#38;</div>
          <div id="ceri" class="calligraphy">C</div>
        </div>
      </div>
      <div id="our-story" class="aok-flex">
        <div id="ca-image"></div>
        <div class="section-content pa-10">
          <h3 class="calligraphy mb-10">Our Story</h3>
          <p>
            On the 22nd July 2018 at the Griffin Pub in Caverham, Reading, Alex
            and Ceri had a first date which was 7 hours long. It left the
            waiting staff wondering if they would ever leave the restaurant, the
            car parking inpectors no choice but to issue tickets and both Alex
            and Ceri with the sense that this first date was the start of
            something special. Fast forward through Ceri's graduation as a
            midwife, 2 new jobs for Alex, a home together with Gryff and 1
            global pandemic, Alex got down onto one knee and asked Ceri to marry
            him.
          </p>
        </div>
      </div>
      <div id="proposal" class="aok-flex">
        <div class="section-content pa-10">
          <h3 class="calligraphy mb-10">The Proposal</h3>
          <p>
            On the 22nd July 2018 at the Griffin Pub in Caverham, Reading, Alex
            and Ceri had a first date which was 7 hours long. It left the
            waiting staff wondering if they would ever leave the restaurant, the
            car parking inpectors no choice but to issue tickets and both Alex
            and Ceri with the sense that this first date was the start of
            something special. Fast forward through Ceri's graduation as a
            midwife, 2 new jobs for Alex, a home together with Gryff and 1
            global pandemic, Alex got down onto one knee and asked Ceri to marry
            him.
          </p>
        </div>
        <div id="ca-image"></div>
      </div>
    </div>
    <div id="venue-image"></div>
    <div id="venue" class="aok-flex justify-center">
      <h2 class="calligraphy mt-10">The Castle Hotel</h2>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  data: () => ({
    imageOffset: 160,
  }),
  methods: {
    handleScroll(e: any) {
      const newValue = 160 - e.target.documentElement.scrollTop / 3;
      this.imageOffset = newValue >= 0 ? newValue : 0;
    },
  },
  created() {
    window.addEventListener("scroll", this.handleScroll);
  },
  destroyed() {
    window.removeEventListener("scroll", this.handleScroll);
  },
});
</script>

<style lang="scss" scoped>
#awreatha-container {
  position: relative;
  z-index: 10;
  width: 100%;
  text-align: center;
  height: calc(100vh - 80px);
  min-height: 750px;
  padding: 60px 60px 0 60px;

  #awreatha {
    position: absolute;
    left: 50%;
    transform: translateX(-50%);
  }

  img {
    width: 100%;
    max-width: 600px;
  }

  #alex {
    font-size: 102px;
    font-weight: 700;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-165%, -75%);
  }

  #and {
    font-size: 48px;
    font-weight: 700;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
  }

  #ceri {
    font-size: 102px;
    font-weight: 700;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(100%, 0%);
  }

  .timedate {
    font-weight: 300;
    letter-spacing: 6px;
    margin-top: 60px;
  }
}

#next {
  height: 600px;
}

#our-story {
  height: 30vw;
  max-height: 400px;
  width: 100%;
  margin-top: 100px;

  #ca-image {
    height: 100%;
    width: 50%;
    background-image: url(~assets/images/canada.jpg);
    background-position: center center;
    background-size: cover;
  }

  .section-content {
    width: 50%;
  }
}

#proposal {
  height: 30vw;
  max-height: 400px;
  width: 100%;
  margin-top: 100px;

  #ca-image {
    height: 100%;
    width: 50%;
    background-image: url(~assets/images/canada.jpg);
    background-position: center center;
    background-size: cover;
  }

  .section-content {
    width: 50%;
  }
}

#venue-image {
  height: 50vw;
  margin-top: 100px;
  max-height: 400px;
  width: 100%;
  background-image: url(~assets/images/aisle.jpg);
  background-position: center center;
  background-size: cover;
}

#venue {
  h2 {
    font-weight: 300;
  }
}
</style>
