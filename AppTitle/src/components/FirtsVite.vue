
<template>
    <figure class="pika">

        <img src="https://www.pokemon.com/static-assets/app/static3/img/og-default-image.jpeg">
    </figure>
    <div>
        <h1 class="first-text">
            {{ name }}
            {{ subtitle }}
        </h1>
        <input class="name-poke" v-model="subtitle" placeholder="inserisci tutti i pokemon!!" type="text">
        <button class="btn-poke" @click="getANewMessage">
            cliccami
        </button>
        <ul>
            <li v-for="element in newText">
                <img class="profile"
                    src="https://thumbor.forbes.com/thumbor/fit-in/900x510/https://www.forbes.com/advisor/in/wp-content/uploads/2022/03/monkey-g412399084_1280.jpg">
                {{ element }}
                <img class="profile"
                    src="https://mir-s3-cdn-cf.behance.net/project_modules/max_1200/8555bc116147295.605c07d985be1.gif">
            </li>
        </ul>
    </div>
</template>


<script>
export default {
    data() {
        return {
            name: 'questa è la mia prima pagina su vite!!',
            subtitle: '',
            newText: [],
        }
    },
    methods: {
        getANewMessage() {


            this.newText.push(this.subtitle)
            this.subtitle = ''
        }
    }
}

</script>


<style>
.first-text {
    background-color: cadetblue;
    border-radius: 15px;
    padding: 15px;
    color: darkkhaki;

}

img {
    max-width: 100%;

}

.btn-poke {
    margin-left: 15px;
    background-color: darkorange;
    border: 0;
}

.btn-poke:hover {
    background-color: forestgreen;
    color: white;
    width: 115px;
    height: 50px;

}

.name-poke {
    border-radius: 20px;
    padding: 10px;
    width: 190px;

}

.profile {
    border-radius: 999px;
    width: 30px;

}
</style>