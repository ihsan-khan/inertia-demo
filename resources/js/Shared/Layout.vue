<template>
    <section class="p-6 bg-gray-200">
    <header class="flex justify-between">
        <div class="font-bold text-lg">
            My App
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
    }
}
</script>