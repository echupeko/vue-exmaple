<template>
  <div>
    <MeInfo/>
  </div>
</template>

<script>
import MeInfo from "@/components/AboutMe/MeInfo";

export default {
  name: "AboutMe",
  components: {
    MeInfo
  }
}
</script>

<style scoped>
div {
  background-image: url("/about-background.png");
  background-color: #2c3e50;
  background-size: cover;
  height: 850px;
}
</style>