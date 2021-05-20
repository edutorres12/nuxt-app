<template>
  <div class="container">
	<Hero />
	<LargeCardDisplay 
		v-for="cardInfo in LargeCardInfo"
		:key="cardInfo.id"
		:cardsSection="cardInfo"
		/>

  </div>
</template>

<script>
import { largeCardSections } from "@/assets/data.js"
export default {
        data() {
            return {
             LargeCardInfo:  largeCardSections 
            }
        },	
}
</script>


<style>

</style>
