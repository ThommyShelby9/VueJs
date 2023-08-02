<script lang="ts" setup>
import panier from '@/components/icons/panier.vue'
</script>

<template>
     <div class="header_content">
        <div class="header_content_logo">
            <panier/>
        </div>
        <div class="header_content_total">
            <p>Total à payer</p>
        </div>
        <div class="header_content_total_price">
            <h3>12 000 <span>Fcfa</span></h3> 
        </div>
    </div>
</template>

<style>

.header{
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
    width: 200px;
    background-color: red;
    line-height: 10px;
    padding: 20px 70px 1px;
    color: white;
}

.header_content{
    padding-bottom: -30px;
}

.header_content_logo{
    padding-top: 30px;
}

.header_content_total{
    font-size: 15px;
}

.header_content_total_price{
    font-size: 25px;
}

.header_content_total_price span{
    font-weight: 100;
}


</style>