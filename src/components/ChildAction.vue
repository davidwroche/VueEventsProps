<template>
<div id="first">
  <h1>ChildAction</h1>
  <input v-model="msg">
  <button v-on:click="Add">Add</button>
</div>
</template>

<script>
export default {
  data() {
    return {
      msg:''
    }
  },
  methods: {
    Add(){
      var self = this;
      self.$emit('passValue',self.msg)

    }


  }


}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1,
h2 {
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
#first{
  background-color: green;
}
</style>
