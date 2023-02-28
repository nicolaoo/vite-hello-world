<script >

import HelloWorld from './components/HelloWorld.vue';
import FirstVite from './components/FirtsVite.vue';
//1. importo il componente 

export default {
  data() {
    return {
      name: 'la mia prima pagina su vite'
    }
  },
  components: {
    FirstVite
    //2. registro all'interno export il componente
    // precedentemente importato
  }
}

</script>

<template>
  <!-- 3. utilizzo il componente  -->
  <FirstVite></FirstVite>
</template>

<style scoped>
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}

.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
