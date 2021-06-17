<template>
  <header id="header" class="fixed-top d-flex align-items-center">
    <div
      class="container-fluid container-xl d-flex align-items-center justify-content-lg-between"
    >
      <h1 class="logo me-auto me-lg-0">
        <!-- Uncomment below if you prefer to use an image logo -->
        <!-- <a href="index.html" class="logo me-auto me-lg-0"><img src="assets/img/logo.png" alt="" class="img-fluid"></a>-->
        <nuxt-link to="/">Partners Kuphela</nuxt-link>
      </h1>
      <div class="d-flex align-items-center">
        <nav-bar />
        <get-quote-btn />
      </div>
    </div>
  </header>
</template>

<script>
import GetQuoteBtn from "./GetQuoteBtn.vue";
import NavBar from "./NavBar.vue";

export default { components: { GetQuoteBtn, NavBar } };
</script>

<style>
#header {
  background: rgba(12, 11, 9, 0.6);
  border-bottom: 1px solid rgba(12, 11, 9, 0.6);
  transition: all 0.5s;
  z-index: 997;
  padding: 15px 0;
  top: 40px;
}

#header.header-scrolled {
  top: 0;
  background: rgba(0, 0, 0, 0.85);
  border-bottom: 1px solid #37332a;
}

#header .logo {
  font-size: 28px;
  margin: 0;
  padding: 0;
  line-height: 1;
  font-weight: 300;
  letter-spacing: 1px;
  text-transform: uppercase;
  font-family: "Poppins", sans-serif;
}

#header .logo a {
  color: #fff;
}

#header .logo img {
  max-height: 40px;
}
</style>
