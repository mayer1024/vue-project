<template>
  <div v-bind:class="demo">{{data}}</div>
</template>

<script setup lang="ts">
  const data = 123
  const config = {
    styleId: 'show'
  }
  function setId() {
    config.styleId = 'hide'
  }
</script>


<style>
.container {
  width: 100px;
  height: 100px;
}
.show {
  background-color: red;
}
.hide {
  background-color: blue;
}
</style>