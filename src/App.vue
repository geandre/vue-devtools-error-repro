<template>
  <div>Test</div>
</template>

<script>
import Comp from "./components/Comp";
import Vue from "vue";
const CompClass = Vue.extend(Comp);

export default {
  name: "App",

  mounted() {
    this.$nextTick().then(() => {
      new CompClass({
        propsData: { item: [] },
      }).$mount();
      //
    });
  },
};
</script>
