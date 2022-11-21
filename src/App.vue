<template>
  <div id="app">
    <div class="containerApp">
      <CDisplay :value="10" />
      <CKeyboard />
    </div>
  </div>
</template>

<script lang="ts">
import Vue from "vue";
import CDisplay from "@/components/Display.vue"; // @ is an alias to /src
import CKeyboard from "@/components/keyboard/keyboard.vue";

export default Vue.extend({
  name: "App",
  components: {
    CDisplay,
    CKeyboard,
  },
});
</script>

<style>
body {
  margin: 0;
}
#app {
  display: flex;
  flex-grow: 1;
  justify-content: center;
  align-items: center;
  align-content: center;
  height: 100vh;
  margin: 0;
  padding: 0;
  background-color: rgb(63, 62, 62);
}
.containerApp {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;
  align-content: center;
  text-align: center;
  width: 350px;
  height: 400px;
}
</style>
