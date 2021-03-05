<template>
    <!-- This template is a wrapper for both products/index.vue and any other nested route -->
    <section>
        <h2>Products Page</h2>
        <nuxt-link to="/products/123">Go to products/123</nuxt-link>
        <nuxt-link to="/products/qwerty">Invalid link to products/qwerty</nuxt-link>
        <nuxt-link to="/">Home</nuxt-link>
        <!-- marks the place where the nested routes should be loaded -->
        <nuxt-child></nuxt-child>
    </section>
</template>

<script>
export default {
    // property provided by Nuxt
    // pass a string corresponding to a layout
    layout: 'custom',
}
</script>