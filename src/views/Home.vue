<template>
  <div class="home" style="width: 100%">
    <Banner style="position: fixed; width: 100vw" />
    <div class="container-fluid" style="position: absolute; top: 20vh">
      <div class="row">
        <div
          class="col s12 m10 l5 xl4 offset-s0 offset-m1 offset-xl1 offset-l1"
        >
          <div class="center valign-wrapper">
            <Imagen style="z-index: 10" />
          </div>
        </div>
        <div class="col s10 m8 l5 xl4 offset-s1 offset-m2 offset-l1 offset-xl2">
          <div class="valign-wrapper center">
            <Inicio />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src

import Banner from "@/components/Banner.vue";
import Inicio from "@/components/Inicio.vue";
import Imagen from "@/components/Imagen.vue";

export default {
  name: "Home",
  components: {
    Banner,
    Inicio,
    Imagen,
  },
};
</script>
