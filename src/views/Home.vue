<template>
  <div class="home">
    
    <Courses msg="Welcome to Your Vue.js App" />
  </div>
</template>

<script>
// @ is an alias to /src
import Courses from "@/components/Courses.vue";

export default {
  name: "Home",
  components: {
     Courses
  }
};
</script>
