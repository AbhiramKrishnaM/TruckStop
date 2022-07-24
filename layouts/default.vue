<template>
  <v-app>
    <nav id="nav-bar" class="navigation-bar">
      <!-- <img id="logo" :src="require('@/assets/images/logo.png')" alt="logo" /> -->
    </nav>

    <!-- <v-main>
      <Nuxt />
    </v-main> -->
  </v-app>
</template>

<script>
export default {
  name: "DefaultLayout",
  data() {
    return {};
  },
};
</script>

<style>
* {
  background: #f5f5f5;
}

.navigation-bar {
  width: 85%;
  margin: 0.01px auto;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
</style>
