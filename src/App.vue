<template>
    <v-app>
        <!-- sidebar -->
        <SideBar/>

        <v-main>
            <!-- cards-->
            <ImageGallery />
        </v-main>

    </v-app>
</template>

<script setup>
import SideBar from "@/components/SideBar.vue";
import ImageGallery from "@/components/ImageGallery.vue";
</script>