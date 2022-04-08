<template>
  <h1>Hello World</h1>
  <div class="nav">
    <ul>
      <li><a href="#">Home</a></li>
    </ul>
  </div>
</template>

<script>
import axios from "axios";

axios.get("http://localhost:1337/api/team-members").then((response) => {
  console.log(response);
});

export default {
  name: "Home-view",
};
</script>

<style>
.nav {
  padding-top: 2rem;
}

ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  display: inline;
}

li {
  text-decoration: none;
  display: inline;
  padding: 2rem;
}
</style>
