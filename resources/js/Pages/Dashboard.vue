<script setup>
import AuthenticatedLayout from '@/Layouts/AuthenticatedLayout.vue';
import { Head } from '@inertiajs/vue3';
import ChatLeftsidebar from '@/Components/ChatLeftsidebar.vue';
import UserChat from '@/Components/UserChat.vue';
</script>

<template>
    <Head title="Dashboard" />

    <AuthenticatedLayout>
        <template #header>
            <h2 class="font-semibold text-xl text-gray-800 leading-tight">Dashboard</h2>
        </template>

        <div class="py-12">
            <div class="max-w-8xl mx-auto sm:px-6 lg:px-7">
                <div class="bg-white overflow-hidden shadow-sm sm:rounded-lg layout-wrapper">
                    <!-- <div class="main-content"> -->
                    <div class="page-content">
                        <div class="container-fluid">
                            <div class="d-lg-flex">

                                <ChatLeftsidebar />

                                <UserChat />

                            </div>
                        </div>
                    </div>
                    <!-- </div> -->
                </div>
            </div>
        </div>
    </AuthenticatedLayout>
</template>