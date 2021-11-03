<template>
  <!-- <Tutorial/> -->
  <div>
    <header>
      <h1 class="cursive">Recessed</h1>
      <h2>Choreographing the browser, by Heidi Latsky and Maya Man</h2>
    </header>
    <Nav></Nav>
    <main>
      <iframe
        src="https://player.vimeo.com/video/561366546?h=be1b99314c&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479"
        width="840"
        height="525"
        frameborder="0"
        allow="autoplay; fullscreen; picture-in-picture"
        allowfullscreen
        title="Recessed (preview)"
      ></iframe>
<br>
<br></br>
      <div class="copy">
        <span> Recessed </span>
        explores the emotional impact of engaging with the browser through a
        series of movement-driven vignettes. Choreographed pop-up windows in
        various configurations capture the intimacy of bodies moving within a
        virtual space. The site, custom-coded by Man, layers recorded
        performances that highlight diverse narratives in motion.
      </div>
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
  width: 65%;
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
  max-width: 840px;
  margin: auto;
  display: block;
}

a {
  color: black;
}


a:hover {
  color: blue;
}
</style>