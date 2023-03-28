<template>

</template>

<script>
import feather from "feather-icons";
export default {
  components: {},
  data: () => {
    return {
      userScrollPosition: 0,
    };
  },
  computed: {
    isScrolled() {
      return this.userScrollPosition > 100;
    },
  },
  mounted() {
    window.addEventListener("scroll", this.updateScrollPosition);
    feather.replace();
  }
}
</script>

<style scoped>

</style>
