<template>
  <!--  <div id="app">
      <LayoutBlue>

      </LayoutBlue>
    </div>-->

  <component :is="layout">
    <router-view :layout.sync="layout"/>
  </component>
</template>

<script>

// import LayoutDefault from "@/layouts/LayoutDefault";
// import LayoutBlue from "@/layouts/LayoutBlue";

export default {
  name: 'App',
  data() {
    return {
      layout: 'div'
    }
  },
  components: {
    // LayoutDefault,
    // LayoutBlue
  }
}

</script>

<style lang="scss">

</style>
