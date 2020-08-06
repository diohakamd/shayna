<template>
  <!-- Partner Logo Section Begin -->
  <div class="partner-logo">
    <div class="container">
      <carousel
        class="logo-carousel"
        :loop="true"
        :autoplay="true"
        :items="5"
        :dots="false"
        :nav="false"
      >
        <div class="logo-item">
          <div class="tablecell-inner">
            <img src="img/logo-carousel/logo-1.png" />
          </div>
        </div>
        <div class="logo-item">
          <div class="tablecell-inner">
            <img src="img/logo-carousel/logo-2.png" />
          </div>
        </div>
        <div class="logo-item">
          <div class="tablecell-inner">
            <img src="img/logo-carousel/logo-3.png" />
          </div>
        </div>
        <div class="logo-item">
          <div class="tablecell-inner">
            <img src="img/logo-carousel/logo-4.png" />
          </div>
        </div>
        <div class="logo-item">
          <div class="tablecell-inner">
            <img src="img/logo-carousel/logo-5.png" />
          </div>
        </div>
      </carousel>
    </div>
  </div>
  <!-- Partner Logo Section End -->
</template>

<script>
import carousel from "vue-owl-carousel";

export default {
  name: "PartnerShayna",
  components: {
    carousel
  }
};
</script>