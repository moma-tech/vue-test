/* eslint-disable */
<template>
  <div class="h1">
    <div>{{message}}</div>

    <div><input type="button" v-on:click="show_my_name()" value="123" /></div>
  </div>
</template>
<script>
let message = "abc";
let person = {
  firstname: "Ivan",
  lastname: "Dong",
  phase: "TO"
};
export default {
  data() {
    return {
      message: person.firstname + "." + person.lastname
    };
  },
  methods: {
    show_my_name: function() {
      console.log("My name " + this.message);
    }
  }
};
</script>
<style>
.h1 {
  color: blue;
  font-size: 20px;
}
</style>
