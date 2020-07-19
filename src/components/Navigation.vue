<template>
    <div>
        <h4>
            <router-link to="/">Categories</router-link>
        </h4>
        <div id="nav" v-for="page in pages" :key="page">
            <div class="mt-3">
                <router-link :to="'/' + page">{{ capitalizeFirstLetter(page) }}</router-link>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data: () => {
        return {
            pages: ["appetizer", "specials", "salads", "seafoods", "traditional"],
        }
    },
    methods: {
        capitalizeFirstLetter(str) {
            return str.charAt(0).toUpperCase() + str.slice(1)
        },
    },
}
</script>

<style lang="scss" scoped>
a {
    color: black;
}
</style>
