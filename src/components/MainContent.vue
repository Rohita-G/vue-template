<template>
  <div class="main-content">
    <div v-for="item in 100" :key="item" class="content-item">
      Content Item {{ item }}
    </div>
  </div>
</template>

<script>
export default {
  name: 'MainContent'
}
</script>

<style scoped>
.main-content {
  flex: 1;
  padding-top: 60px; /* Adjust based on header height */
  overflow-y: auto;
  height: calc(100vh - 60px); /* Ensure full height minus the header */
  box-sizing: border-box;
}

.content-item {
  margin: 10px;
  padding: 10px;
  border: 1px solid #ccc;
}
</style>