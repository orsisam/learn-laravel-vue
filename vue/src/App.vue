<script>
import HelloWorld from "./components/HelloWorld.vue";
import { mapState } from "vuex";

export default {
  components: {
    HelloWorld,
  },
  computed: {
    ...mapState(["user"]),
  },
};
</script>

<template>
  <pre>{{ user }}</pre>
  <img src="./assets/vue.svg" alt="Vue Logo" />
  <HelloWorld msg="Hello Vue 3 + Vite" />
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
