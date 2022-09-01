<template>
    <div id="aplicacion">
        <h1>Punto 11: Notas calculadas con objetos</h1>
        <h2>Ingrese su nombre</h2>
        <input type="text" v-model="estudiante.nombre">
        <h2>Ingrese sus notas</h2>
        <div id="res">
            <input type="number" v-model="estudiante.nota1">
            <input type="number" v-model="estudiante.nota2">
            <input type="number" v-model="estudiante.nota3">
        </div>
        <h2 v-if="estudiante.nota1 === '' || estudiante.nota2 === '' || estudiante.nota3 === '' || nombre === ''"></h2>
        <h2 v-else>Hola {{ estudiante.nombre }}, en esta ocasion usted {{ notas }} la materia</h2>
    </div>
</template>


<script >
    export default {
        name: 'ObjNotas',
        data() {
            return {
                estudiante: {
                    nombre: '',
                    nota1: '',
                    nota2: '',
                    nota3: ''
                }
            }
        },
        computed: {
            notas() {
                var prom = 0;
                prom = Number((this.estudiante.nota1 + this.estudiante.nota2 + this.estudiante.nota3)) / 3
                if (prom >= 3.0) {
                    return 'pasa'
                } else {
                    return 'nopasa'
                }
            }
        }
    }
</script>