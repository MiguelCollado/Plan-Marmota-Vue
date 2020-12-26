<template lang="pug">
    #noise
</template>

<script>
export default {
    name: "NoiseComponent"
}
</script>

<style scoped lang="scss">
#noise {
    position: fixed;
    left: 0;
    top: 0;
    right: 0;
    bottom: 0;
    z-index: 999;
    width: 100%;
    height: 100%;
    background-image: url("../assets/noise.gif");
    background-position: 0 0;
    opacity: 0.04;
    pointer-events: none;
}
</style>