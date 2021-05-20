<template>
    <div class="card">
        <img :src="require(`~/assets/images/${card.image||'fe1.jpg'}`)" alt="fe" class="img-fluid image">
        <h3 class="header">{{card.title}}</h3>
        <p class="snippet">{{card.snippet}}</p>
    </div>
</template>

<script>
    export default {
        props:['card']
    }
</script>

<style lang="sass" scoped>

.card 
	width: 31.5% 
	height: 427px 
	border: none 
	overflow: hidden 
	padding: 0 
	cursor: pointer 

.image 
	border-radius: 0.5rem
    object-fit: cover
    min-height: 228px

.header 
	font-size: 1rem 
	margin-top: 0.4rem 

.snippet 
	color: grey 

</style>