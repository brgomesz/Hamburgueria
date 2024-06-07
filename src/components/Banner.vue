<template>
    <div id="main-banner">
<h2>Faça seu hamburguer</h2>

    </div>

</template>

<script>
export default {
    name: "Banner"

}
</script>

<style scoped>
#main-banner{
    background-image: url('/public/img/burguer.jpg');
    background-position: 0 -250px;
    background-size: cover;
    height: 400px;
    display: flex;
    align-items: center;
    justify-content: flex-start;
    margin-bottom: 80px;
    
   
}

#main-banner h2{
    color:#fff;
    text-align: center;
    font-size: 60px; 
    background-color: #222222a2;
    padding: 20px 40px;
}



</style>