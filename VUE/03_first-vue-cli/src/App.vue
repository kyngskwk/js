<template>
  <div id="app">
    <hr>
    <!-- step3. 사용한다. -->
    <MyComponent />
    <!-- <GreateComponent /> -->
  </div>
</template>

<script>
// 컴포넌트 사용하기
// step1. import 한다
import MyComponent from './components/MyComponent.vue'
// import GreateComponent from './components/GreateComponent.vue'
export default {
  name: 'App',
  components: {
    // step2. 등록한다.
    MyComponent,
    // GreateComponent,
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
