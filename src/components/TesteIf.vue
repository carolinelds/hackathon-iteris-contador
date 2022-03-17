<template>
    <div class="teste-if">
        <h1 v-if="podeVer">Teste TRUE</h1>
        <h1 v-else>Teste False</h1>
    </div>
</template>

<script>
export default {
    name: 'TesteIf',
    data() {
        return {
            podeVer: false
        }
    }
}
</script>

<style scoped>

</style>