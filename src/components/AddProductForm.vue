<template>
    <div class="productform">
        <div class="productFormView container">
            <h5 class="card-title jumbotron">Add new Product</h5>
            <div class="row">   
                <div class="col-sm-3"></div> 
                <div class="col-sm-6">
                    <form class="formview">
                        <div class="form-group">
                            <label for="forProductName">{{title}} Product Name</label>
                            <input placeholder="Enter Product Name" v-model="name" class="linespace form-control" name="productName" type="text">
                        </div>

                        <div class="form-group">
                            <label for="forDesc">{{title}} Description</label>
                            <textarea placeholder="Enter Product Description" v-model="desc"  name="productDescription" class="form-control" rows="3"></textarea>
                        </div>

                        <div class="form-group">
                            <label for="forQty">Total Quantity</label>
                            <input v-model="qty" number class="form-control" name="productQty" type="number">                
                        </div>

                        <div class="form-group">
                            <label for="forPrice">Price</label>
                            <input v-model="price" number name="productPrice" class="form-control" type="number">                
                        </div>

                        <div class="form-group">
                            <select class="custom-select form-control">
                                <option selected disabled>Select product category</option>
                                <option value="1">Electronics</option>
                                <option value="2">Men</option>
                                <option value="3">FootWear</option>
                                <option value="4">Furniture</option>
                                <option value="5">Study</option>
                            </select>
                        </div>
                        
                        <button class="btn btn-primary form-control" v-on:click="submit" type="submit">Submit</button>
                    </form>
                </div>

                <div class="col-sm-3"></div>

            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'AddProductForm',
    data(){
        return {
            title:'Product',
            name: '',
            desc: '',
            qty: 0,
            price: 0,
            selected: 0,
        }
    },
    methods : {
        submit (){
                alert(this.price);
            }
    }
}
</script>

<style>
.productFormView{
    margin-bottom: 40px;
}
</style>

