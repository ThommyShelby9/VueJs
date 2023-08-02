<script lang="ts" setup>
import mobile from '@/components/icons/mobile.vue'
import credit from '@/components/credit.vue'
import { ref } from 'vue'

const paiement = ref([
   {
    methods: ''
   }
])

function paiementMethod(){
    const findIndex= paiement.value.findIndex((item) => (item.methods='mobile'))

}
</script>


<template>
     <div class="banner_content_select" v-for="element in paiement" >
        <div class="banner_content_select_item">
            <div class="banner_content_select_item_img" @click="paiementMethod()">
                <mobile/> 
            </div>
            <div class="banner_content_select_item_text">
                <p>Paiement Mobile</p>
            </div>
        </div>
        <div class="banner_content_select_item">
            <div class="banner_content_select_item_img" @click="paiementMethod()">
                <credit/>
            </div>
            <div class="banner_content_select_item_text">
                <p>Carte de crédit</p>
            </div>
        </div>

        <div v-if="element.methods = 'mobile'">
            <h1>Pas encore disponible</h1>
        </div>
    </div>
    
</template>

<style>

.banner{
    display: flex;
    flex-direction: column;
    text-align: center;
    padding: 1px 20px;
    font-size: 15px;
    background-color: rgb(212, 181, 146);
}

.banner_content_select{
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    gap: 10px;
}

.banner_content_select_item{
    display: flex;
    flex-direction: column;
    text-align: center;
    align-items: center;
}

.banner_content_select_item_img{
    border: 1px solid rgb(255, 1, 1);
    width: 50px;
    height: 30px;
    padding-top: 6px;
    color: red;
}

.banner_content_select_item_img:hover{
    background-color: red;
    color: white;
    cursor: pointer;
}

.banner_content_select_item_text{
    font-size: 10px;
}
</style>