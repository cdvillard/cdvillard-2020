<template>
  <footer>
    {{ year }}
  </footer>
</template>

<script>
export default {
  data() {
    return { year: new Date().getFullYear() };
  },
};
</script>
