<template>
    <nav class="navbar navbar-dark bg-dark">
    <div class="container-fluid">
      <a class="navbar-brand" href="#">{{title}}</a>
      <form class="d-flex">
        <input type="search"
         placeholder="Поиск..."
          aria-label="Search" 
          class="form-control me-2"
          v-model="search"
          @input="changeSearch(search)"
          >
            
        <button type="reset" class="btn btn-outline-light">
          все
        </button>
      </form>
    </div>
  </nav>
</template>

<script>
    export default {
        name: "AppHeader",
        props: ['title','changeSearch'],
        data() {
            return {
                search: '',
            }
        },
    }
</script>

<style scoped>

</style>
