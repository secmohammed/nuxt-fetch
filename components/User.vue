<template>
    <div>
        {{ user }}
    </div>
</template>
<script>
    export default {
        props: {
            id: {
                required: true
            }
        },
        data() {
            return {
                user: null
            }
        },
        async fetch() {
            let user = await this.$axios.$get(`https://jsonplaceholder.typicode.com/users/${this.id}`)
            this.user = user
        }
    }
</script>