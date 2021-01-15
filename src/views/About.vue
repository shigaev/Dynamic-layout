<template>
  <div class="about">
    <AboutUp/>
  </div>
</template>

<script>

import LayoutBlue from "@/layouts/LayoutBlue";
// import LayoutDefault from "@/layouts/LayoutDefault";

import AboutUp from "@/components/About/AboutUp";


export default {
  name: 'About',
  created() {
    this.$emit('update:layout', LayoutBlue)
  },
  components: {
    AboutUp,
  }
}

</script>
