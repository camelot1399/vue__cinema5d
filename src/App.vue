<template>
  <div id="app">
   <component :is="isLayout">
     <router-view />
   </component>
  </div>
</template>
<script>
export default {
  computed: {
    isLayout() {
      const LayoutName = this.$route.meta.layout || 'Empty';
      return () => import(`@/layouts/${LayoutName}Layout.vue`)
    }
  }
}
</script>

<style lang="scss">
@import './assets/scss/style.scss';
</style>
