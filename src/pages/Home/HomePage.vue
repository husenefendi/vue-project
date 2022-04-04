<template>
  <v-container>
    <h1>ini home : {{ title }}</h1>
  </v-container>
</template>

<script>
export default {
  props: ["title"],
  data: () => {},
  computed() {
    console.log("Home computed");
  },
  created() {
    console.log({ created: this.title });
  },
};
</script>