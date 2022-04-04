<template>
  <v-app>
    <v-main>
      <Home title="Title From App" />
    </v-main>
  </v-app>
</template>

<script>
import Home from "./pages/Home/HomePage.vue";

export default {
  name: "App",

  components: {
    Home,
  },

  data: () => ({
    //
  }),
};
</script>
