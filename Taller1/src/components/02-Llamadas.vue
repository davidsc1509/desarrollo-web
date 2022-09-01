<template>
    <div id="aplicacion">
        <h1>Punto 2: Calcular valor de la llamda</h1>
        <input type="number" v-model="numero">
        <h2 v-if="numero <= 3">La llamada tiene un valor de $100 </h2>
        <h2 v-else-if="numero === null"></h2>
        <h2 v-else>La llamada tiene un valor de ${{ 100 + (numero - 3) * 50 }}</h2>
    </div>
</template>

<script >
export default {
    name: 'Llamada',
    data() {
        return {
            numero: null
        }
    }
}
</script>