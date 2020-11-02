<template>
  <li>
    <span>
      {{ item.title }}
    </span>
  </li>
</template>

<script>
export default {
  name: "MenuItem",
  props: {
    item: {
      type: Object,
      required: true
    },
    index: Number
  }
}
</script>

<style scoped>
li {
  transition: 0.2s ease-in;
  list-style: none;
  color: white;
  margin: 5px;
  padding: 5px 15px;
  cursor: pointer;
  text-transform: uppercase;
  font-weight: bold;
  border-bottom: 2px solid transparent;
}

li:hover {
  transition: 0.2s ease-out;
  color: #ff7a06;
  border-bottom: 2px solid #888888;
}
</style>