<template>
  <span class="wrapper img-wrap">
    <img
      class="me"
      src="https://cdn.khaleelgibran.com/IMG_20201231_221159_770.jpg"
      alt="A picture of me."
      title="That's me."
    />
  </span>
</template>

<script>
export default {
  name: "Me",
};
</script>

<style scoped>
/*  */

.me {
  width: 20vw;
  display: block !important;
  border-radius: 5px;
  box-shadow: 0 6.2px 5.3px rgba(0, 0, 0, 0.048),
    0 20.8px 17.9px rgba(0, 0, 0, 0.072), 0 93px 80px rgba(0, 0, 0, 0.12);
  /* border: 5px solid #7952B3; */
}

.image-wrap {
  padding: 0px !important;
  display: block;
}
</style>