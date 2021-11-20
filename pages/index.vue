<template>
  <div>
    <Header></Header>

    <Nav></Nav>
    <main>
      <div style="padding: 62.5% 0 0 0; position: relative">
        <iframe
          src="https://player.vimeo.com/video/561366546?h=be1b99314c&title=0&autoplay=1&byline=0&portrait=0"
          style="position: absolute; top: 0; left: 0; width: 100%; height: 100%"
          frameborder="0"
          allow="autoplay; fullscreen; picture-in-picture"
          allowfullscreen
        ></iframe>
      </div>

      <br />
      <div class="copy">
        <p>
          <span class="italic"> Recessed</span>, by Heidi Latsky and Maya Man,
          explores the emotional potential of engaging with the web browser
          through a series of movement-driven vignettes.
        </p>
        <p>
          Pop-up windows choreographed to appear in specific configurations
          capture the intimacy of bodies moving within a virtual space. The
          site, a custom-coded movement palimpsest by Man, layers recorded
          performances to highlight diverse narratives in motion.
        </p>
      </div>

      <br />
      <!-- <img
        class="preview"
        src="https://cdn.shopify.com/s/files/1/0068/0486/5082/files/05_Sabrina_1024x1024.gif?v=1627071530"
        alt="Sabrina moving in a large browser window on screen"
      />
      <img
        class="preview"
        src="https://storage.googleapis.com/recessed-assets/documentation/02_Jillian.gif"
        alt="Five pop up windows featuring Jillian dancing outside under a blue sky"
      /> -->
    </main>
  </div>
</template>

<script>
export default {};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Monsieur+La+Doulaise&display=swap");

body {
  padding: 0px;
  font-family: sans-serif;
  font-size: 18px;
  line-height: 24px;
  margin: 0px;
}

.bold {
  font-weight: bold;
}

.cursive {
  font-family: "Monsieur La Doulaise", cursive;
}

.italic {
  font-style: italic;
}

main {
  padding: 50px 0px;
  text-align: center;
  width: 50%;
  margin: auto;
  display: block;
}

header {
  text-align: center;
  padding: 25px 0px;
  font-weight: normal;
}

h1 {
  text-align: left;
  font-size: 172px;
  line-height: 225px;
  font-weight: normal;
  margin: 0px;
  text-align: center;
  height: auto;
}

h2 {
  font-weight: normal;
  font-size: 18px;
  line-height: 24px;
}

iframe {
  width: 100%;
}

::selection {
  color: white;
  background: blue;
}

.copy {
  text-align: left;
  width: 100%;
  margin: auto;
  display: block;
}

img.preview {
  max-width: 100%;
  min-width: 90%;
  display: block;
  margin: auto;
}

a {
  color: black;
}

a:hover {
  color: blue;
}
</style>