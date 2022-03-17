<template>
    <div class="meu-contador">
        <div>
            <p><strong>Contador: </strong>{{ numero }}</p>
        </div>
        <div class="buttons">
            <button v-on:click="apertaMenos">-</button>
            <button v-on:click="apertaMais">+</button>
        </div>
    </div>
</template>

<script>
export default {
    name: 'MeuContador',
    data(){
        return {
            numero: 0
        }
    },
    methods: {
        apertaMais(){
            this.numero += 1;
        },
        apertaMenos(){
            this.numero -= 1;
        }
    }
}
</script>

<style scoped>
    .p {
        font-size: large;
    }
    .buttons{
        margin-top: 20px;
        display: flex;
        justify-content: center;
    }
</style>