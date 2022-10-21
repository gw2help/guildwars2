<template>
    <div class="row bg-nav rounded py-3 mx-0 border-bottom border-primary navBar" style="min-width:800px">
		<div class="col-3 ms-5 row" style="min-width:380px">		
			<router-link :to="{ name: 'progress' }" class="navBtn achievBtn"> <div class="col-2 px-auto mx-auto border border-primary bg-darkz roundedz text-white navBtn"> <img class="w-100" src="../img/main/gui_achievements2.png"></div> </router-link>
        	<router-link :to="{ name: 'armor' }" class="navBtn armorBtn"> <div class="col-2 mx-auto border border-primary bg-darkz roundedz text-white navBtn"><img class="w-100" src="../img/main/gui_armor2.png"></div> </router-link>
			<router-link :to="{ name: 'build' }" class="navBtn buildBtn"> <div class="col-2 mx-auto border border-primary bg-darkz roundedz text-white navBtn"><img class="w-100" src="../img/main/gui_build2.png"></div> </router-link>
			<router-link :to="{ name: 'crafting' }" class="navBtn craftBtn"> <div class="col-2 mx-auto border border-primary bg-darkz roundedz text-white navBtn"><img class="w-100" src="../img/main/gui_crafting2.png"></div> </router-link>
			<router-link :to="{ name: 'timers' }" class="navBtn masteryBtn"> <div class="col-2 mx-auto border border-primary bg-darkz roundedz text-white navBtn"><img class="w-100" src="../img/main/gui_mastery2.png"></div> </router-link>
			<router-link :to="{ name: 'killproof' }" class="navBtn storyBtn"> <div class="col-2 mx-auto border border-primary bg-darkz roundedz text-white navBtn"><img class="w-100" src="../img/main/gui_story2.png"></div> </router-link>
            <router-link :to="{ name: 'mf_weapon_prices'}" class="navBtn mfBtn"> <div class="col-2 mx-auto border border-primary bg-darkz roundedz text-white navBtn"><img class="w-100" src="../img/main/gui_mysticforge2.png"></div> </router-link>
		</div>
	<!--
		<div class="col-3 mx-auto row" >
			<router-link 	
					:to="{name: 'itemfinder'}" 
					@mouseover="hovered = true"
					@mouseleave="hovered = false"
        			:class="{'link-hover': hovered}"
					class="mf_upgradeBtn navBtn mx-auto"><div width="42px" height="42px" class="col-2 mx-auto border border-primary bg-dark roundedz text-white navBtn"><img class="w-100 roundedz" src="../img/main/map_bank.png"></div></router-link>

		
		</div>
	-->
		<!--	
			<div class="col-3">
				<div class="row">				
					<input type="text" class="token roundedz border-primary mx-auto text-center text-white d-block bg-black" placeholder="paste-> api_key" style="min-width: 190px" value="10A33C63-85D8-D743-ABCD-B0219626D384F1D1A5B1-BADF-484D-81D4-65FF16D6B218">
				</div>
			</div>
		-->

		<div class="col-3 row">
			<router-link :to="{ name: 'builds' }" class="navBtn">
				<div class="col-2 mx-auto border border-primary bg-darkz roundedz text-white navBtn"><img class="w-100" src="../img/main/gui_mysticforge2.png"></div> 
			</router-link>
			<router-link 	
					:to="{name: 'itemfinder'}" 
					@mouseover="hovered = true"
					@mouseleave="hovered = false"
        			:class="{'link-hover': hovered}"
					class="mf_upgradeBtn navBtn"><div class="col-2 mx-auto border border-primary bg-dark roundedz text-white navBtn">
						<img class="w-100 roundedz" src="../img/main/map_bank.png"></div>
			</router-link>
			<router-link 	
					:to="{name: 'salvage'}" 
					@mouseover="hovered = true"
					@mouseleave="hovered = false"
        			:class="{'link-hover': hovered}"
					class="mf_upgradeBtn navBtn"><div class="col-2 mx-auto border border-primary bg-dark roundedz text-white navBtn">
						<img class="w-100 roundedz" src="../img/main/salvage_kit.png"></div>
			</router-link>
		</div>

		<div class="col-3 ms-auto me-0 row" style="min-width:380px">
			<!--
			<div class="row mx-auto text-center">
				
				<div class="col-4 navBtnz ml-2 ml-md-0">
					<button 
						class="btnGo border border-primary bg-dark roundedz text-white text-bold py-2 px-3" 
						@click="$emit('apiSearch')"><b> SEARCH </b>
					</button>
				</div>
				-->
				<!--
					<div class="col-2 mx-auto ml-md-2  mt-2 mt-md-0">

						router-link class="link" :to"{ name: 'xx' }" 
							class="ml-2 border border-primary bg-dark roundedz text-white py-2 px-3" 
							onclick="swap()"> <b> SWAP </b>
						</router-link>

						<img width="42px" height="42px" class="border border-primary roundedz grayedOut navBtnz" src="../img/main/shiny_bauble.png">
	
					</div>
				-->
				
				<router-link 	
					:to="{name: 'mf_upgrade'}" 
					@mouseover="hovered = true"
					@mouseleave="hovered = false"
        			:class="{'link-hover': hovered}"
					class="mf_upgradeBtn navBtn">
					<div width="42px" height="42px" class="col-2 mx-auto border border-primary bg-dark roundedz text-white navBtn">
						<img class="w-100 roundedz" src="../img/main/mystic_forge.png" alt="MF upgrades">
					</div>
				</router-link>

				<router-link 	
					:to="{name: 'attribute'}" 
					@mouseover="hovered = true"
					@mouseleave="hovered = false"
        			:class="{'link-hover': hovered}"
					class="attributeBtn navBtn"><div width="42px" height="42px" class="col-2 mx-auto border border-primary bg-dark roundedz text-white navBtn"><img class="w-100 roundedz" src="../img/main/map_vendor_weapons.png"></div></router-link>

				<router-link 	
					:to="{name: 'foodies'}" 
					@mouseover="hovered = true"
					@mouseleave="hovered = false"
        			:class="{'link-hover': hovered}"
					class="foodiesBtn navBtn"><div width="42px" height="42px" class="col-2 mx-auto border border-primary bg-dark roundedz text-white navBtn"><img class="w-100 roundedz" src="../img/main/map_craft_cooking.png"></div></router-link>

				<router-link 	
					:to="{name: 'rune'}" 
					@mouseover="hovered = true"
					@mouseleave="hovered = false"
        			:class="{'link-hover': hovered}"
					class="testBtn navBtn"><div width="42px" height="42px" class="col-2 mx-auto border border-primary bg-dark roundedz text-white navBtn"><img class="w-100 roundedz" src="../img/main/rune.png"></div></router-link>
				
				<router-link 	
					:to="{name: 'sigil'}" 
					@mouseover="hovered = true"
					@mouseleave="hovered = false"
        			:class="{'link-hover': hovered}"
					class="testBtn navBtn"><div width="42px" height="42px" class="col-2 mx-auto border border-primary bg-dark roundedz text-white navBtn"><img class="w-100 roundedz" src="../img/main/sigil.png"></div></router-link>

				<router-link 	
					:to="{name: 'provisioner'}" 
					@mouseover="hovered = true"
					@mouseleave="hovered = false"
        			:class="{'link-hover': hovered}"
					class="provisionBtn ml-2 navBtn"><div width="42px" height="42px" class="col-2 mx-auto border border-primary bg-dark roundedz text-white navBtn"><img class="w-100 roundedz" src="../img/main/provisioner_token.png"></div></router-link>
				
				<router-link 	
					:to="{name: 'converters'}" 
					@mouseover="hovered = true"
					@mouseleave="hovered = false"
        			:class="{'link-hover': hovered}"
					class="convertersBtn navBtn"><div width="42px" height="42px" class="col-2 mx-auto border border-primary bg-dark roundedz text-white navBtn"><img class="w-100 roundedz" src="../img/main/herta.png"></div></router-link>

				
			<!--
			</div>
			-->
		</div>
	</div>
	<div class="fakeNav py-3 py-md-5"></div>
</template>

<script>
export default {
    name: 'Nav',
    data(){
      return{
      	

      }
    },
    props:{
        
    },
    methods:{
		hoverBorder(){
			
		},
		/*
		clickParent(){ // comp B , wil method van comp A gebruiken
			this.$root.$emit('apiSearch');
		}
		*/
    }
}
</script>

<style scoped>
    .navBtn{
		width: 40px;
    	height: 40px;
        margin-left: 10px;
        padding: 2px;
	}

	.fakeNav{
		height: 75px;
	}

	.navBar{
		position: fixed;
		top: 0;
		width: 100%;
		z-index: 1000;
		height: 75px;
	}

    .bg-nav{
		background-color:  #2E303E;
	}

	.token{
		height: 36px;
		margin-top: 4px;
	}

	.navBtn:hover, .btnGo:hover {
		border-width: 2px !important;
	}



</style>
    
