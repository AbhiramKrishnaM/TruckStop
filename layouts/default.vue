<template>
  <v-app>
    <v-navigation-drawer v-model="drawer" app>
      <v-list dense flat nav>
        <v-list-item v-for="[icon, text] in links" :key="icon" link dense :ripple="false" :to="`/${text}`" color="#38B069" active-class="link-active">
          <v-list-item-icon class="mr-3">
            <v-icon>{{ icon }}</v-icon>
          </v-list-item-icon>

          <v-list-item-content>
            <v-list-item-title>{{ text }}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>

    <!-- <v-main>
      <Nuxt />
    </v-main> -->
  </v-app>
</template>

<script>
export default {
  name: "DefaultLayout",
  data() {
    return {
      drawer: null,
      links: [
        ["mdi-inbox-arrow-down", "Dashboard"],
        ["mdi-send", "Freight management"],
        ["mdi-delete", "Tracking order"],
        ["mdi-alert-octagon", "Carriers"],
        ["mdi-alert-octagon", "Order history"],
        ["mdi-alert-octagon", "Billing details"],
        ["mdi-alert-octagon", "Settings"],
      ],
    };
  },
};
</script>

<style>
* {
  background: #e4eae5;
}

.link-active {
  border-left: 3px solid #38b069;
}
</style>
