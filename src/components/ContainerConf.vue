<template>
  <div class="container">
      <br>
      <div class="columns is-desktop is-mobile is-table is-multiline is-centered">
          <configuration v-for="payflowRule of payflowRules" v-bind:key="payflowRule.name" v-bind:payflowRule="payflowRule"/>
      </div>
  </div>
</template>

<script lang="ts">
import Vue from "vue";
import Configuration from "@/components/Configuration.vue";

function responseCodeMapper() {
  return {
    name: "Response Code Mapper",
    description: "Para mapear codigos de respuesta",
    url: "endpoint"
  };
}

function antifraudImplementation() {
  return {
    name: "Antifraud Implementations",
    description: "Reglas para configurar proveedores de antifraude",
    url: "endpoint"
  };
}

export default Vue.extend({
  name: "ContainerConf",
  components: {
    Configuration
  },
  data: function() {
    return { payflowRules: [
        responseCodeMapper(), 
        antifraudImplementation()
    ] };
  }
});
</script>