<template>
    <div class="container">
        <h3 class="header">{{smallCardSection.title}}</h3>
        <div class="card-container">
            <SmallCard 
                v-for="cardImage in smallCardSection.cards"
                :key="cardImage.id"
                :cardImageInfo="cardImage"
            />  
        </div>    
    </div>

</template>

<script>
    export default {
        props:['smallCardSection']
    }
</script>

<style lang="sass" scoped>

    .container 
        padding: 2rem 0 
    .header 
        font-weight: 700 
        font-size: 1.5rem 
        margin-bottom: 2rem 
    .card-container 
        display: flex 
        justify-content: space-between 
        flex-wrap: wrap 
        gap: 14px

</style>