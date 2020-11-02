<template>
  <div>
    <ul>
      <MenuItem
          v-for="(item, i) in menuList"
          v-bind:item="item"
          v-bind:index="i"
      />
    </ul>
  </div>
</template>

<script>
import MenuItem from '@/components/Header/MenuItem';

export default {
  name: 'ToDoList',
  props: ['menuList'],
  components: {
    MenuItem
  },
  methods: {}
}
</script>

<style scoped>
ul {
  display: inline-flex;
  flex-direction: row;
  align-items: center;
  height: 50px;
  margin: 0;
  padding: 0;
  background-color: rgba(48, 48, 48, 0.9);
  border: 2px solid rgba(153, 153, 153, 0.45);
}
</style>