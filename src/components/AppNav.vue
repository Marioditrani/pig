<script>

</script>

<template>
    <div class="header">
        <div class="logo">
            <span class="logo-up">federalist</span>
            <span class="logo-down">pig</span>
        </div>
        <ul class="nav">
            <li class="menu"><strong>menu</strong></li>
            <li class="catering"><strong>catering</strong></li>
            <li class="locations"><strong>locations</strong></li>
            <li class="bbq-box"><strong>bbq box</strong></li>
            <li class="supper-club"><strong>supper club</strong></li>
            <li class="gift-cards"><strong>gift cards</strong></li>
            <li class="orders-online"><strong>orders online</strong></li>
        </ul>
    </div>
</template>

<style scoped>
*{
    text-transform: uppercase;
}
.header{
    background-color: #ffd700;
    display: flex;
    justify-content: space-between;
    align-items: center;
}
.logo{
   display: flex;
   flex-direction: column;
   font-size: 45px;
   padding: 5px 30px;
   
}

.nav{
    padding: 0px 30px;
    height: 100%;
    display: flex;
    gap: 20px;
    font-size: 16px;
}

.menu, .catering, .locations, .bbq-box, .supper-club, .gift-cards, .orders-online{
    padding: 7px 5px;
}
.menu:hover, .catering:hover, .locations:hover, .bbq-box:hover, .supper-club:hover, .gift-cards:hover{
    background-color: black;
    color: #ffd700;
    padding: 7px 5px;
    transition: all  linear 0.2s ;
    
}
.orders-online{
    border: 2px solid black;
    padding: 5px 10px;
}
.orders-online:hover{
    padding: 5px 10px;
    background-color: black;
    color: #ffd700;
    transition: all  linear 0.2s ;
}
</style>