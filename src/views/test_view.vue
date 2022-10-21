<template>
    <button @click="showz"> ok </button>
    <div class="row w-90 mx-auto">
        <mfComp v-for="x in json.array"
            :key="x"
            :name="x.main.name"
            :img="x.main.img"
            :wiki="x.main.wiki"
            
            :name1="x.one.name"
            :img1="x.one.img"
            :amount1="x.one.amount"
            :wiki1="x.one.wiki"

            :name2="x.two.name"
            :img2="x.two.img"
            :amount2="x.two.amount"
            :wiki2="x.two.wiki"

            :name3="x.three.name"
            :img3="x.three.img"
            :amount3="x.three.amount"
            :wiki3="x.three.wiki"

            :name4="x.four.name"
            :img4="x.four.img"
            :amount4="x.four.amount"
            :wiki4="x.four.wiki"
        >
        </mfComp>
    </div>
</template>

<script>
/*
import display_component from '../components/display_component.vue'
*/

import jsonData from '../assets/test.json'
import mfComp from '../components/mf_upgrade_component.vue'

export default {
    name: 'test_view',
    data(){
        return{
            json: jsonData
        }
    },
    methods:{
        showz(){
            console.log("SHOWZ");
            console.log(this.json.array);
            console.log(this.json.array.length);
            /*
            for(var x = 0; x < jsonData.lenght; x++){
                console.log("obj" + x );
                for(var y = 0; y < jsonData[x][y].length ; y++){
                    console.log(jsonData[x][y]);
                }
            }
            */
        }
    },
	components:{
		mfComp
	}
}
</script>

<style scoped>

</style>