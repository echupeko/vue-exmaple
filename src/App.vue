<template>
  <div id="app">
    <Header
        v-bind:menuList="menuList"
    />
    <AboutMe/>
  </div>
</template>

<script>
import Header from './components/Header/Header';
import AboutMe from '@/components/AboutMe/AboutMe';

export default {
  name: 'App',
  data() {
    return {
      menuList: [
        {id: 0, title: 'Навыки'},
        {id: 1, title: 'Работа'},
        {id: 2, title: 'Обучение'},
        {id: 3, title: 'Увлечения'},
        {id: 4, title: 'Контакты'}
      ]
    }
  },
  components: {
    Header,
    AboutMe
  }
}
</script>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css2?family=Open+Sans&family=Roboto&display=swap');
#app {
  font-family: 'Roboto', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;

}
</style>
