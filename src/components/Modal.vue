<template>
  <div class="backdrop">
    <div class="modal">
      <h1>{{ modalTitle }}</h1>
      <p>Modal content</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Modal",
  props: {
    modalTitle: {
      type: String,
      required: true
    }
  }
};
</script>

<style>
.modal {
  width: 400px;
  padding: 20px;
  margin: 100px auto;
  background: white;
  border-radius: 10px;
}
.backdrop {
  top: 0;
  position: fixed;
  background: rgba(0, 0, 0, 0.5);
  width: 100%;
  height: 100%;
}
</style>
