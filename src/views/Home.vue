<template>
  <div class="home">
    <div class="container">
      <BlockFirst></BlockFirst>
      <BlockTwo></BlockTwo>
      <BlockThree></BlockThree>
      <BlockFour></BlockFour>
    </div>
  </div>
</template>

<script>

import LayoutDefault from "@/layouts/LayoutDefault";

import BlockFirst from "@/components/Home/BlockFirst";
import BlockTwo from "@/components/Home/BlockTwo";
import BlockThree from "@/components/Home/BlockThree";
import BlockFour from "@/components/Home/BlockFour";

export default {
  name: 'Home',
  created() {
    this.$emit('update:layout', LayoutDefault)
  },
  components: {
    BlockFirst,
    BlockTwo,
    BlockThree,
    BlockFour
  }
}
</script>
