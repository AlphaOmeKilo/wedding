2<template>
  <div>
    <div
      id="awreatha-container"
      class="uk-section uk-padding-remove-top uk-padding-remove-bottom uk-flex uk-flex-middle"
    >
      <div class="uk-container uk-width-1-1">
        <div class="uk-grid uk-flex-center">
          <div class="uk-width-3-4 uk-width-2-3@m uk-width-1-2@l">
            <img
              uk-scrollspy="cls:uk-animation-fade; delay:1000"
              data-src="~/assets/images/awreatha.png"
              alt="awreatha"
              uk-img
            />
          </div>
        </div>
      </div>
    </div>
    <div id="menu" class="uk-section uk-flex uk-flex-center">
      <nav class="uk-navbar-container" uk-navbar>
        <div class="uk-navbar-center">
          <ul
            class="uk-navbar-nav uk-flex-wrap uk-child-width-1-1 uk-child-width-auto@m"
          >
            <li><a href="#our-story" class="lsbold">Our Story</a></li>
            <li><a href="#the-proposal" class="lsbold">The Proposal</a></li>
            <li><a href="#the-venue" class="lsbold">The Venue</a></li>
            <li>
              <a href="#gryffs-thoughts" class="lsbold">Gryff's Thoughts</a>
            </li>
            <li><a href="#order" class="lsbold">Order of the day</a></li>
          </ul>
        </div>
      </nav>
    </div>
    <div id="our-story" class="uk-section">
      <div class="uk-container">
        <div class="uk-grid">
          <div class="uk-width-1-1 uk-width-2-5@m">
            <img
              uk-scrollspy="cls:uk-animation-slide-bottom-small; offset-top:-200"
              data-src="~/assets/images/colourFam.jpeg"
              alt="family"
              uk-img
            />
          </div>
          <div class="uk-width-1-1 uk-width-3-5@m">
            <div class="text-content uk-padding-small">
              <h2
                class="calligraphy"
                uk-scrollspy="cls:uk-animation-slide-right-small; offset-top:-260"
              >
                Our Story
              </h2>
              <p
                uk-scrollspy="cls:uk-animation-slide-right-small; offset-top:-230; delay: 250"
              >
                On the 22nd July 2018 at the Griffin Pub in Caverham, Reading,
                Alex and Ceri had a first date which was 7 hours long. It left
                the waiting staff wondering if they would ever leave the
                restaurant, the car parking inpectors no choice but to issue
                tickets and both Alex and Ceri with the sense that this first
                date was the start of something special. Fast forward through
                Ceri's graduation as a midwife, 2 new jobs for Alex, a home
                together with Gryff and 1 global pandemic, Alex got down onto
                one knee and asked Ceri to marry him.
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div id="the-proposal" class="uk-section">
      <div class="uk-container">
        <div class="uk-grid">
          <div class="uk-width-1-1 uk-width-3-5@m uk-flex-last uk-flex-first@s">
            <div class="text-content uk-padding-small">
              <h2
                class="calligraphy"
                uk-scrollspy="cls:uk-animation-slide-left-small; offset-top:-260"
              >
                The Proposal
              </h2>
              <p
                uk-scrollspy="cls:uk-animation-slide-left-small; offset-top:-230; delay:250"
              >
                On the 22nd July 2018 at the Griffin Pub in Caverham, Reading,
                Alex and Ceri had a first date which was 7 hours long. It left
                the waiting staff wondering if they would ever leave the
                restaurant, the car parking inpectors no choice but to issue
                tickets and both Alex and Ceri with the sense that this first
                date was the start of something special. Fast forward through
                Ceri's graduation as a midwife, 2 new jobs for Alex, a home
                together with Gryff and 1 global pandemic, Alex got down onto
                one knee and asked Ceri to marry him.
              </p>
            </div>
          </div>
          <div class="uk-width-1-1 uk-width-2-5@m">
            <img
              uk-scrollspy="cls:uk-animation-slide-bottom-small; offset-top:-200"
              data-src="~/assets/images/colourFam.jpeg"
              alt="family"
              uk-img
            />
          </div>
        </div>
      </div>
    </div>
    <div id="the-venue" class="uk-section uk-padding-remove-bottom">
      <div
        class="uk-height-medium uk-flex uk-flex-center uk-flex-middle uk-background-cover uk-light"
        data-src="~/assets/images/aisle.jpg"
        uk-parallax="bgy: -50"
        uk-img
      ></div>
    </div>
    <div class="uk-section">
      <div class="uk-container">
        <h2
          class="calligraphy uk-text-center"
          uk-scrollspy="cls:uk-animation-slide-bottom-small; offset-top:-200"
        >
          The Castle Hotel
        </h2>
      </div>
    </div>
    <div id="gryffs-thoughts" class="uk-section">
      <div class="uk-container">
        <div class="uk-grid">
          <div class="uk-width-1-1 uk-width-2-5@m">
            <img
              uk-scrollspy="cls:uk-animation-slide-bottom-small; offset-top:-200"
              data-src="~/assets/images/gryff1.jpeg"
              alt="family"
              uk-img
            />
          </div>
          <div class="uk-width-1-1 uk-width-3-5@m">
            <div class="text-content uk-padding-small">
              <h2
                class="calligraphy"
                uk-scrollspy="cls:uk-animation-slide-right-small; offset-top:-260"
              >
                Gryff's Thoughts
              </h2>
              <p
                uk-scrollspy="cls:uk-animation-slide-right-small; offset-top:-230; delay: 250"
              >
                On the 22nd July 2018 at the Griffin Pub in Caverham, Reading,
                Alex and Ceri had a first date which was 7 hours long. It left
                the waiting staff wondering if they would ever leave the
                restaurant, the car parking inpectors no choice but to issue
                tickets and both Alex and Ceri with the sense that this first
                date was the start of something special. Fast forward through
                Ceri's graduation as a midwife, 2 new jobs for Alex, a home
                together with Gryff and 1 global pandemic, Alex got down onto
                one knee and asked Ceri to marry him.
              </p>
              <p
                uk-scrollspy="cls:uk-animation-slide-left-small; offset-top:-230; delay:2000"
              >
                Also, sausages.
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div id="order" class="uk-section">
      <div class="uk-container">
        
        <div class="uk-grid uk-flex-center">
          <div class="uk-card uk-card-default uk-card-body uk-width-3-4">
            <h2 class="calligraphy uk-text-center">Order of the day</h2>
            <div class="uk-grid">
              <h3 class="uk-width-2-5 calligraphy">1pm</h3>
              <div class="uk-width-3-5 uk-flex uk-flex-middle">Guest arrival for drinks reception</div>
              <h3 class="uk-width-2-5 calligraphy">1.45pm</h3>
              <div class="uk-width-3-5 uk-flex uk-flex-middle">Guests take their seats for the ceremony</div>
              <h3 class="uk-width-2-5 calligraphy">2pm</h3>
              <div class="uk-width-3-5 uk-flex uk-flex-middle">Ceremony begins</div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({});
</script>

<style lang="scss" scoped>
#awreatha-container {
  min-height: 100vh;
}

#menu {
  position: relative;

  &:after {
    content: "";
    display: block;
    position: absolute;
    top: 50%;
    left: 0;
    right: 0;
    height: 2px;
    background-color: var(--aok-shadow);
  }

  .uk-navbar-container {
    background-color: var(--aok-white);
    z-index: 10;
  }
}
</style>
