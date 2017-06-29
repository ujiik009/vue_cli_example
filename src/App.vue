<template>
  <div>
    <input v-model="name"/>
    <profile v-bind:name="name"></profile>
    <profile :name="name"></profile>
  </div>
 
</template>

<script>
import profile from './components/Profile'

export default {
  components: {
    profile
  },
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
    say (text) {
      alert('hi ' + text)
    }
  }
}
</script>
