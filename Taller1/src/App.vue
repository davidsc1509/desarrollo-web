<template>
  <div class="complete">
    <HoraSeg />
    <Llamada />
    <Saludo />
    <TresNumeros />
    <ListaNumeros />
    <ImparMenores />
    <GuardaSalario />
    <PosicionAleatoria />
    <CrearTabla />
    <Matriz></Matriz>
    <ObjNotas />
    <ArrNotas />
    <h3>Taller 1. David Sanchez Collazos</h3>
  </div>



</template>
  
<script>
  import HoraSeg from './components/01-Hora.vue';
  import Llamada from './components/02-Llamadas.vue';
  import Saludo from './components/03-Saludo.vue';
  import TresNumeros from './components/04-TresNumeros.vue';
  import ListaNumeros from './components/05-ListarNumeros.vue';
  import ImparMenores from './components/06-ImparMenor.vue';
  import GuardaSalario from './components/07-Salario.vue';
  import PosicionAleatoria from './components/08-PosAleatorio.vue'
  import CrearTabla from './components/09-CrearTabla.vue';
  import Matriz from './components/10-Matriz.vue';
  import ObjNotas from './components/11-ObjetosNotas.vue';
  import ArrNotas from './components/12-ArregloNotas.vue';
  export default {
  name: 'App',
  components: {
      HoraSeg,
      Llamada,
      Saludo,
      TresNumeros,
      ImparMenores,
      ListaNumeros,
      GuardaSalario,
      PosicionAleatoria,
      CrearTabla,
      Matriz,
      ObjNotas,
      ArrNotas
  }
}
</script>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Outfit:wght@400;700&display=swap');
  
  
  #aplicacion-der {
    background-color: #78E3FD;
    padding: 2em;
    margin: 1em;
    border-radius: 1.5em;
    display: flex;
    flex-direction: column;
    width: 100%;
  
  }
  
  #aplicacion-izq {
    background-color: #78E3FD;
    padding: 2em;
    margin: 1em;
    border-radius: 1.5em;
    display: flex;
    flex-direction: column;
    width: 100%;
  
  }
  
  #aplicacion {
    background-color: #78E3FD;
    padding: 2em;
    margin: 1em;
    border-radius: 10px;
    display: flex;
    flex-direction: column;
  
  }
  
  h1 {
    font-family: 'Outfit', sans-serif;
    font-style: bold;
    font-weight: 700;
    font-size: 1.5em;
    line-height: 1.5em;
    text-align: left;
    padding-bottom: 1rem;
  }
  
  h2 {
    font-family: 'Outfit', sans-serif;
    font-style: normal;
    font-weight: 200;
    font-size: 1em;
    line-height: 1.5em;
    text-align: left;
    text-indent: 5px;
  }
  
  h3 {
    font-family: 'Outfit', sans-serif;
    font-style: normal;
    font-weight: 400;
    font-size: 0.8em;
    line-height: 1.5em;
    text-align: right;
    text-indent: 5px;
    margin: 2em
  }
  
  #res {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    gap: 5px;
  }
  
  input {
    font-family: 'Outfit', sans-serif;
    font-style: normal;
    font-weight: 300;
    font-size: 0.8em;
    line-height: 1.5em;
    text-align: left;
    text-indent: 5px;
    background-color: #D1F5FF;
    border-radius: 5px;
    outline: none;
    border: none;
    padding: 5px;
    width: 300px;
  }
  
  #tres {
    display: flex;
    flex-direction: column;
    gap: 3px;
    justify-content: space-between;
    
  }


  button {
    background-color: #34c7eb;
    font-family: 'Outfit', sans-serif;
    font-style: normal;
    font-weight: 200;
    font-size: 1em;
    line-height: 1.5em;
    text-align: center;
    text-indent: 5px;
    color: #292929;
    width: 300px;
    align-content: center;
    border: none;
    border-radius: 0.2em;
    
  }
  
  table {
    font-family: 'Outfit', sans-serif;
    font-size: 12px;
    margin: 45px;
    width: 50%;
    text-align: left;
    border-collapse: collapse;
  }
  
  th {
    font-size: 13px;
    font-weight: normal;
    padding: 8px;
    background: #D1F5FF;
    border-top: 4px solid #aabcfe;
    border-bottom: 1px solid #fff;
    color: #292929;
  }
  
  td {
    padding: 8px;
    background: #D1F5FF;
    border-bottom: 1px solid #fff;
    color: #292929;
    border-top: 1px solid transparent;
  }
  
  tr:hover td {
    background: #34f6f2;
    color: #292929;
  }
</style>