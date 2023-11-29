<template>
  <div class="flex p-10 justify-center">
    <input type="text" class="rounded-2xl border-2 border-gray-400" />
    {{ meals }}
  </div>
</template>

<script setup lang="ts">
import { computed } from "vue";
import store from "../store";

const meals = computed(() => store.state.meals);
</script>

<style scoped></style>
