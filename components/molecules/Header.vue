<template>
  <div class="container">
    <div class="header">
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
  components: { LogoIcon },
};
</script>

<style lang="scss" scoped>
.container {
  .header {
    display: flex;
    flex: 1;
    margin: 32px 0 0;
    justify-content: space-between;

    .logo-contianer {
      position: relative;
      margin-left: 32px;
    }

    .nav-menu {
      display: flex;
      position: relative;
      margin-right: 32px;

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
