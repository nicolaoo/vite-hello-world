<script >

import HelloWorld from './components/HelloWorld.vue';
import FirstText from './components/AppTitle.vue';
//1. importo il componente 

export default {
  data() {
    return {
      name: 'la mia prima pagina su vite'
    }
  },
  components: {
    AppTitle
    //2. registro all'interno export il componente
    // precedentemente importato
  }
}

</script>

<template>
  <div>
    <a href="https://vitejs.dev" target="_blank">
      <img src="/vite.svg" class="logo" alt="Vite logo" />
    </a>
    <a href="https://vuejs.org/" target="_blank">
      <img src="./assets/vue.svg" class="logo vue" alt="Vue logo" />
    </a>
  </div>
  <HelloWorld msg="Vite + Vue" />

  <!-- 3. utilizzo il componente  -->
  <AppTitle></AppTitle>
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}

.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}

.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
