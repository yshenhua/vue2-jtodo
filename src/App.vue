<template>
  <div id="app">
    <Header/>
    <Todo/>
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Header'
import Todo from './components/Todo'
import Footer from './components/Footer'

export default {
  name: 'App',
  components: {
    Header,
    Todo,
    Footer
  }
}
</script>

<style lang="scss" scoped>
#app {
  position: absolute;
  left: 0;
  right: 0;
  top: 0;
  bottom: 0;
  &::before {
    content: '';
    position: absolute;
    left: 0;
    top: 0;
    right: 0;
    bottom: 0;
    z-index: -1;
    background-color: #999;
    opacity: .9;
  }
}
</style>
