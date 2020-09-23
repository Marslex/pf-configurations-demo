<template>
  <ContainerConfiguration/>
</template>

<script lang="ts">
import Vue from "vue";
import ContainerConfiguration from "@/components/ContainerConfiguration.vue";

export default Vue.extend({
  name: "Home",
  components: {
      ContainerConfiguration
  }
});
</script>
