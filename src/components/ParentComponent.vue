<script setup>
import { reactive, ref } from 'vue';
import Child from './ChildComponent.vue';

const data = reactive({
    message: 'Data from Parent'
})
</script>

<template>
    <Child v-model:message="data.message" />
</template>