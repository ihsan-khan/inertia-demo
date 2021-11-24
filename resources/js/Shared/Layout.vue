<template>
    <section class="p-6 bg-gray-200">
    <header class="flex justify-between">
        <div class="flex item-center">
           <h1 class="font-bold text-lg"> My App </h1>
           <p class="font-sm ml-4 mt-1">Welcome back - {{ username }}</p>
        </div>
        <Nav />

    </header>

    </section>
    <section class="p-6">
    <div class="max-w-3xl mx-auto">
      <slot />

    </div>

    </section>
</template>

<script>
import Nav from '../Shared/Nav.vue';
export default {
    components:{
        Nav
    },
    computed:{
        username(){
            return this.$page.props.auth.user.username;
        }
    }
}
</script>