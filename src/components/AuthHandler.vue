<template>
    <div>Please wait haho ...</div>
</template>

<script>
    import {mapActions} from 'vuex';
    export default {
        name: "AuthHandler",
        methods : mapActions(['finalizeLogin']),
        created(){
            console.log('created!!!');
            this.finalizeLogin(window.location.hash);
        }
    }
</script>

<style scoped>

</style>