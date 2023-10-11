<script>
export default{
    data(){
        return{
            obs:0,
            slides:[
            "https://images.getbento.com/accounts/22022076ca31682d32e6a3253b8e9e7c/media/images/70222220826_FedPig_B1_Traditional4_0401.jpg?w=1200&fit=crop&auto=compress,format&crop=focalpoint&fp-x=0.5&fp-y=0.5",
            "https://images.getbento.com/accounts/22022076ca31682d32e6a3253b8e9e7c/media/images/67494IMG_2648.JPG?w=1200&fit=crop&auto=compress,format&crop=focalpoint&fp-x=0.44&fp-y=0.66",
            "https://images.getbento.com/accounts/22022076ca31682d32e6a3253b8e9e7c/media/images/41145federalist-pig-home-pattern-black.jpg?w=1200&fit=crop&auto=compress,format&crop=focalpoint&fp-x=0.5&fp-y=0.5",
            "https://images.getbento.com/accounts/22022076ca31682d32e6a3253b8e9e7c/media/images/6865220826_FedPig_A3_FavTraditional_0110.jpg?w=1200&fit=crop&auto=compress,format&crop=focalpoint&fp-x=0.48&fp-y=0.98",
            "https://images.getbento.com/accounts/22022076ca31682d32e6a3253b8e9e7c/media/images/95907IMG_6837.JPG?w=1200&fit=crop&auto=compress,format&crop=focalpoint&fp-x=0.5&fp-y=0.5",
            ]
        };
    },
    methods: {
        primaImg(){
            this.obs = 0
        },
        secondaImg(){
             this.obs = 1
        },
        terzaImg(){
             this.obs = 2
        },
        quartaImg(){
             this.obs = 3
        },
        quintaImg(){
             this.obs = 4
        },
    }
}

</script>

<template>
    <div class="carousel">
        <div class="carousel-image" v-for="(slide, i) in slides" :key="slide">
            <img v-if="i == obs" :src="slides[i]" >
        </div>
    </div>
    <div class="carousel-button">
        <div class="button1" :class="obs == 0 ? 'btn-active' : ''" @click="primaImg"></div>
        <div class="button2" :class="obs == 1 ? 'btn-active' : ''" @click="secondaImg"></div>
        <div class="button3" :class="obs == 2 ? 'btn-active' : ''" @click="terzaImg"></div>
        <div class="button4" :class="obs == 3 ? 'btn-active' : ''" @click="quartaImg"></div>
        <div class="button5" :class="obs == 4 ? 'btn-active' : ''" @click="quintaImg"></div>
    
    </div>
</template>

<style scoped>
.carousel{
    
}
.carousel-image{
    
}
.carousel-image img{
    width: 100%;
    
}
.carousel-button{
    gap: 13px;
    display: flex;
    background-color: #ffd700;
    padding: 17px;
    max-width: 350px;
    margin: 10px;
    align-items: center;
    justify-content: center;
    border-top-left-radius: 20px;
    border-top-right-radius: 20px;
}
.button1, .button2, .button3, .button4, .button5{
    width: 13px;
    height: 13px;
    border-radius: 50%;
    background-color: black;
    opacity: .65;
}
.button1:hover, .button2:hover, .button3:hover, .button4:hover, .button5:hover{
    opacity: 1;
}
.btn-active{
    opacity: 1;
}
</style>