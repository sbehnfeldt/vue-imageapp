<template>
    <v-app>
        <!-- sidebar -->
        <SideBar @select-option="onSelectOption"/>

        <v-main>
            <!-- cards-->
            <ImageGallery :asGrayscale="!isWithColor" />
        </v-main>

    </v-app>
</template>

<script setup>
import SideBar from "@/components/SideBar.vue";
import ImageGallery from "@/components/ImageGallery.vue";
import {ref} from "vue"

const isWithColor = ref(true);
const onSelectOption = (withColor) => {
    isWithColor.value = withColor;
}
</script>