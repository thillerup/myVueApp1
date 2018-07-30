<template>
  <div id="app">
    <img style="width: 100px; height; 100px" src="https://upload.wikimedia.org/wikipedia/commons/thumb/8/85/Smiley.svg/600px-Smiley.svg.png">
    <h1>{{ msg }} {{ title }}</h1>
    <hr>
    <div style="border: 1px solid #ccc; width: 200px; margin:0 auto;">{{ title }}</div>
    <br>
    <input type="text" v-model="title">
   
    <button @click="newTitle()">New Title</button>
  </div>
</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      msg: 'Hello',
      title: 'Thillerup'
    }
  },
  methods: {
    newTitle() {
//       alert('Hi');
      this.title = 'New Title';
    }
    
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
