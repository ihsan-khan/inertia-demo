<template>
    <Layout>
        <h1 class="text-4xl">Users</h1>
    </Layout>
</template>

<script>
import Layout from '../Shared/Layout.vue';
import { Link } from '@inertiajs/inertia-vue3';
export default {
    components:{
        Layout,
        Link
    },
    props:{
        time: String
    }
}
</script>

