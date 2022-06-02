<template>
  <v-app>
    <nav id="nav-bar" class="navigation-bar">
      <img id="logo" :src="require('@/assets/images/logo.png')" alt="logo" />

      <div class="nav-links">
        <h1 class="nav-link-collections">Collections</h1>
        <h1 class="nav-link-brands">Brands</h1>
        <h1 class="nav-link-new">New</h1>
        <h1 class="nav-link-sales">Sales</h1>
      </div>

      <div id="login-signup-button" class="login-signup-button-wrapper">
        <v-btn dark fab icon plain class="mr-4" :ripple="false"
          ><v-icon>mdi-cart</v-icon></v-btn
        >
        <v-btn dark fab plain outlined :ripple="false"
          ><v-icon>mdi-truck-check</v-icon></v-btn
        >
      </div>
    </nav>

    <!-- <v-main>
      <Nuxt />
    </v-main> -->
  </v-app>
</template>

<script>
export default {
  name: 'DefaultLayout',
  data() {
    return {}
  },
}
</script>

<style>
* {
  background: #1f252e;
}

.navigation-bar {
  width: 85%;
  margin: 0.01px auto;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.nav-links {
  flex: 0.9;
  display: flex;
  align-items: center;
  justify-content: end;
}

h1 {
  color: white;
  font-weight: 300;
  margin: 0 60px;
}

img {
  width: 200px;
  height: 200px;
  object-fit: contain;
}

.login-signup-button-wrapper {
  display: flex;
  justify-content: end;
}
</style>
