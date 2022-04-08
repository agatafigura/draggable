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
  column-gap: 1rem;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}

.list-group {
  width: 15rem;
  display: flex;
  flex-direction: column;
  row-gap: 0.3rem;
  margin-bottom: 0.5rem;
  min-height: 18rem;
}

.list1 .list-group-item {
  /* background-color: lightblue; */
  border: solid 0.5px rgb(243, 243, 155);
  border-left-width: 0.5rem;
}

.list2 .list-group-item {
  border: solid 0.5px lightblue;
  border-left-width: 0.5rem;
}

.list3 .list-group-item {
  border: solid 0.5px lightgreen;
  border-left-width: 0.5rem;
}

.list4 .list-group-item {
  border: solid 0.5px lightcoral;
  border-left-width: 0.5rem;
}

h3 {
  text-align: center;
  padding: 0.5rem;
  margin: 0;
}

#list1 h3 {
  background-color: rgb(243, 243, 155);
 }

 #list2 h3 {
   background-color: lightblue;
 }

 #list3 h3 {
   background-color: lightgreen;
 }

 #list4 h3 {
   background-color: lightcoral;
 }

.list-group-item {
  margin-left: 0.5rem;
  margin-right: 0.5rem;
  /* border: solid 0.5px gray; */
  text-align: left;
  padding: 0.5rem;
}

#list1 {
  border: rgb(211, 211, 44) 1px solid;
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  row-gap: 1rem;
}

#list2 {
   border: rgb(96, 187, 218) 1px solid;
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  row-gap: 1rem;
}

#list3 {
   border: rgb(41, 196, 41) 1px solid;
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  row-gap: 1rem;
}

#list4 {
   border: rgb(240, 76, 76) 1px solid;
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  row-gap: 1rem;
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
