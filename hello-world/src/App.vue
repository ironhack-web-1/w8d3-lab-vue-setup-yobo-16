<template>
  <div>
    <AboutUs></AboutUs>
    <ToDoItem></ToDoItem>
  </div>
</template>

<script>
import AboutUs from "./components/AboutUs.vue";
import ToDoItem from "./components/ToDoItem.vue";
export default {
  name: "App",
  components: {
    ToDoItem,
    AboutUs,
  },
};
</script>

<style></style>
