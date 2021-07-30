<template>
    <div class="cardshop " >
        <img :src="image" width="100%" height="auto">
        <div class="row my-3">
            <div class="col-6 text-center">
                <div class="cardshop-name">{{name}}</div>
                <div class="cardshop-price">{{price}} ฿</div> 
            </div>
            <div class="col-6 my-auto">
                <b-button class="cardshop-button">ADD TO CART</b-button>
            </div>
        </div>   
    </div>
</template>

<script>
export default {
    props:{
        id: {
            type: Number,
            default: 0
        },
        name: {
            type: String,
            default: ''
        },
        price: {
            type: Number,
            default: 0
        },
        image: {
            type: String,
            default: ''
        }
    }
}
</script>

<style scoped>
    .cardshop {
    transition: 0.3s;
    }

    .cardshop:hover {
    transform: scale(1.03);
    }
   .cardshop{
       background-color: rgb(253, 251, 249);
       padding: 15px;
       border-radius: 3px;
   }
   
   .cardshop-name{
       font-size: 23px;
       font-weight: bold;
   }
   .cardshop-price{
       font-size: 20px;
   }
   .cardshop-button{
       background-color: black;
       border-radius: 3px;
       padding: 10px;
   }
   
</style>