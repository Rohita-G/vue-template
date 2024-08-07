<template>
  <div id="app">
    <AppHeader />
    <div class="container">
      <LeftSidebar />
      <MainContent />
      <RightSidebar />
    </div>
  </div>
</template>

<script>
import AppHeader from './components/AppHeader.vue';
import LeftSidebar from './components/LeftSidebar.vue';
import RightSidebar from './components/RightSidebar.vue';
import MainContent from './components/MainContent.vue';

export default {
  name: 'App',
  components: {
    AppHeader,
    LeftSidebar,
    RightSidebar,
    MainContent
  }
}
</script>

<style>
body {
  margin: 0;
  font-family: Avenir, Helvetica, Arial, sans-serif;
}
#app {
  display: flex;
  flex-direction: column;
  height: 100vh;
  overflow: hidden;
}
.container {
  display: flex;
  flex: 1;
  margin-top: 60px; /* Prevent content from going under the fixed header */
}
</style>