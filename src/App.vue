<template>
  <div id="app">
   <List />
  </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.row {
  display: flex;
  justify-content: space-around;
  padding-top: 5rem;
  margin-left: 20rem;
  margin-right: 20rem;
}

.list-group {
  width: 15rem;
  display: flex;
  flex-direction: column;
  row-gap: 0.1rem;
}

.list1 .list-group-item {
  background-color: lightblue;
  border: solid 0.5px rgb(106, 164, 184);
}

.list2 .list-group-item {
  background-color: lightgreen;
  border: solid 0.5px rgb(93, 189, 93);
}

h3 {
  text-align: left;
}

.list-group-item {
  padding: 0.5rem;
  /* border: solid 0.5px gray; */
  text-align: left;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>

<script>
import List from './components/List.vue'

export default {
  components: {
    List
  }
}
</script>
