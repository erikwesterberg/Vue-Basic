<template>
  <div id="app">
    
  </div>
</template>

<script>

export default {
  name: 'app',
  components: {
 
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
  }
}
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
