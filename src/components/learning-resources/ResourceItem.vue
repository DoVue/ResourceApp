<template>
  <li>
    <div>
      <header>
        <h3></h3>
        <button>Delete</button>
      </header>
    </div>
    <p></p>
    <nav><a href="">View Resource</a></nav>
  </li>
</template>

<script>
export default {
  name: "ResourceItem",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
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
