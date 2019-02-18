<template>
  <div id="app">
    <div id="nav">
      <div class="left-nav">
        <router-link to="/" class="nav-link">
          <img src="@/assets/enactus_logo.png" class="enactus-logo">
        </router-link>
      </div>
      <div class="right-nav">
        <router-link to="/about" class="nav-link">About</router-link>
        <router-link to="/projects" class="nav-link">Projects</router-link>
        <router-link to="/recruitment" class="nav-link">Recruitment</router-link>
        <router-link to="/sponsors" class="nav-link">Sponsors</router-link>
        <router-link to="/contact" class="nav-link">Contact Us</router-link>
      </div>
    </div>
    <router-view/>
    <div id="lower-banner">
      <div class="left-nav">
        <img src="@/assets/enactus_logo_reversed.png" class="enactus-logo">
      </div>
      <div class="right-nav">
        <p class="banner-link">Privacy Policy</p>
        <router-link to="/contact" class="banner-link">Contact Us</router-link>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  // margin: 0;
}
#nav {
  height: 10vh;
  padding: 1vh 0;
  a {
    color: #2c3e50;
    &.router-link-exact-active {
      color: black;
      font-weight: bold;
    }
  }

  display: flex;
  flex-direction: row;
  align-items: center;
}

.left-nav {
  display: flex;
  flex-direction: row;
  justify-content: flex-start;
  width: 50vw;
  height: 10vh;
  padding-left: 1vw;
  align-items: center;
}

.right-nav {
  display: flex;
  flex-direction: row;
  justify-content: flex-end;
  width: 50vw;
  align-items: center;
  padding-right: 2vw;
}
.nav-link {
  padding: 0 1vw;
  text-decoration: none;
}

.enactus-logo {
  width: 8vw;
  height: auto;
}

#lower-banner {
  display: flex;
  flex-direction: row;
  align-items: center;
  background-color: black;
  padding: 1vh 1vw;
  height: 10vh;
}

.banner-link {
  color: grey;
  text-decoration: none;
  padding: 0 1vw;
  font-weight: bold;
}
</style>
