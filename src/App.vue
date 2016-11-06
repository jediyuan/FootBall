<template>
  <div>
    <router-view class="view" transition="test" transition-mode="out-in" keep-alive></router-view>
  </div>
</template>
<script>
  module.exports={};
</script>
<style>
  .view {
    position: absolute;
    height: 100%;
    min-width: 100%;
    transition: all .5s ease;
  }
  .test-enter, .test-leave {
    opacity: 0;
    transform: translate3d(10px, 0, 0);
  }
  .v-link-active {
    color: red;
  }
  [v-cloak] {
    display: none;
  }
</style>