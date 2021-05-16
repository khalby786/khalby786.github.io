<template>
  <div class="home">
    <span class="hidden-text">pretend you didn't see this</span>
    <Me />
    <h1 id="heading">Khaleel Gibran</h1>
    <p id="tagline">a fourteen-year-old alien from out there...</p>
    <h3>who am i?</h3>
    <p>
      I am a fourteen-year-old web designer/developer from India. I started
      coding since I was 11, and I've been creating clean and really cool
      websites ever since! I <b>do not</b> fix printers and I
      <b>will not</b> hack Facebook for you.
    </p>
    <h5>fun facts</h5>
    <ul>
      <li>I like donuts.</li>
      <li>I really like donuts.</li>
      <li>I really, really like donuts.</li>
      <li>I create <a href="https://instagram.com/khalby786">3D</a> <a href="https://art.khaleelgibran.com">art</a> when I'm not doing other stuff.</li>
      <li>I write a <a href="https://blog.khaleelgibran.com">blog</a>!</li>
      <li><b>Favourite OS</b> Ubuntu</li>
      <li>
        <b>Favourite movie </b>
        <a href="https://en.wikipedia.org/wiki/Bumblebee_(film)">Bumblebee</a>
      </li>
      <li>
        <b
          ><a href="https://www.youtube.com/watch?v=dQw4w9WgXcQ"
            >Favourite song(s) </a
          ></b
        >
        <a href="https://www.youtube.com/watch?v=Ow_PNMtMGhU"
          >Roadtrip by Dream ft. PmBata</a
        >,
        <a href="https://www.youtube.com/watch?v=7C2z4GqqS5E"
          >Fake Love by BTS</a
        >
      </li>
    </ul>
    <h5>tech</h5>
    <Tech />
    <br /><br />
    <h5>social</h5>
    <span
      >i'm <code>@khalby786</code> on all social platforms, except for
      <a href="https://dsc.bio/khalby786">discord</a> 🤷</span
    >
    <Social />
    <br /><br />
    <h5>projects</h5>
    <Projects />
    <Footer />
  </div>
</template>

<script>
import Me from "@/components/Me.vue";
import Tech from "@/components/Tech.vue";
import Social from "@/components/Social.vue";
import Projects from "@/components/Projects.vue";

export default {
  name: "Home",
  components: {
    Me,
    Tech,
    Social,
    Projects,
  },
};
</script>

<style scoped>
h1 {
  margin-bottom: 0px;
}

#tagline {
  text-align: center;
  margin-bottom: 200px;
  max-width: 100% !important;
}

.hidden-text {
  color: white;
  margin: 0px;
}

p {
  max-width: 500px;
}

@media only screen and (max-width: 500px) {
  .home {
    margin-top: 50px;
  }
}
</style>