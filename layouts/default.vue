<template>
  <div>
    <top-bar />
    <site-header />
    <Nuxt />
  </div>
</template>

<script>
import TopBar from "../components/TopBar.vue";
import SiteHeader from "../components/SiteHeader.vue";
export default {
  components: { TopBar, SiteHeader }
};
</script>

<style>
:root {
  --main-color: #d9ba85;
  --link-color: #cda45e;
}
body {
  font-family: "Open Sans", sans-serif;
  background: #0c0b09;
  color: #fff;
}

a {
  color: var(--link-color);
  text-decoration: none;
}

a:hover {
  color: var(--main-color);
  text-decoration: none;
}

h1,
h2,
h3,
h4,
h5,
h6 {
  font-family: "Playfair Display", serif;
}
</style>
