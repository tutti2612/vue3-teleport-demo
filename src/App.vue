<template>
  <div>
    <h1>Vue3 Teleport Demo</h1>
    <div style="position: relative">
      <h3>Tooltips with Vue 3 Teleport</h3>
      <div>
        <modal-button></modal-button>
      </div>
    </div>
  </div>
</template>

<script>
import ModalButton from "./components/ModalButton";
export default {
  components: {
    ModalButton,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
