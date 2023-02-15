<template>
  <div>
    <p>detail</p>
    <p>Data Input: {{ dataInput?.msg }}</p>
  </div>
</template>

<script setup lang="ts">
import { onMounted, ref } from "vue";

interface Props {
  msg: string;
  bar?: number;
}

const dataInput = defineProps<Props>();
const hasObject = ref();

onMounted(() => {
  console.log(dataInput.msg);
  hasObject.value = false;

});
</script>

<style scoped></style>
