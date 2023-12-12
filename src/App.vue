<template>
    <main id="app">
        <router-view/>
    </main>
</template>
<script>
import { RouterLink, RouterView } from 'vue-router'
import HomeView from '../src/views/HomeView.vue'

export default {
    name: 'App',
    components: {
        RouterLink,
        RouterView,
        HomeView
    }
}
</script>
