<template>

  <div class="container">
	<Hero />
	<LargeCardDisplay 
		v-for="cardInfo in LargeCardInfo"
		:key="cardInfo.id"
		:cardsSection="cardInfo"
		/>
  <SmallCardDisplay 
    v-for="smallCard in SmallCardInfo" 
    :key="smallCard.id"
    :smallCardSection="smallCard"
  />

  </div>
</template>

<script>
import { largeCardSections, smallCardSections } from "@/assets/data.js"
export default {
        data() {
            return {
              LargeCardInfo:  largeCardSections,
              SmallCardInfo: smallCardSections
            }
        },	
}
</script>


<style>

</style>
