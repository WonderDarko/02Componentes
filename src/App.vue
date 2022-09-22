<template>
  <h1>Componentes en Vue</h1>
  <hr/>
  <card url="https://cdn.svgporn.com/logos/vue.svg" nombre="Vue.js"/>
  <card url="https://cdn.svgporn.com/logos/angular-icon.svg" nombre="Angular"/>
  <card url="https://cdn.svgporn.com/logos/vuetifyjs.svg" nombre="Vuetify"/>
  <card url="https://cdn.svgporn.com/logos/react.svg" nombre="React"/>
  <br>
  <contador nombre-clase="btn btn-info"></contador>
  <contador nombre-clase="btn btn-danger"></contador>
  <contador nombre-clase="btn btn-success"></contador>
  <br>
  <modal>
    <template v-slot:header>
      <h5 class="modal-title" id="exampleModalLabel">Hola Mundo</h5>
    </template>
    <p>Esto es un contenido para nuestro modal</p>
    <template v-slot:footer>
      <button type="button" class="btn btn-secondary" data-dismiss="modal">Cerrar</button>
      <button type="button" class="btn btn-primary">Enviar</button>
    </template>
  </modal>
  <button type="button" class="btn btn-primary" data-toggle="modal" data-target="#exampleModal">
  Launch demo modal
  </button>
</template>

<script>
  import Card from "./components/Card.vue";
  import Contador from "./components/Contador.vue";
  import Modal from "./components/Modal.vue";
  export default{
    components: { Card, Contador, Modal },
    
  };
</script>