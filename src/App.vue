<script setup>
import { ref, reactive, onMounted, nextTick, computed, watch } from 'vue';
import HelloWorld from './components/HelloWorld.vue';
import CustomInput from './components/CustomInput.vue';
const searchText = ref('hello');
</script>

<template>
  <HelloWorld msg="Vite + Vue" />
  <br />
  <CustomInput v-model="searchText" /> {{ searchText }}
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
