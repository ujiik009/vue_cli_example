<template>
  <div>
    <input v-model="name"/>
    <br>
    <input v-model="link">
    <profile v-bind:name="name"></profile>
    <img :src="link">
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
      link: 'https://media.licdn.com/media/AAEAAQAAAAAAAANbAAAAJDE5NjBkNDk1LTY3ZGQtNDA0NS04YTJiLTdkNmU3NjZiNjI3Mg.png',
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
