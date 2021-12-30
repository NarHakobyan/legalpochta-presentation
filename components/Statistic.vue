<script setup lang="ts">
import { ref } from "vue";

const props = defineProps({
  count: {
    type: String,
    required: true,
  },
  text: {
    type: String,
    required: true,
  },
});

const count = ref(props.count);
const text = ref(props.text);
</script>

<template>
  <div flex="~ col auto" align="items-center">
      <b text="5xl" m="2">{{ count }}</b>
      <b>{{ text }}</b>
    </div>

    
</template>
