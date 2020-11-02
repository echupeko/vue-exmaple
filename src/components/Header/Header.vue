<template>
  <div>
    <MenuList
        v-bind:menuList="menuList"/>
  </div>
</template>

<script>
import MenuList from "@/components/Header/MenuList";

export default {
  name: "Header",
  props: {
    menuList: Array
  },
  components: {
    MenuList
  }
}
</script>

<style scoped>
div {
  position: absolute;
  display: block;
  left: 0;
  right: 0;
}
</style>