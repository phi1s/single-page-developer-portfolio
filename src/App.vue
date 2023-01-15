<template>
  <DeveloperPortfolio />
</template>

<script>
import DeveloperPortfolio from "./components/DeveloperPortfolio.vue";

export default {
  name: "App",
  components: {
    DeveloperPortfolio,
  },
};
</script>

<style>
@font-face {
  font-family: "SpaceGrotesk";
  src: local("SpaceGrotesk"),
    url("./assets/fonts/SpaceGrotesk-VariableFont_wght.ttf") format("truetype");
}
#app {
  font-family: "SpaceGrotesk", sans-serif;
  font-style: normal;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #ffffff;
  background-color: #151515;
  text-align: center;
  position: absolute;
  top: 0;
  left: 0;
  width: 100vw;
  overflow: hidden;
}

h1 {
  font-weight: 700;
  font-size: 40px;
  line-height: 40px;
  letter-spacing: -1.1px;
}
h2 {
  font-weight: 700;
  font-size: 32px;
  line-height: 40px;
  letter-spacing: -1px;
}
h3 {
  font-weight: 700;
  font-size: 24px;
  line-height: 32px;
}
p {
  color: #d9d9d9;
  font-weight: 500;
  font-size: 16px;
  line-height: 26px;
}

button {
  color: #ffffff;
  height: 40px;
  font-weight: 700;
  font-size: 16px;
  line-height: 26px;
  letter-spacing: 2.3px;
  text-transform: uppercase;
  border: none;
  background-color: transparent;
  border-bottom: 2px solid #4ee1a0;
  padding: 0px;
  padding-bottom: 10px;
}

button:hover {
  color: #4ee1a0;
}

.icons > img:hover {
  filter: invert(77%) sepia(56%) saturate(455%) hue-rotate(93deg)
    brightness(92%) contrast(90%);
}

span {
  border-bottom: 4px solid #4ee1a0;
}

@media screen and (min-width: 700px) {
  #app {
    text-align: left;
  }
  h1 {
    font-size: 72px;
    line-height: 72px;
    letter-spacing: -2px;
  }
  h2 {
    font-size: 48px;
    line-height: 56px;
    letter-spacing: -1.5px;
  }
  p {
    font-size: 18px;
    line-height: 28px;
  }
}
@media screen and (min-width: 1200px) {
  h1 {
    font-size: 88px;
    line-height: 88px;
    letter-spacing: -2.5px;
  }
}
</style>
