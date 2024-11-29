<template>
    <div>
        {{ $route.query.page }}
        Úsuario <br>


        <button @click="login()">
            login
        </button>

    </div>
</template>


<script>
export default {
    created(){
        console.log(this.$route);
    },
    methods:{
        login(){
            this.$router.push('/about');
            console.log('Chegou...');
        }
    }
}
</script>