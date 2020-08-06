 <template>
  <!-- Breadcrumb Section Begin -->
  <div class="breacrumb-section text-left">
    <div class="container">
      <div class="row">
        <div class="col-lg-12">
          <div class="breadcrumb-text product-more">
            <router-link to="/">
              <i class="fa fa-home"></i> Home
            </router-link>
            <span>Detail</span>
          </div>
        </div>
      </div>
    </div>
  </div>
  <!-- Breadcrumb Section End -->
</template>

<script>
export default {
  name: "Breadcrumb"
};
</script>