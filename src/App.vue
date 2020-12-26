<template lang="pug">
    #app
        NavComponent
        NoiseComponent
        transition(name="fade" mode="out-in")
            router-view
</template>

<script>
// @ is an alias to /src
import NoiseComponent from '@/components/NoiseComponent.vue'
import NavComponent from "@/components/NavComponent";

export default {
    name: 'App',
    components: {
        NavComponent,
        NoiseComponent
    }
}
</script>

<style>
*{
    box-sizing: border-box;
}

html,
body{
    background-color: #FEDCC8;
}

#app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
}


.fade-enter-active,
.fade-leave-active {
    transition-duration: 0.3s;
    transition-property: opacity;
    transition-timing-function: ease;
}

.fade-enter,
.fade-leave-active {
    opacity: 0
}
</style>
