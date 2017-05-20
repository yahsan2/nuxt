<template>
  <v-app>
    <v-toolbar class="grey lighten-1">
      <v-toolbar-side-icon @click.native.stop="$store.commit('toggleSidebar')" />
    </v-toolbar>
    <main>
      <v-sidebar left fixed drawer v-model="$store.state.sidebar">
        <v-list>
          <v-list-item>
            <v-list-tile to="/">
              <v-list-tile-title>Home</v-list-tile-title>
            </v-list-tile>
            <v-list-tile to="/about">
              <v-list-tile-title>About</v-list-tile-title>
            </v-list-tile>
          </v-list-item>
        </v-list>
      </v-sidebar>
      <v-content>
        <v-container fluid>
          <nuxt />
        </v-container>
      </v-content>
    </main>
  </v-app>
</template>

<style>
  html {
    font-family: "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
    font-size: 16px;
    word-spacing: 1px;
    -ms-text-size-adjust: 100%;
    -webkit-text-size-adjust: 100%;
    -moz-osx-font-smoothing: grayscale;
    -webkit-font-smoothing: antialiased;
    box-sizing: border-box;
  }
  *, *:before, *:after {
    box-sizing: border-box;
    margin: 0;
  }
  .page {
    display: flex;
    align-items: center;
    justify-content: center;
    min-height: 100vh;
    margin-top: -64px;
  }
</style>
