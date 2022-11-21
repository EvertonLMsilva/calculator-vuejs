<template>
  <div id="idKeyboard" class="containerKeyboard">
    <div class="numberOrder">
      <Button
        class="alignItens buttonKeyboard"
        values="AC"
        bgColor="rgb(236, 132, 46)"
      />
      <Button class="alignItens buttonKeyboard" values="⬅" />
      <Button class="alignItens buttonKeyboard" values="%" />
      <Button class="alignItens buttonKeyboard" values="/" />
    </div>
    <div class="numberOrder">
      <Button class="alignItens buttonKeyboard" :values="9" />
      <Button class="alignItens buttonKeyboard" :values="8" />
      <Button class="alignItens buttonKeyboard" :values="7" />
      <Button class="alignItens buttonKeyboard" values="*" />
    </div>
    <div class="numberOrder">
      <Button class="alignItens buttonKeyboard" :values="6" />
      <Button class="alignItens buttonKeyboard" :values="5" />
      <Button class="alignItens buttonKeyboard" :values="4" />
      <Button class="alignItens buttonKeyboard" values="-" />
    </div>
    <div class="numberOrder">
      <Button class="alignItens buttonKeyboard" :values="3" />
      <Button class="alignItens buttonKeyboard" :values="2" />
      <Button class="alignItens buttonKeyboard" :values="1" />
      <Button class="alignItens buttonKeyboard" values="+" />
    </div>
    <div class="numberOrder">
      <Button class="alignItensTwoColumns buttonKeyboard" :values="0" />
      <Button class="alignItens buttonKeyboard" values="," />
      <Button
        class="alignItens buttonKeyboard"
        values="="
        bgColor="rgb(97, 173, 235)"
      />
    </div>
  </div>
</template>

<script lang="ts">
import Button from "@/components/keyboard/button.vue";
export default {
  name: "CKeyboard",
  components: { Button },
  methods: {},
};
</script>

<style>
.containerKeyboard {
  display: flex;
  flex-direction: column;
  padding: 2px;
  width: 100%;
  height: 100%;
  background: rgb(255, 255, 255);
}
.numberOrder {
  display: flex;
  justify-content: space-between;
  flex: 1;
}
.alignItens {
  text-align: center;
  justify-content: center;
  flex: 1;
  margin: 1px;
}
.alignItensTwoColumns {
  justify-content: center;
  text-align: center;
  flex: 2;
  margin: 1px;
}
.buttonKeyboard {
  font-size: 1.5rem;
  cursor: pointer;
}
</style>
