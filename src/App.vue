<template>
  <div id="app">
    <div id="nav">
      <app-header/>
    </div>
    <router-view/>
  </div>
</template>
<script>
  import Header from './components/Header.vue'
export default {
  components: {
    'app-header': Header
  }
}
</script>