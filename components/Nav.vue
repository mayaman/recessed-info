<!-- Please remove this file from your project -->
<template>
  <nav>
    <ul class="nav-right">
      <li><NuxtLink to="/">✧ Home ✧</NuxtLink></li>
      <li><NuxtLink to="/about">✧ About ✧</NuxtLink></li>
      <li><NuxtLink to="/artists">✧ Artists ✧</NuxtLink></li>
      <li><NuxtLink to="/contact">✧ Contact ✧</NuxtLink></li>
    </ul>
  </nav>
</template>


<style scoped>
nav {
  justify-content: space-between;
  align-content: center;
  color: black;
  text-align: center;
}

ul {
  list-style: none;
  display: flex;
  font-family: sans-serif;
  font-size: 18px;
  line-height: 24px;
  justify-content: center;
  text-align: center;
  /* margin: 50px 0px; */
}

li {
  padding: 0px 50px;
}

a {
  text-decoration: none;
  color: black;
}

a:hover {
  color: blue;
}

a.nuxt-link-exact-active {
  color: blue;
}
</style>
