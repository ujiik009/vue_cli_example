<template>
  <div >
   Hi, {{name}} year ={{ year }}
  </div>
</template>

<script>
export default {
  props: [
    'name',
    'year'
  ]
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
