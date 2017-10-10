<template>
<div id="first">
  <h1>ChildList</h1>
  {{msg}}
</div>
</template>

<script>
export default {
  props:['msg'],

  data() {
    return {
    }
  },
  methods: {


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
  background-color: blue;
}
</style>
