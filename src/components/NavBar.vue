<template>
    <v-app-bar app color="#111111" dark flat class="px-8">
        <v-btn color="red">
            <v-icon>
                mdi-home
            </v-icon>
        </v-btn>
        <v-spacer></v-spacer>
        <v-btn class="mx-2" color="red" @click="scroll('home')">Inicio</v-btn>
        <v-btn class="mx-2" color="red" @click="scroll('about')">Acerca de</v-btn>
        <v-btn class="mx-2" color="red" @click="scroll('project')">Proyectos</v-btn>
        <v-btn class="mx-2" color="red" @click="scroll('contact')">Contacto</v-btn>
    </v-app-bar>
</template>

<script>
export default {
    methods: {
        scroll(refName) {
            const element = document.getElementById(refName);
            element.scrollIntoView({behavior: "smooth"});
        }
    }
}
</script>

<style>
</style>