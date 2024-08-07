<template>
  <div class="sidebar">
    <div v-for="button in 100" :key="button" class="sidebar-button">
      Button {{ button }}
    </div>
  </div>
</template>

<script>
export default {
  name: 'RightSidebar'
}
</script>

<style scoped>
.sidebar {
  width: 200px;
  height: calc(100vh - 60px); /* Adjust based on header height */
  padding-top: 60px; /* Prevent content from going under header */
  overflow-y: auto;
  background-color: #f4f4f4;
  box-sizing: border-box;
}

.sidebar-button {
  padding: 10px;
  border: 1px solid #ccc;
  margin: 5px 0;
}
</style>