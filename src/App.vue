<template>
  <div>
    <app-header v-on:renew="renewString" v-bind:propsdata="str"></app-header>
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";

export default {
  data: function () {
    return {
      str: "Header",
    };
  },
  components: {
    "app-header": AppHeader,
  },
  methods: {
    renewString: function () {
      this.str = "Hi";
    },
  },
};
</script>

<style></style>
