<template>
  <button @click="modalOpen = true">Open full screen modal!</button>

  <teleport to="body">
    <div v-if="modalOpen" class="modal">
      <div>
        <ChildComponent name="fullscreen modal" />
        <button @click="modalOpen = false">Close</button>
      </div>
    </div>
  </teleport>
</template>

<script>
import ChildComponent from "./ChildComponent";
export default {
  components: {
    ChildComponent,
  },
  data() {
    return {
      modalOpen: false,
    };
  },
};
</script>

<style lang="scss" scoped>
.modal {
  color: white;
  background-color: blue;
  position: absolute;
  top: 0;
  left: 0;
  width: 100vw;
  height: 100vh;
}
</style>