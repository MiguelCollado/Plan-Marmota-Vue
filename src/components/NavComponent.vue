<template lang="pug">
    nav
        router-link(to="/") Home
        router-link(to="/about") About
</template>

<script>
export default {
    name: "NavComponent"
}
</script>

<style scoped lang="scss">
nav {
    display: flex;
    flex-direction: row;
    justify-content: left;
    align-items: center;
    position: sticky;
    top: 0;
    left: 0;
    z-index: 1;
    padding: 30px;

    a {
        margin-right: 2em;
    }
}

nav a {
    font-weight: bold;
    color: #2c3e50;
}

nav a.router-link-exact-active {
    color: #42b983;
}
</style>