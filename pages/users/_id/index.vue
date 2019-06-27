<template>
  <h1> A single user, with ID: {{ $route.params.id}}</h1>
</template>

<script>

  export default {
    validate (data) {
      console.log(data)
      return /^\d+$/.test(data.params.id) //valida que sea un numero
    },
    layout:'users'
  }
</script>
