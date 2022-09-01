<template>
    <div id="aplicacion">
        <h1>Punto 3: Saludo</h1>
        <h2>Ingresa tu nombre</h2>
        <input id="nombre" type="text" v-model="nombre">
        <h2>¿Qué hora es?</h2>
        <input id="hora" type="time" v-model="hora">
        <h2 v-if="hora > '12:00' && hora < '18:01'">Buenas tardes, {{ nombre }}</h2>
        <h2 v-else-if="hora > '18:00' && hora < '24:00'">Buenas noches, {{ nombre }} </h2>
        <h2 v-else-if="hora == ''"></h2>
        <h2 v-else>Buenos dias, {{ nombre }}</h2>
    </div>
</template>


<script >
    export default {
        name: 'Saludo',
        data() {
            return {
                nombre: '',
                hora: ''
            }
        }    
    }
</script>