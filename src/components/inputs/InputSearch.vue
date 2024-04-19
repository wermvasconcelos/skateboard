<template>
    <div class="relative text-white">
        <input type="text" class="w-full bg-gray-700 placeholder-white px-4 py-2 rounded-lg opacity-30 focus:opacity-60 outiline-none focus:outiline-none pr-10" placeholder="Pesquisar">
        <SearchIcon class="w-4 h-4 absolute top-2.5 right-2.5"/>
    </div>
</template>

<script lang="ts" setup>
    import SearchIcon from "../icons/SearchIcon.vue";
</script>