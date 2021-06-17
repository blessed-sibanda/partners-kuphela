<template>
  <div id="topbar" class="d-flex align-items-center fixed-top">
    <div
      class="container d-flex justify-content-center justify-content-md-between"
    >
      <div class="contact-info d-flex align-items-center">
        <i class="bi bi-phone d-flex align-items-center"
          ><span>+263 78 303 9225</span></i
        >
        <i class="bi bi-clock d-flex align-items-center ms-4"
          ><span> Mon-Fi: 8AM - 5PM</span></i
        >
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
#topbar {
  height: 40px;
  font-size: 14px;
  transition: all 0.5s;
  z-index: 996;
}

#topbar.topbar-scrolled {
  top: -40px;
}

#topbar .contact-info i {
  font-style: normal;
  color: var(--main-color);
}

#topbar .contact-info i span {
  padding-left: 5px;
  color: #fff;
}
</style>
