<template>
  <transition name="fade">
    <div
      v-show="modal"
      @click="showModal()"
      class="
      bg-filter bg-black bg-opacity-50
          fixed
          inset-0
          w-full
          h-full
          z-20
"></div>
    <!-- Modal contents -->>
    <main class="flex">

    </main>
  </transition>

</template>

<script>
import feather from "feather-icons";
import Button from "./reusable/Button.vue";
export default {
  props: ["showModal", "modal", "categories"],
  components: {
    Button,
  },
  data: () => {
    return {
      // @todo
    };
  },
  mounted() {
    feather.replace()
  },
  methods:{
    // @todo
  }
}
</script>

<style scoped>

</style>
