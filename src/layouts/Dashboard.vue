<template>
    <div class="bg-gray-800 flex text-white max-h-screen h-screen">
        <!-- Side bar -->
        <div class="w-64">
            <span class="font-semibold p-6 block opacity-90">CCN +++++++</span>
            <nav class="p-6">
                <h3 class="opacity-50 uppercase font-semibold tracking-wiider mb-6">Menu</h3>

                <div class="space-y-6">
                    <MenuItem :icon="HomeIcon">Página Inicial</MenuItem>
                    <MenuItem :icon="TrendingUpIcon">Renovações</MenuItem>
                    <MenuItem :icon="TrendingUpIcon">Emissões</MenuItem>
                    <MenuItem :icon="TrendingUpIcon">Comissões</MenuItem>
                    <MenuItem :icon="TrendingUpIcon">Vendas por mês</MenuItem>
                </div>

            </nav>
        </div>

        <!-- Searc e avatar + notificação -->
        <div class="p-5 flex-1">
            <header class="flex items-center justify-between">
                <InputSearch class="w-96"/>
                <div class="flex items-center">
                    <div class="flex items-center space-x-3">
                        <Avatar class="rounded-full overflow-hidden w-10 h-10" />
                        <span>Wermenson</span>
                        <ChevronDownIcon class="w-4 h-4" />
                    </div>

                    <BellIcon class="w-5 h-5 ml-8 opacity-50 hover:opacity-100 cursor-pointer transition durantion-100"/>
                </div>
            </header>

            <h1 class="font-bold text-4xl mt-6 mb-4">Descubra</h1>
            
            <div class="grid gap-4 grid-cols-12">

                <div class="col-span-8 h-96 rounded-3xl borde overflow-hidden relative">
                    <div class="flex w-full h-full">
                        <img src="../assets/img/banda.jpg" class="w-full object-cover">
                    </div>

                    <div class="z-10 absolute top-0 p-6 w-full bottom-0">
                        <h3 class="text-2xl max-w-xs">A melhor banda de rock!</h3>

                        <div class="absolute right-6 bottom-6 px-2 py-1 rounded-lg bg-gray-800 bg-opacity-50 text-white">🤘</div>
                    </div>
                </div>

                <div class="col-span-4 h-96 rounded-3xl borde overflow-hidden relative">
                    <div class="flex w-full h-full">
                        <img src="../assets/img/office_plaza.jpg" class="w-full object-cover">
                    </div>

                    <div class="z-10 absolute top-0 p-6 w-full bottom-0">
                        <h3 class="text-2xl max-w-xs">Protesto para aumento de salário!</h3>

                        <div class="absolute right-6 bottom-6 px-2 py-1 rounded-lg bg-gray-800 bg-opacity-50 text-white">💸</div>
                    </div>
                </div>

                
            </div>



        </div>


    </div>
</template>

<script lang="ts" setup>
import MenuItem from './navs/MenuItem.vue';
import TrendingUpIcon from '../components/icons/TrendingUpIcon.vue';
import HomeIcon from '../components/icons/HomeIcon.vue';
import InputSearch from '../components/inputs/InputSearch.vue';
import Avatar from '../components/Avatar.vue';
import ChevronDownIcon from '../components/icons/ChevronDownIcon.vue';
import BellIcon from '../components/icons/BellIcon.vue';
</script>