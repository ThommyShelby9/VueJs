<script setup lang="ts">
import Input from '@/components/icons/input.vue'
import paiement from '@/components/icons/paiment.vue'
import eader from '@/components/icons/header.vue'
</script>

<template>
    <div class="wrapper">
        <div class="container">
            <header class="header">
              <eader/> 
            </header>
            <main class="main">
                <section class="banner">
                    <div class="banner_content">
                        <p>Sélectionner un mode de paiement</p>
                        <paiement/>
                    </div>
                </section>
                <div class="main_content">
                   <Input/>
                </div>
                <button class="payer">Payer 12 000 Fcfa</button>
            </main>
        </div>
    </div>
</template>

<style scoped>
.wrapper{
    display: flex;
    flex-direction: column;
    margin:auto;
}

.container{
    margin: 60px auto; 
    padding-bottom: 20px;
    box-shadow: 1px 1px 1px 1px;
}

.payer{
    width: 86%;
    padding: 10px;
    margin-left: 15px;
    background-color: red;
    font-weight: 800;
    color: white;
    border: none;
    cursor: pointer;
}

.container.active{
    display: none;
}
</style>
