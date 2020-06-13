<script>
    let qnt = 1;

    const minusQty = () => {
        if (qnt > 1) {
            qnt--;
        }
    }
</script>


<li class="product_block">
    <div class="product_image"></div>
    <div class="product">
        <div class="product_info">
            <div class="product_info_top">
                <h4 class="product_title">Vegetarian Pizza</h4>
                <p>$9.25</p>
            </div>
            <div class="product_excerpt">
                green pasta, tomato sauce, milk, eggs, green papper
            </div>
            <div class="product_rate">
                <img src="images/star.png" alt="Rating">5.0
                <span class="rate_line">|</span>
                <span class="product_weight">250g</span>
            </div>
            <div class="product_bottom">
                <div class="product_quantity">
                    <button on:click={minusQty}>-</button>
                    <input type="number" value={qnt} class="product_qnt">
                    <button on:click={() => qnt++}>+</button>
                </div>
                <div class="add_to_cart">Add to cart</div>
            </div>
        </div>
    </div>
</li>

<style>
    .product_block{
        position: relative;
    }
    .product{
        max-width: 90%;
        width: 100%;
        border-radius: 20px;
        box-shadow: 4px 3px 15px #00000026;
        display: flex;
        justify-content: space-between;
        margin-bottom: 30px;
        margin-left: auto;
    }
    .product_image{
        width: 140px;
        height: 140px;
        border-radius: 20px;
        background-image: url(/images/pizza.jpg);
        background-position: center;
        background-size: cover;
        position: absolute;
        left: 0;
        top: -15px;
    }
    .product_info{
        flex-basis: calc(100% - 135px);
        padding: 15px 15px 15px 0;
        margin-left: auto;
    }
    .product_info_top{
        display: flex;
        justify-content: space-between;
        align-items: center;
        font-size: 14px;
        margin-bottom: 15px;
    }
    .product_info_top p{
        font-weight: bold;
        color: #80cb4b;
    }
    .product_excerpt{
        font-size: 12px;
    }
    .product_rate{
        padding: 12px 0;
        font-size: 12px;
        line-height: 15px;
    }
    .product_rate img{
        width: 9px;
        margin-right: 5px;
    }
    .rate_line{
        margin: 0 2px;
    }
    .product_bottom{
        display: flex;
        justify-content: space-between;
    }
    .product_qnt{
        border: 1px solid #80cb4b;
        border-radius: 5px;
        background-color: transparent;
        max-width: 15px;
        text-align: center;
        height: 17px;
    }
    .product_quantity{
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
    .product_quantity button{
        border-radius: 50%;
        background-color: #80cb4b;
        color: #ffffff;
        border: none;
        width: 15px;
        height: 15px;
        display: flex;
        justify-content: center;
        align-items: center;
    }
    .product_quantity input{
        margin: 0 5px;
    }
    .add_to_cart{
        background-color: #80cb4b;
        color: #ffffff;
        box-shadow: 3px 4px 8px #80cb4b;
        border-radius: 50px;
        padding: 0 20px;
        font-size: 13px;
        display: flex;
        justify-content: center;
        align-items: center;
    }
    @media all and (max-width: 360px) {
        .add_to_cart{
            padding: 0 10px;
            font-size: 10px;
        }
        .product_info_top{
            margin-bottom: 5px;
        }
        .product_image {
            top: 50%;
            transform: translateY(-50%);
        }
    }
</style>