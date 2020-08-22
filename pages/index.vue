<template>
  <div class="">
    <section class="section">
      <Text-Image />
    </section>
    <section data-aos="fade-in" class="section">
      <CompaniesSection />
    </section>
  </div>
</template>

<script>
import TextImage from "../components/molecules/TextImage";
import CompaniesSection from "../components/molecules/CompaniesSection";

export default {
  components: {
    CompaniesSection,
    TextImage
  }
};
</script>

<style lang="scss" scoped>
.section {
  padding: 50px 0;
  // overflow: hidden;

  &:first-child {
    padding: 100px 0 50px;
  }
}
</style>
