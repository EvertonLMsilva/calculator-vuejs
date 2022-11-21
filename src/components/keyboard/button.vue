<template>
  <div id="idButton" class="container">
    <input
      class="button"
      type="button"
      :value="values"
      :style="`${bgColor ? 'background: ' + bgColor : ''};`"
    />
  </div>
</template>

<script lang="ts">
export default {
  name: "CButton",
  props: {
    values: [Number, String],
    bgColor: {
      type: String,
    },
  },
};
</script>

<style>
.container {
  display: flex;
  justify-content: center;
  align-content: center;
  flex: 1;
}
.button {
  color: #fff;
  font-size: 1.5rem;
  cursor: pointer;
  border: none;
  width: 100%;
  height: 100%;
  background: rgb(173, 173, 173);
}
.button:hover {
  background: rgb(107, 107, 107);
  font-size: 1.7rem;
}
</style>
