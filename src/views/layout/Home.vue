<template>
  <div class="home">
    <list-menu></list-menu>
    <div :class="{ 'main-app': true, 'menu-unfold': $store.state.collapsed }">
      <slider-nav></slider-nav>
    </div>
  </div>
</template>

<script>
import listMenu from './components/menu.vue';
import sliderNav from './components/sliderNav.vue';

export default {
  components: {
    listMenu,
    sliderNav,
  },

};
</script>
<style lang="less">
@import url("~@/assets/css/home.less");
</style>
