<script setup>
defineProps(['message'])
defineEmits(['update:message'])
</script>

<template>
    <div class="flex flex-col">
        <h1 class="text-2xl mb-10">{{ message }}</h1>
        <button @click="$emit('update:message', 'Update from Child Component')" class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded">Click</button>
    </div>
</template>