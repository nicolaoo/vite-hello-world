
<template>
    <div>
        <h1 class="first-text">
            {{ name }}
            {{ subtitle }}
        </h1>
        <input v-model="subtitle" type="text">
        <button>
            cliccami
        </button>
    </div>
</template>


<script>
export default {
    data() {
        return {
            name: 'questa è la mia prima pagina su vite!!',
            subtitle: ''
        }
    },
    methods: {
        getANewMessage() {
            concole.log(this.subtitle)
        }
    }
}

</script>


<style>
.first-text {
    background-color: cadetblue;
}
</style>