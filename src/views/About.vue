<template>
  <div
    class="about"
    style="
      width: 100%;
      background-color: black;
      min-height: 540px;
      position: absolute;
      top: 0vh;
    "
  >
    <div class="container-fluid">
      <div class="row">
        <div class="col s8 offset-s2">
          <h1>Hola</h1>
          <p>
            Muchas gracias por visitar esta sección, este proyecto fue realizado
            con Vue.js, Materialize y Three.js
          </p>
          <p>
            ¿Deseas ver otros trabajos mios? Accede a ellos pulsando
            <a href="https://mabmab159.github.io/" style="color: #08fdd8"
              >aquí</a
            >
          </p>
        </div>
        <footer class="footer">
          <p class="center-align">
            <a href="https://github.com/mabmab159">MabMab^^</a> - Copyright 2021
            💚 - Supported by:
            <a href="https://github.com/AndyRCR">AndyRCR</a>
          </p>
        </footer>
      </div>
    </div>
  </div>
</template>
<style scoped>
.about {
  margin-top: 64px;
}
h1 {
  font-size: 40px;
  color: #08fdd8;
}
p {
  font-size: 20px;
}
* {
  color: white;
}
a:hover {
  color: #08fdd8;
}
.footer {
  position: absolute;
  bottom: 40px;
  width: 100vw;
  color: white;
  padding: 0 20px;
}
</style>
