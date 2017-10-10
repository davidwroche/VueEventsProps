<template>
<div id="first">
  <h1>ParentPanel</h1>

  <!-- I am the parent component. I hold all the data for this block.
      The only value attribute I have is msg. I have two children.

      I accept event's from the child component action. This event updates my msg data

      My other child childlist gets passed this data as props. So when I get an update
      from action I pass my data to List-->


      <!-- If you need me to expand upon this with props as an array or delete -->
      <!-- Delete should be the same you just emit an event from list back to here
          and the parent will update the child data-->

  <childaction @passValue="msg = $event"></childaction>
  <childlist :msg="msg"></childlist>

</div>
</template>

<script>
import ChildAction from './ChildAction.vue';
import ChildList from './ChildList.vue';

export default {
  components: {
      childaction: ChildAction,
      childlist: ChildList,
    },

  data() {
    return {
      msg: ''
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
  background-color: #FF3333;
  padding-bottom: 30px;
}
</style>
