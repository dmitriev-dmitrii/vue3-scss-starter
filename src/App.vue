<template>
  <img alt="Vue 3 logo" src="@/assets/logo.png" class="logo" />
  <div class="nav contanier">
    <router-link to="/">Home</router-link>
    <router-link to="/about">About</router-link>
  </div>
  <router-view />
</template>

<style lang="scss">
body {
  background-color: $bgColor1;
  color: $mainTxtColor;
}
.logo {
  max-height: 1em;
}

#app {
}

.nav {
  padding: 1.5em 0;
  a {
    font-weight: bold;
    margin-right: 1em;
    color: inherit;
    &.router-link-exact-active {
      color: $mainAccentColor;
    }
  }
}
</style>
