<template>
  <div class="layout">
    <Header></Header>
    <slot />
    <Footer></Footer>
  </div>
</template>

<script>
import Header from "./../components/header";
import Footer from "./../components/footer";
export default {
  components: {
    Header,
    Footer
  }
};
</script>

<style lang="scss">
body {
  font-family: -apple-system, system-ui, BlinkMacSystemFont, "Segoe UI", Roboto,
    "Helvetica Neue", Arial, sans-serif;
  margin: 0;
  padding: 0;
  line-height: 1.5;
  /* width: 100vw; */
  .layout {
  }
}
</style>
