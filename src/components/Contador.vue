<script>
    export default {
        data: () => ({
            count : 0,
        }),
        props:{
            nombreClase:String
        }
    };
</script>
<template>
    <button :class="nombreClase" v-on:click="count++"> Click {{count}} veces</button>
</template>