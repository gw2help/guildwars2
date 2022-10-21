<template>

    <wingz></wingz>

</template>

<script>
import wingz from '../components/wingz_component.vue'
import json from '../assets/gw2_progression_data.json'

export default 
  {
    name: 'progress_view',
    data(){
        return{
            result: ""
        }
    },
    components: { 
        wingz
    },
    methods: {
		
    }
}
</script>

<style scoped>


</style>