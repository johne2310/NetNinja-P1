<template>
  <h1>{{ title }}</h1>
  <Modal :modal-title="header"></Modal>
</template>

<script>
import Modal from "@/components/Modal";
export default {
  name: "App",
  components: {
    Modal
  },
  data() {
    return {
      title: "My first Vue App :)",
      header: "Sign up for the giveaway"
    };
  },
  methods: {
    clickHandler() {
      console.log(this.$refs.name);
      this.$refs.name.classList.add("active");
      this.$refs.name.focus();
    }
  }
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
