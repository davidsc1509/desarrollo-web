<template>
    <div id="aplicacion">
        <h1>Punto 9: Generar tabla</h1>
        <div id="res">
            <h2>Columna</h2>
            <input type="number" v-model="columna">
            <h2>Fila</h2>
            <input type="number" v-model="fila">
            <button v-on:click.once="genera_tabla()">Genera</button>
        </div>
        <div id="tablam"></div>
    </div>
</template>

<script >
    export default {
        name: 'CrearTabla',
        data() {
            return {
                columna: '',
                fila: ''
            }
        },
        methods:
        {
            genera_tabla() {
                var body = document.getElementById('tablam');
                var tabla = document.createElement("table");
                var tblBody = document.createElement("tbody");
                for (var i = 0; i <= this.fila; i++) {
                    var hilera = document.createElement("tr");
                    for (var j = 0; j <= this.columna; j++) {
                        var celda = document.createElement("td");
                        var textoCelda = document.createTextNode("Fila" + i + ", Columna " + j);
                        celda.appendChild(textoCelda);
                        hilera.appendChild(celda);
                    }
                    tblBody.appendChild(hilera);
                }
                tabla.appendChild(tblBody);
                body.appendChild(tabla);
                tabla.setAttribute("border", "2");
            }
        }
    }
</script>