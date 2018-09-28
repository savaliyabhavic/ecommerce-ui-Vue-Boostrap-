<template>

        <div class="container">
            <div class="page-header jumbotron"><h1>Products</h1></div>
           <div class="row">
               <div class="col-md-3 product-grid card card-hover" v-for="item in productItems" v-bind:key="item.id">
                   <div class="card-body">
                    <h5 class="card-title">{{item.name}}</h5>
                    <p class="card-text">{{item.descrption}}</p>
                    <p>Available Qty: {{item.qty}}</p>
                    <p>Price: {{item.price}} Rs.</p>
                    <button class="btn btn-primary" @click="addToCart(item)">ADD TO CART</button>
                   </div>
               </div>
           </div>
        </div>


</template>

<script>
export default {
    name: 'Products',
    data() {
        return{
            productItems: [
                    {
                        "id": 1,
                        "name": "Dell Vostro",
                        "descrption": "Laptos lalalall balla bla",
                        "qty": 3,
                        "price": 35000,
                        "category": 1,
                        "cid": 1,
                        "cname": "Electronics"
                    },
                    {
                        "id": 2,
                        "name": "Shoool Beg",
                        "descrption": "begs las las bla",
                        "qty": 2,
                        "price": 760,
                        "category": 2,
                        "cid": 2,
                        "cname": "Men"
                    },
                    {
                        "id": 3,
                        "name": "testing",
                        "descrption": "las las bla",
                        "qty": 5,
                        "price": 600,
                        "category": 1,
                        "cid": 4,
                        "cname": "wev"
                    },
                    {
                        "id": 4,
                        "name": "testing",
                        "descrption": "las las bla",
                        "qty": 5,
                        "price": 600,
                        "category": 1,
                        "cid": 4,
                        "cname": "wev"
                    },
                    {
                        "id": 4,
                        "name": "testing",
                        "descrption": "las las bla",
                        "qty": 5,
                        "price": 600,
                        "category": 1,
                        "cid": 4,
                        "cname": "wev"
                    },
                    {
                        "id": 4,
                        "name": "testing",
                        "descrption": "las las bla",
                        "qty": 5,
                        "price": 600,
                        "category": 1,
                        "cid": 4,
                        "cname": "wev"
                    },
                    {
                        "id": 4,
                        "name": "testing",
                        "descrption": "las las bla",
                        "qty": 5,
                        "price": 600,
                        "category": 1,
                        "cid": 4,
                        "cname": "wev"
                    },
                    {
                        "id": 4,
                        "name": "testing",
                        "descrption": "las las bla",
                        "qty": 5,
                        "price": 600,
                        "category": 1,
                        "cid": 4,
                        "cname": "wev"
                    },
                    {
                        "id": 4,
                        "name": "testing",
                        "descrption": "las las bla",
                        "qty": 5,
                        "price": 600,
                        "category": 1,
                        "cid": 4,
                        "cname": "wev"
                    },
                    {
                        "id": 4,
                        "name": "testing",
                        "descrption": "las las bla",
                        "qty": 5,
                        "price": 600,
                        "category": 1,
                        "cid": 4,
                        "cname": "wev"
                    },
                    {
                        "id": 4,
                        "name": "testing",
                        "descrption": "las las bla",
                        "qty": 5,
                        "price": 600,
                        "category": 1,
                        "cid": 4,
                        "cname": "wev"
                    }
                ]
        }
    },
    created(){
        //Make a network Call,
        //Response,
        //this.productItems 

        ///Start the loader
    },
    methods: {
        addToCart(item){
            console.log(item);
        }
    }
}
</script>

<style>


.product-grid{
    border: 1px solid black;
    margin-bottom: 10px;
    padding: 10px;
    height: 300px;
}

.card-hover:hover{
    background: whitesmoke;
}

</style>
