<template>
    <section>
        <h2>Products {{ id }}</h2>
        <nuxt-link to="/products">Back to products</nuxt-link>
    </section>
</template>

<script>
export default {
    // method provided by Nuxt
    // validating url
    validate(data) {
        console.log(data);

        // only allow numbers
        return /^\d+$/.test(data.params.id);
    },
    computed: {
        id() {
            return this.$route.params.id;
        }
    },
}
</script>