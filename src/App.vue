<template>
  <div>
    
    <ul>
      <li v-for="list in lists ">{{ list }}</li>
    </ul>
    <button @click="say('Ice')">say</button>
     <Hello name="ice" year="2017"></Hello>
      <Hello name="ice1" year="2015"></Hello>
       <Hello name="ice2" year="2016"></Hello>
  </div>
 
</template>

<script>
import Hello from './components/Hello'
export default {
  components: {
    Hello
  },
  data () {
    return {
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
