<script  setup lang="ts">
const icons = [
    'mdi-facebook',
    'mdi-twitter',
    'mdi-google-plus',
    'mdi-linkedin',
    'mdi-instagram'
]
</script>
<template>
    <!-- <v-card height="auto" class="pa-10 mt-4"> -->
        <v-card flat tileclass="text-xs-center" class="mt-5">
            <v-card-text>
                <v-btn v-for="icon in icons" :key="icon" class="mx-3 white--text" icon>
                    <v-icon size="24px">{{ icon }}</v-icon>
                </v-btn>
            </v-card-text>

            <v-card-text class="white--text pt-0">
                Phasellus feugiat arcu sapien, et iaculis ipsum elementum sit amet. Mauris cursus commodo interdum. Praesent
                ut risus eget metus luctus accumsan id ultrices nunc. Sed at orci sed massa consectetur dignissim a sit amet
                dui. Duis commodo vitae velit et faucibus.
            </v-card-text>

            <v-divider></v-divider>

            <v-card-text class="white--text">
                &copy;2018 — <strong>Vuetify</strong>
            </v-card-text>
        </v-card>
    <!-- </v-card> -->
</template>
<style scoped></style>
  