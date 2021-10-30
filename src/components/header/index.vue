<template>
  <div class="header">
    <div class="header__container">
      <div class="header__body">
        <LogoComponent />

        <UserBlockComponent />
      </div>
    </div>
  </div>
</template>

<script>
import LogoComponent from "@/components/header/logo.vue";
import UserBlockComponent from "@/components/header/UserBlock.vue";
export default {
  components: {
    LogoComponent,
    UserBlockComponent
  }
}
</script>

<style lang="scss">
@import '@/assets/scss/config-style.scss';

.header {
  background-color: $menuBackground;
  color: $menuColor;
  &__container {
    width: $md1;
  }
  &__body {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 10px;
  }
}

.logoBlock {
  display: flex;
  align-items: center;
  flex-direction: column;
  &__img {
    width: 100px;
    height: 100px;
  }
  &__name {
    font-size: 20px;
    color: white;
  }
}
</style>
