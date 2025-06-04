<script setup lang="ts">
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
</script>

<template>
  <div class="title">Antoine Gires</div>
  <header>
    <img alt="Vue logo" class="logo" src="./assets/git-logo.svg" width="200" height="200" />
    <div class="wrapper">
      <HelloWorld msg="Welcome to my Git-pages" />
    </div>
  </header>
  <div class="main-grid">
    <main><TheWelcome /></main>
  </div>
</template>

<style scoped>
.title {
  grid-column: 1/3;
  grid-row: 1;
  font-size: 300%;
  text-align: center;
  margin-bottom: 50px;
}
header {
  grid-column: 1;
  grid-row: 2;
  line-height: 1.5;
}
.main-grid {
  grid-column: 2;
  grid-row: 2;
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
