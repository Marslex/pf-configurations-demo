<template>
  <div class="column is-12-mobile is-4-desktop is-4-tablet">
    <div class="card">
      <header class="card-header">
        <p class="card-header-title">{{ payflowRule.name }}</p>
      </header>
      <div class="card-content">
        <div class="columns is-desktop is-mobile is-table is-multiline is-centered">
          <div class="column is-full">{{ payflowRule.description }}</div>
          <div class="column is-full">
            <button class="button is-rounded is-info is-small">Download rules</button>
            <button class="button is-rounded is-info is-small">Upload Rules</button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  name: "Header",
  props: ["payflowRule"]
});
</script>
