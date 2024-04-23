<template>
    <div class="bg-gray-800 flex text-white max-h-screen h-screen">
        <div class="w-64">
            <span class="font-semibold p-6 block opacity-90">skateboard</span>
            <nav class="p-6">
                <h3 class="opacity-50 uppercase font-semibold tracking-wiider mb-6">Menu</h3>

                <div class="space-y-6">
                    <MenuItem :icon="HomeIcon">Discover</MenuItem>
                    <MenuItem :icon="TrendingUpIcon">Trending</MenuItem>
                    <MenuItem :icon="TrendingUpIcon">Trending</MenuItem>
                    <MenuItem :icon="TrendingUpIcon">Trending</MenuItem>
                    <MenuItem :icon="TrendingUpIcon">Trending</MenuItem>
                </div>

            </nav>
        </div>


        <div class="p-5 flex-1">
            <header class="flex items-center justify-between">
                <InputSearch />
                <div>
                    <div class="flex items-center space-x-3">
                        <div class="w-10 h-10">
                            <Avatar class="rounded-full" />
                        </div>
                        <span>Wermenson</span>
                        <ChevronDownIcon class="w-4 h-4" />
                    </div>

                    <Notifications />
                </div>
            </header>
        </div>
    </div>
</template>

<script lang="ts" setup>
import MenuItem from './navs/MenuItem.vue';
import TrendingUpIcon from '../components/icons/TrendingUpIcon.vue';
import HomeIcon from '../components/icons/HomeIcon.vue';
import InputSearch from '../components/inputs/InputSearch.vue';
import Avatar from '../components/Avatar.vue';
</script>