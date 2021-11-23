<template>
    <h1>Users</h1>

    <Nav />

    <div class="mt-40">
        <p>the current time is:{{ time }}</p>
        <Link href="/users" class="text-blue-400 hover:underline">Refresh</Link>
    </div>
</template>

<script>
import Nav from '../Shared/Nav.vue';
import { Link } from '@inertiajs/inertia-vue3';
export default {
    components:{
        Nav,
        Link
    },
    props:{
        time: String
    }
}
</script>

