<template>
    <h3>Mike is on</h3>
</template>

<script setup>
  import { onUnmounted } from 'vue';

  onUnmounted(()=>{
    console.log("Mike-Onunmounted");
  })

</script>