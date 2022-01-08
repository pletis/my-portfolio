<template>
  <div id="app">
    <Header />
    <Profile />
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Profile from "@/components/Profile.vue";

export default {
  name: "App",
  components: {
    Header,
    Profile,
  },
};
</script>

<style>
body {
  margin: 0;
  padding: 0;
}
</style>
