<template>
    <v-navigation-drawer expand-on-hover rail>
        <v-list>
            <v-list-item
                    prepend-avatar="https://randomuser.me/api/portraits/women/85.jpg"
                    title="Sandra Adams"
                    subtitle="sandra_a88@gmail.com"
            >
            </v-list-item>
            <v-divider/>
            <v-list density="compact" nav>
                <v-list-item prepend-icon="mdi-image" title="Color Gallery" value="color"
                             @click="selectOption(true)"></v-list-item>
                <v-list-item prepend-icon="mdi-dialpad" title="Grayscale Gallery" value="gray"
                             @click="selectOption(false)"></v-list-item>
            </v-list>
        </v-list>

    </v-navigation-drawer>

</template>

<script setup>
import {defineEmits} from 'vue';

const emits = defineEmits(['selectOption']);

const selectOption = (isColor) => {
    emits("selectOption", isColor);
}
</script>

<style scoped>

</style>