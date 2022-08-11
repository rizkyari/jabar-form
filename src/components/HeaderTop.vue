<template>
    <header>
        <div class="header-left">
            <img class="logo-img" src="../assets/logo_jds.png"/>
        </div>
            <div class="header-right">
                <ul class="menu-right">
                    <li>Layanan</li>
                    <li>Harga</li>
                    <li>Artikel</li>
                </ul>
            </div>
    </header>
</template>

<script>
</script>

<style scoped>
header{
    display: flex; 
    justify-content: space-between;
    align-items: center;
}

.logo-img{
    width: 30%;
    height: 30%;
}

.menu-right{
    display: flex;
    list-style-type: none;
}

li{
    margin: 0 10px;
    cursor: pointer;
}

</style>
