<template>
  <div>
    <input v-model="name">
    <p v-if="name">Hi, {{ name }}</p>
    <ul>
      <li v-for="list in lists ">{{ list }}</li>
    </ul>
    <button @click="say">say</button>
  </div>

</template>

<script>
export default {
  data () {
    return {
      name: '',
      lists: [
        1,
        2,
        3,
        4,
        5
      ]
    }
  },
  methods: {
    say: () => {
      alert(555)
    }
  }
}
</script>
