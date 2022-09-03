<template>
  <div class="col">
    <h4 class="text-indigo-9">{{Nombre_completo}}</h4>
    <h4 class="text-deep-purple-6">{{titulo}}</h4>
    <hr>
    <div>
      <span><strong>Fecha de nacimiento:</strong> {{datos_personales.fecha_nacimiento}} </span>
      <span><strong>Cedula de Identidad:</strong> {{datos_personales.ci}}</span>
      <span><strong>Dirección:</strong> {{datos_personales.direccion}}</span>
      <span><strong>Email:</strong> {{datos_personales.email}}</span>
      <span><strong>Telefono</strong> {{datos_personales.telefono}}</span>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Title',
  setup () {
    const Nombre_completo = 'Adonis David Pérez Farias'
    const titulo = 'Síntesis Curricular'
    const datos_personales = {
      fecha_nacimiento:'01-10-1993',
      ci:'23.917.268',
      direccion:'Av. Orinoco, frente a la Agencia Unida de Automóviles (Chevrolet), casa #304-A. Edo. Monagas',
      email:'Adonisdavid20@gmail.com',
      telefono: '0414-8942782'
    }
    return { Nombre_completo, titulo, datos_personales}
  }
}
</script>
<style lang="scss" scoped>
  hr {
    height: 5px;
    background-color: black;
  }
  span{
    display: block;
  }
</style>
