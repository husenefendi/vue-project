<template>
  <v-app>
    <!-- <v-navigation-drawer v-model="drawer" absolute temporary app>
      <SidebarComponent />
    </v-navigation-drawer> -->

    <v-app-bar app>
      <nav>
        <router-link to="/">Home</router-link> |
        <router-link to="/about">About</router-link>
      </nav>
    </v-app-bar>

    <!-- Sizes your content based upon application components -->
    <v-main>
      <!-- Provides the application the proper gutter -->
      <v-container fluid>
        <!-- If using vue-router -->
        <router-view></router-view>
      </v-container>
    </v-main>

    <v-footer app>
      <footer>
        <h2>footer</h2>
      </footer>
    </v-footer>
  </v-app>
</template>
<script>
// @ is an alias to /src
// import SidebarComponent from "./components/Layouts/Sidebar/SidebarComponent.vue";

export default {
  name: "MainApp",
  components: {
    // SidebarComponent,
  },
  data() {
    return {
      drawer: null,
    };
  },
};
</script>


<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
