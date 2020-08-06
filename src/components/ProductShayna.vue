<template>
  <!-- Product Shop Section Begin -->
  <section class="product-shop spad page-details">
    <div class="container">
      <div class="row">
        <div class="col-lg-12">
          <div class="row">
            <div class="col-lg-6">
              <div class="product-pic-zoom">
                <img class="product-big-img" :src="default_img" alt />
              </div>
              <div class="product-thumbs">
                <carousel
                  class="product-thumbs-track ps-slider"
                  :items="3"
                  :dots="false"
                  :nav="false"
                >
                  <div
                    class="pt"
                    @click="changeImage(active[0])"
                    :class="active[0] == default_img ? 'active' : ''"
                  >
                    <img src="img/mickey1.jpg" alt />
                  </div>

                  <div
                    class="pt"
                    @click="changeImage(active[1])"
                    :class="active[1] == default_img ? 'active' : ''"
                  >
                    <img src="img/mickey2.jpg" alt />
                  </div>

                  <div
                    class="pt"
                    @click="changeImage(active[2])"
                    :class="active[2] == default_img ? 'active' : ''"
                  >
                    <img src="img/mickey3.jpg" alt />
                  </div>

                  <div
                    class="pt"
                    @click="changeImage(active[3])"
                    :class="active[3] == default_img ? 'active' : ''"
                  >
                    <img src="img/mickey4.jpg" alt />
                  </div>
                </carousel>
              </div>
            </div>
            <div class="col-lg-6 text-left">
              <div class="product-details">
                <div class="pd-title">
                  <span>oranges</span>
                  <h3>Pure Pineapple</h3>
                </div>
                <div class="pd-desc">
                  <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Corporis, error officia. Rem aperiam laborum voluptatum vel, pariatur modi hic provident eum iure natus quos non a sequi, id accusantium! Autem.</p>
                  <p>
                    Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quam possimus quisquam animi, commodi, nihil voluptate nostrum neque architecto illo officiis doloremque et corrupti cupiditate voluptatibus error illum. Commodi expedita animi nulla aspernatur.
                    Id asperiores blanditiis, omnis repudiandae iste inventore cum, quam sint molestiae accusamus voluptates ex tempora illum sit perspiciatis. Nostrum dolor tenetur amet, illo natus magni veniam quia sit nihil dolores.
                    Commodi ratione distinctio harum voluptatum velit facilis voluptas animi non laudantium, id dolorem atque perferendis enim ducimus? A exercitationem recusandae aliquam quod. Itaque inventore obcaecati, unde quam
                    impedit praesentium veritatis quis beatae ea atque perferendis voluptates velit architecto?
                  </p>
                  <h4>$495.00</h4>
                </div>
                <div class="quantity">
                  <router-link to="/cart">
                    <a href="" class="primary-btn pd-cart">Add To Cart</a>
                  </router-link>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
  <!-- Product Shop Section End -->
</template>

<script>
import carousel from "vue-owl-carousel";

export default {
  name: "Productshayna",
  components: {
    carousel
  },
  data() {
    return {
      default_img: "img/mickey1.jpg",
      active: [
        "img/mickey1.jpg",
        "img/mickey2.jpg",
        "img/mickey3.jpg",
        "img/mickey4.jpg"
      ]
    };
  },
  methods: {
    changeImage(urlImage) {
      this.default_img = urlImage;
    }
  }
};
</script>

<style scoped>
.product-thumbs .pt {
  margin-right: 12px;
  margin-left: 12px;
}
</style>