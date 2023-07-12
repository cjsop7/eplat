<script setup lang="ts">
import { ref } from "vue";
import firstImage from '@/assets/first.jpg'
import secondImage from '@/assets/second.jpg'
import thirdImage from '@/assets/third.jpg'

// const slides = ref(['first','second','third'])
const slides = ref([firstImage, secondImage, thirdImage])

</script>

<template>
    <v-container class="pa-0 ma-0" fluid>
            <v-card class="mx-auto fill-height">
                <v-carousel class="mx-auto fill-height" continuous show-arrows="hover" hide-delimiters delimiter-icon="mdi-square" color="primary">
                    <v-carousel-item v-for="(slide, i) in slides" :key="i">
                        <v-container class="fill-height pa-0">
                            <v-img :src=slide aspect-ratio="1" style="width:1600px;height:900px"></v-img>
                        </v-container>
                    </v-carousel-item>
                </v-carousel>
            </v-card>
            <v-card class="my-5">
                <v-img :src=firstImage />
            </v-card>
            <v-card class="my-5">
                <v-img :src=secondImage />
            </v-card>
            <v-card class="my-5">
                <v-img :src=thirdImage />
            </v-card>
    </v-container>
</template>

<style scoped></style>