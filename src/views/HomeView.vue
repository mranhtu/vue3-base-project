<template>
  <main>
    <TheWelcome />
    <DetailView :msg="'hello'" />
  </main>
</template>

<script setup lang="ts">
import TheWelcome from '../components/TheWelcome.vue'
import DetailView from "@/views/DetailView.vue";
</script>
