<template>
  <div id="app">
    <AppHeader />
    <Intro />
    <AppFooter />
  </div>
</template>

<script>
import AppHeader from './Header/Header.vue';
import Intro from './Intro/Intro.vue';
import AppFooter from './Footer/Footer.vue';

export default {
  name: 'app',
  components: {
    AppHeader,
    Intro,
    AppFooter,
  },
};
</script>

<style lang="scss">

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  // -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}

.Container {
  margin: 0 auto;
  max-width: 1180px;
  width: 100%;
  padding: 0 15px;
}

.ContainerBox {
  max-width: 800px;
}

.Button {
  padding: 1em 3em;
  text-transform: uppercase;
  font-weight: bolder;
  text-decoration: none;
  display: inline-block;
  color: #666;
  position: relative;
  box-shadow: 0px 27px 30px 8.16px rgba(162, 162, 162, 0.3);
  transition: all .3s ease;
  top: 0;
  border-top: 2px solid transparent;
  border-bottom: 2px solid transparent;

  &.-default {
    background-color: #ffffff;
  }

  &:hover {
    box-shadow: 0px 29px 42.84px 8.16px rgba(162, 162, 162, 0.3);
    text-decoration: none;
    color: #524d31e7;
    top: -2px;
    border-bottom: 2px solid #ffdd00;
  }

  &:active {
    top: 1px;
    box-shadow: 0px 27px 30px 8.16px rgba(162, 162, 162, 0.3);
    transform: all .1s ease;
    color: #ffdd00;
  }
}

</style>
