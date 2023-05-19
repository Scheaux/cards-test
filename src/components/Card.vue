<script lang="ts">
export default {
    props: ['title', 'body', 'icon'],
};
</script>

<template>
    <div class="flex flex-col gap-4 shadow-md bg-white p-12">
        <img v-bind:src="icon" class="w-[60px]" alt="icon2" />
        <h3 class="text-xl font-semibold">{{ title }}</h3>
        <p class="font-light">{{ body }}</p>
    </div>
</template>
