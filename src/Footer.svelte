<script>

</script>

<footer>
    <ul class="footer_menu">
        <li class="active">
            <img src="images/footer/menu.png" alt="Menu">
            <p>Menu</p>
        </li>
        <li>
            <img src="images/footer/gift.png" alt="Gift">
            <p>Discounts</p>
        </li>
        <li>
            <img src="images/footer/cart.png" alt="Cart">
            <p>Cart</p>
        </li>
        <li>
            <img src="images/footer/order.png" alt="My order">
            <p>My order</p>
        </li>
        <li>
            <img src="images/footer/more.png" alt="More">
            <p>More</p>
        </li>
    </ul>
</footer>

<style>
    footer{
        position: fixed;
        bottom: 0;
        left: 0;
        width: 100%;
        padding: 10px 0 20px;
        box-shadow: 1px 3px 6px #000;
        background-color: #fff;
    }
    .footer_menu{
        display: flex;
        justify-content: space-between;
        list-style: none;
        margin: 0;
        padding: 0;
    }
    .footer_menu li{
        flex-basis: 20%;
        text-align: center;
    }
    .footer_menu li img{
        width: auto;
        height: 25px;
    }
    .footer_menu li p{
        font-size: 12px;
        color: #000000;
        margin: 0;
    }
    .footer_menu li.active p{
        color: #80cb4b;
    }
</style>