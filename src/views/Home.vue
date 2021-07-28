<template>
  <div class="home m-3">
    <button type="button" @click="vistaAgregar()" class="btn btn-primary">Agregar</button>

  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'Home',
  components: {
  },
  methods:{
    vistaAgregar() {
      this.$router.push({ name: "Agregar" });
    }
  }
}
</script>
