<template>
  <div class="container grid">
    <div class="header col-desk-12">
      <div class="logo-contianer">
        <nuxt-link to="/">
          <LogoIcon class="logo" />
        </nuxt-link>
      </div>
      <div class="nav-menu">
        <div class="nav-menu__item">
          <nuxt-link to="/help">
            <div class="link">Help</div>
          </nuxt-link>
        </div>
        <div class="nav-menu__item">
          <nuxt-link to="/faq">
            <div class="link">FAQ</div>
          </nuxt-link>
        </div>
        <div class="nav-menu__item">
          <nuxt-link to="/about">
            <div class="link">About</div>
          </nuxt-link>
        </div>
        <div class="nav-menu__item">
          <nuxt-link to="/preorder">
            <div class="link--bold-red">Preorder</div>
          </nuxt-link>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import LogoIcon from "assets/svg/logo.svg";

export default {
  components: { LogoIcon }
};
</script>

<style lang="scss" scoped>
.container {
  .logo-contianer {
    left: -50%;
  }

  .header {
    display: flex;
    flex: 1;
    margin: 32px 0 0;
    justify-content: space-between;

    .nav-menu {
      display: flex;

      &__item {
        margin-left: 20px;
      }

      .link {
        &--bold-red {
          margin-left: 60px;
          color: $color-red;
          font-family: $font-roag-bold;
        }
      }
    }
  }
}
</style>
