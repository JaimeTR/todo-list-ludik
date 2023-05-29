<template>
  <div id="app">
    <task v-bind:tasks="tasks"></task>
  </div>
</template>

<script>
import Task from "./components/Task.vue";

export default {
  name: "App",
  components: {
    Task,
  },
  data() {
    return {
      tasks: [
        {
          id: 1,
          title: "Aprendo Vue.js",
          completed: true,
        },
        {
          id: 2,
          title: "Trabajo en Ludik",
          completed: true,
        },
        {
          id: 3,
          title: "Me voy de paseo",
          completed: false,
        },
        {
          id: 4,
          title: "Hago la tarea",
          completed: false,
        },
        {
          id: 5,
          title: "Envio correos",
          completed: false,
        },
      ],
    };
  },
};
</script>