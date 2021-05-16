<template>
  <header>
    <p
      >🚧 my <a href="https://blog.khaleelgibran.com">blog</a> will be down for a few days, maintenance in progress!</p
    >
  </header>
</template>

<script>
export default {
  name: "Banner",
};
</script>

<style scoped>
header {
  position: absolute;
  top: 5px;
  left: 0px;
  right: 0px;
  width: 100%;
  background-color: yellow;
  font-family: "Fira Code", "IBM Plex Mono", monospace;
  text-align: center;
  min-height: 40px;
  padding-bottom: 5px;
  vertical-align: middle;
  margin-bottom: 20px;
}

header > p {
  vertical-align: middle;
  display: inline-block;
  color: #4B0082;
}

header::after {
    content: ""
}
</style>