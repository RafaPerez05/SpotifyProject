<script setup>
import AuthenticatedLayout from '@/Layouts/AuthenticatedLayout.vue';
import { Head } from '@inertiajs/vue3';
import MusicaList from '@/Components/MusicaList.vue'

</script>

<template>
    <Head title="Dashboard" />

    <AuthenticatedLayout>

        <!--MEXE AQUI PRA MEXER TUDO AS PARADA-->
        <div class="container mt-10 ml-10 p-4">
            <div class="flex">
                <!-- Conteúdo à esquerda -->
                <div class="bg-gray-800 p-4 rounded-lg shadow-md w-80 mr-4 h-40">
                    
                    <a href="#"
                        class="flex items-center space-x-4 text-gray-300 visited:text-slate-50 w-min divide-none mt-2">
                        <img src="../components/img/casa.png" alt="icone de casa" class="w-5 h-5">
                        <p class="ml-2">Início</p>
                    </a>
                    
                    <a href="#"
                        class="flex items-center space-x-4 text-gray-300 visited:text-slate-50 w-min divide-none mt-2">
                        <img src="../components/img/lupa.png" alt="icone de lupa" class="w-5 h-5">
                        <p class="ml-2">Buscar</p>
                    </a>

                        <a href="#"
                            class="flex items-center space-x-4 text-gray-300 visited:text-slate-50 w-max divide-none mt-2 mb-4">
                            <img src="../components/img/biblioteca.png" alt="icone de lupa" class="w-6 h-6">
                            <p class="ml-4">Sua Biblioteca</p>
                            <img src="../components/img/plus.png" alt="icone de mais, para criar playlist"
                                class="w-6 h-6 ml-32">
                        </a>

                        <div class="bg-gray-800 p-4 rounded-lg shadow-md w-74 mb-4">
                            <p class="text-white h-9">Crie sua primeira playlist</p>
                            <p class="text-white text-sm h-10">É fácil, vamos te ajudar</p>
                            <button class="bg-white text-black rounded-full h-8 w-32">Criar playlist</button>
                        </div>
                        <div class="bg-gray-800 p-4 rounded-lg shadow-md w-74 ">
                            <p class="text-white h-9">Que tal seguir um podcast novo?</p>
                            <p class="text-white text-sm h-10">Avisaremos você sobre novos episódios</p>
                            <button class="bg-white text-black rounded-full h-8 w-36">Explore podcasts</button>
                        </div>
                </div>


        <!-- Conteúdo à direita -->
        <div class="bg-gray-800 p-4 rounded-xl shadow-md w-74 mb-3">
            <h1 class="text-xl mt-4 text-white py-2">Playlists do Spotify</h1>
            <div class="flex space-x-3">
               <MusicaList />
            </div>
            <p class="text-white h-40 px-2"></p>
        </div>
    </div>
    </div>
    </AuthenticatedLayout>
</template>