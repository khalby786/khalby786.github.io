<template>
  <div id="tech">
    <p>
      <i class="devicon-html5-plain colored"></i>
      <br /><br />
      HTML
    </p>
    <p>
      <i class="devicon-css3-plain colored"></i>
      <br /><br />
      CSS
    </p>
    <p>
      <i class="devicon-javascript-plain colored"></i>
      <br /><br />
      JavaScript
    </p>
    <p>
      <i class="devicon-jquery-plain colored"></i>
      <br /><br />
      jQuery
    </p>
    <p>
      <i class="devicon-nodejs-plain colored"></i>
      <br /><br />
      NodeJS
    </p>
    <p>
      <i class="devicon-express-original colored"></i>
      <br /><br />
      Express
    </p>
    <p>
      <i class="devicon-vuejs-plain colored"></i>
      <br /><br />
      VueJS
    </p>
    <p>
      <i class="devicon-mongodb-plain colored"></i>
      <br /><br />
      MongoDB
    </p>
    <p>
      <i class="devicon-git-plain colored"></i>
      <br /><br />
      Git
    </p>
    <p>
      <i class="devicon-typescript-plain colored"></i>
      <br /><br />
      <span style="color: orange">TypeScript</span>
    </p>
  </div>
</template>

<script>
export default {
  name: "Tech",
};
</script>

<style scoped>
#tech {
  display: grid;
  grid-template-columns: repeat(5, 100px);
  grid-template-rows: repeat(2, 1fr);
  grid-column-gap: 0px;
  grid-row-gap: 10px;
  text-align: center;
  overflow: auto;
}

[class~="colored"] {
  font-size: 30px;
  isolation: isolate;
}
</style>