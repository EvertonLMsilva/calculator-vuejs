<template>
  <div class="constainer">
    <span class="font">
      {{ value }}
    </span>
  </div>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  name: "CButton",
  props: {
    value: [String, Number],
  },
});
</script>

<style scoped>
.constainer {
  display: flex;
  justify-content: end;
  align-items: center;
  width: 100%;
  min-height: 80px;
  padding: 2px;
  background-color: rgb(255, 255, 255);
}
.font {
  font-size: 2rem;
  padding: 2px;
  font-family: monospace;
}
</style>
