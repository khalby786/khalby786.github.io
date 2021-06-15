<template>
  <header>
    <p><a href="https://blog.khaleelgibran.com" target="_blank">blog</a></p>
    <p><a href="https://art.khaleelgibran.com" target="_blank">art</a></p>
    <p><a href="https://github.com/khalby786" target="_blank">github</a></p>
  </header>
  <div id="nav">
    <div id="top">
      <div id="progress-indicator"></div>
    </div>

    <Banner v-if="showBanner === true" />
    <!-- <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link> -->
  </div>

  <transition name="fade" mode="out-in">
    <router-view />
  </transition>

  <Footer />
</template>

<script>
import Banner from "@/components/Banner.vue";
import Footer from "@/components/Footer.vue";

export default {
  name: "App",
  components: {
    Footer,
    Banner,
  },
  data: function () {
    return {
      showBanner: false,
    };
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Fira+Code:wght@400;700&family=Inter:wght@300;400;500;700;900&display=swap");

body {
  max-width: 700px;
  margin: 0 auto;
  padding-top: 100px;
  padding-bottom: 10px;
  font-family: "Inter", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto,
    Oxygen, Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif;
  letter-spacing: -0.004em;
  font-kerning: normal;
  font-variant-ligatures: contextual common-ligatures;
  font-feature-settings: "kern", "liga", "calt";
  height: auto;
  --block-shadow-color: #ff6b6b;
  color: black;
}

::selection {
  background-color: cyan;
  color: black;
}

h1 {
  font-family: "Fira Code", "Fira Mono", monospace;
  font-size: 5vw;
}

h2,
h3,
h4,
h5,
h6 {
  font-family: "Fira Code", "Fira Mono", monospace;
  color: #AA2EE6;
}

a {
  color: #6b17e6;
  transition: opacity 0.2s;
  isolation: isolate;
}

#top {
  background: #ff6b6b;
  position: fixed;
  z-index: 999;
}

#top {
  left: 0;
  right: 0;
  height: 5px;
  top: 0;
}

header {
  position: absolute;
  top: 5px;
  left: 0px;
  right: 0px;
  bottom: 0px;
  background-color: #9c6bff;
  color: white;
  height: 30px;
  padding-left: 10px;
  vertical-align: middle;
  font-weight: bold;
  padding-top: 5px;
  /* padding-bottom: 5px; */
}

header > p {
  display: inline-block;
  margin-right: 10px;
  margin-top: 0px;
  margin-bottom: 0px;
  vertical-align: middle;
}

header > p > a {
  text-decoration: none;
  color: inherit;
}

/* footer {
  position: absolute;
  left: 0px;
  right: 0px;
  bottom: 0px;
  width: 100%;
  height: 200px;
  background-color:  #ff6b6b;
  overflow: auto;
} */

.fade-enter-active,
.fade-leave-active {
  transition-duration: 0.3s;
  transition-property: opacity;
  transition-timing-function: ease;
}

.fade-enter,
.fade-leave-active {
  opacity: 0;
}
</style>
