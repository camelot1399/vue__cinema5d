<template>
  <div className="wrapper">
    <HeaderComponent />

    <router-view />
  </div>
</template>

<script>
import HeaderComponent from '@/components/header';

export default {
  name: "MainLayout",
  components: {
    HeaderComponent
  }
}
</script>

<style>

</style>
