<template>
  <div>
    <div class="container">
      <Header />
      <Tasks :tasks="tasks"/>
    </div>
  </div>
</template>

<script>
import Header from "./components/Header";
import Tasks from './components/Tasks'

export default {
  name: "App",
  components: {
    Header,
    Tasks,
  },
  data() {
    return {
      task: [],
    };
  },
  created() {
    this.task = [
      {
        id: 1,
        text: "Doctors Appointment",
        day: "March 1st at 2:30",
        reminder: true,
      },
      {
        id: 2,
        text: "Design Appointment",
        day: "April 1st at 2:30",
        reminder: false,
      },
      {
        id: 3,
        text: "Developer Appointment",
        day: "Mayu 1st at 2:30",
        reminder: true,
      },
    ];
  },
};
</script>

<style scoped>
.container {
  width: 600px;
  height: 300px;
  border: 1px solid black;
}
</style>