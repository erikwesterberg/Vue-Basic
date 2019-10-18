<template>
  <div id="app">
    <Header />
    <Todos v-bind:todos="todos" v-on:del-todo="deleteTodo" />
  </div>
</template>

<script>
import Header from "./components/layout/Header";
import Todos from "./components/Todos";

export default {
  name: "app",
  components: {
    Header,
    Todos
  },
  data() {
    return {
      todos: [
        {
          id: 0,
          title: "Learn Vue and then look at Nuxt",
          completed: false
        },
        {
          id: 1,
          title: "Enjoy it",
          completed: false
        },
        {
          id: 2,
          title: "Drink beer",
          completed: true
        },
        {
          id: 3,
          title: "Refactor code",
          completed: false
        }
      ]
    }
  },

  methods: {
    deleteTodo(id) {
      this.todos = this.todos.filter(todo => todo.id !== id);
    }
  }
};
</script>

<style>
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

body {
  font-family: Arial, Helvetica, sans-serif;
  line-height: 1.4;
}
</style>
