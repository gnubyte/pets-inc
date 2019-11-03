<template>
  <div id="app">
    <!-- Navbar-->
          <b-navbar toggleable="sm" type="dark" variant="dark">
          <b-navbar-toggle target="nav-text-collapse"></b-navbar-toggle>
          <b-navbar-brand>Test Site</b-navbar-brand>

          <b-collapse id="nav-text-collapse" is-nav>
            <b-navbar-nav>
              <b-nav-item><router-link class="nav-link" to="/home">Home</router-link></b-nav-item>
              <b-nav-item><router-link class="nav-link" to="/cats">Cats</router-link></b-nav-item>
              <b-nav-item><router-link class="nav-link" to="/dogs">Dogs</router-link></b-nav-item>
            </b-navbar-nav>
          </b-collapse>
        </b-navbar>
        <router-view>

        </router-view>
    <!-- end Navbar-->
  </div>
</template>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
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
