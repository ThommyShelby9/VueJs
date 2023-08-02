<template>
     <div class="main_content_top">
            <label for="name">Nom et Prénoms</label> <br>
            <input type="text" id="name" required>
     </div>
        <div class="main_content_bottom">
            <label for="number">Numéro de téléphone</label> <br>
            <input type="number" id="number">
        </div>
</template>

<style>

.main_content{
    display: flex;
    flex-direction: column;
    gap: 10px;
    padding: 15px 20px;
}

#name, #number{
    width: 90%;
    padding: 10px;
    border: 1px solid rgba(104, 104, 104, 0.315);
}
</style>