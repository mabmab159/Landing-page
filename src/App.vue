<template>
  <div class="container-fluid" style="position: relative">
    <div id="nav">
      <nav>
        <div class="nav-wrapper black">
          <router-link
            to="/"
            class="brand-logo"
            style="margin-left: 15px; font-size: 40px"
            >MabMab^^</router-link
          >
          <a
            href="#"
            data-target="mobile-demo"
            class="sidenav-trigger"
            @click="abrirMenu()"
            ><i class="material-icons">menu</i></a
          >
          <ul class="right hide-on-med-and-down">
            <li>
              <router-link to="/">Inicio</router-link>
            </li>
            <li><router-link to="/about">Sobre mí</router-link></li>
          </ul>
        </div>
      </nav>

      <ul class="sidenav" id="mobile-demo">
        <li>
          <router-link to="/" id="inicio" @click="test">Inicio</router-link>
        </li>
        <li>
          <router-link to="./about" id="about" @click="test"
            >Sobre mí</router-link
          >
        </li>
      </ul>
    </div>

    <router-view style="position: absolute; top: 0vh; z-index: -1" />
  </div>
</template>

<script>
import M from "materialize-css";

export default {
  mounted() {
    M.AutoInit();
  },
  methods: {
    test() {
      document.querySelector("body").style.setProperty("overflow", "");
      document
        .querySelector(".sidenav")
        .style.setProperty("transform", "translateX(-105%)");
      document.querySelector(".sidenav-overlay").style.display = "none";
      document.querySelector(".sidenav-overlay").style.opacity = 0;
    },
    abrirMenu() {
      document
        .querySelector(".sidenav")
        .style.setProperty("transform", "translateX(0%)");
      document
        .querySelector(".sidenav")
        .style.setProperty("transition", "transform 1s");
    },
  },
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Ubuntu+Mono&display=swap");
@import url("https://fonts.googleapis.com/icon?family=Material+Icons");
* {
  font-family: "Ubuntu Mono", monospace;
}
.material-icons {
  font-family: "Material Icons";
}
ul li a {
  font-size: 20px;
}

ul li a:hover {
  font-size: 20px;
  color: #08fdd8;
}
.brand-logo:hover {
  color: #08fdd8;
}

@keyframes media {
  0% {
    transform: translateX(-105%);
  }
  100% {
    transform: translateX(0%);
  }
}
</style>
