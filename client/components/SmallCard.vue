<template>
        <NuxtLink :to="`/products/${cardImageInfo.id}`" class="card">
            <img class="image" :src="require(`~/assets/images/${cardImageInfo.image||'fe1.jpg'}`)" alt="">
        </NuxtLink>
</template>

<script>
    export default {
        props:['cardImageInfo']
    }
</script>

<style lang="sass" scoped>
    .card
        width: 24%
        height: 12.5rem
        overflow: hidden
        cursor: pointer
        border-radius: .5rem
        flex: auto
        

    .image
        width: 100%
        height: 100%
        object-fit: cover
        margin: 0px
        
</style>