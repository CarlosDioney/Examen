<template>
    <Grid>
        <slot></slot>
        <h2>{{ nombre }}</h2>
        <h4>{{ descripcion }}</h4>
        <h4>{{ costo }}</h4>
        <a :href="url" target="_blank">Comprar</a>
    </Grid>
</template>

<script>
    import Grid from "./Grid.vue";
    export default{
    props: {
        nombre: {
            String,
        },
        descripcion: {
            String,
        },
        costo: {
            String,
        },
    },
    components: { Grid },
};
</script>

<style scopet>

    img{
        width: 8rem;
        height: 8rem;
        padding: 0.5rem;
        background: snow;
    }
    a{
        text-decoration: none;
        color: rgb(255, 255, 255);
        background: #b85900cc;
        padding: 0.3rem;
        border-radius: 5px;
        border: 1px solid #ffffff;
    }
</style>