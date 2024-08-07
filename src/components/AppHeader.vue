<template>
  <header class="app-header">
    <h1>HRMS</h1>
  </header>
</template>

<script>
export default {
  name: 'AppHeader'
}
</script>

<style scoped>
.app-header {
  width: 100%;
  height: 60px;
  background-color: #333;
  color: white;
  display: flex;
  align-items: center;
  padding: 0 20px;
  box-sizing: border-box;
  position: fixed; /* Make the header fixed */
  top: 0;
  z-index: 1000;
}

.app-header h1 {
  margin: 0;
}
</style>