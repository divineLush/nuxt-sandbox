<template>
    <section>
        <h1>Products {{ id }}</h1>
        <nuxt-link to="/">Home</nuxt-link>
    </section>
</template>

<script>
export default {
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