<script setup>
import HelloWorld from './components/HelloWorld.vue';
import TheWelcome from './components/TheWelcome.vue';
import ErebusHosted from './components/ErebusHosted.vue';
import LoginMenu from './components/LoginMenu.vue';
</script>

<template>
  <header>
    <img alt="CHOAM logo" class="logo" src="./assets/logo.svg" width="125" height="125" />

    <div class="wrapper">
      <HelloWorld welcomemsg="welcome to" submsg="The first Spice as a Service!"/>
    </div>
  </header>

  <main>
    <TheWelcome />
    <ErebusHosted />
  </main>
</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
