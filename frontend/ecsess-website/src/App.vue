<template>
  <div id="app">
    <div id="firstscreen" class="firstscreen">
      <NavBar/>
    </div>
    <transition class="route-transition">
      <router-view/>
    </transition>
  </div>
</template>

<script>
import NavBar from './components/NavBar'

export default {
  name: 'App',
  components: {NavBar},
  created() {
    window.addEventListener("scroll", function () {
        if (this.document.getElementById("main-image") !== null) {
            document.getElementById("main-image").style.opacity = 1 - 0.005 * window.scrollY;
        }
    });
  },
}
</script>

<style lang="scss">
@import "./components/styles/style-components/button.scss";

* {
  margin: 0;
  padding: 0;
  -ms-overflow-style: none;
  scrollbar-width: none;
}

*::-webkit-scrollbar {
    display: none;
}

body {
  background-color: lightyellow;

}

html {
  scroll-behavior: smooth;
}

.route-transition {
  transition: ease-in-out 0.3s;
}

a {
    text-decoration: none;
}

</style>
