<template>
  <div id="app">
    <Popper arrow hover>
      <button>Click this</button>
      <template #content>
        <div>This is the content</div>
      </template>
    </Popper>
    <Popper arrow hover placement="top">
      <button>Click this</button>
      <template #content>
        <div>This is the content</div>
      </template>
    </Popper>
    <Popper arrow hover placement="left">
      <button>Click this</button>
      <template #content>
        <div>This is the content</div>
      </template>
    </Popper>
    <Popper arrow hover placement="right">
      <button>Click this</button>
      <template #content>
        <div>This is the content</div>
      </template>
    </Popper>
  </div>
</template>

<script>
  import { defineComponent } from "vue";
  import Popper from "@/component/Popper.vue";

  export default defineComponent({
    name: "ServeDev",
    components: {
      Popper,
    },
  });
</script>

<style>
  #app {
    color: #2c3e50;
    height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap: 100px;
  }
</style>
