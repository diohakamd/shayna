<template>
  <div class="product">
    <HeaderShayna />
    <Breadcrumb />
    <ProductShayna />
    <RelatedShayna />
    <FooterShayna />
  </div>
</template>

<script>
// @ is an alias to /src
import HeaderShayna from "@/components/HeaderShayna.vue";
import ProductShayna from "@/components/ProductShayna.vue";
import Breadcrumb from "@/components/Breadcrumb.vue";
import RelatedShayna from "@/components/RelatedShayna.vue";
import FooterShayna from "@/components/FooterShayna.vue";

export default {
  name: "Product",
  components: {
    HeaderShayna,
    ProductShayna,
    Breadcrumb,
    RelatedShayna,
    FooterShayna
  }
};
</script>
