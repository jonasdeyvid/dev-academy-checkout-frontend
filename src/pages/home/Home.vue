<template>
    <div class="home">
        <home-product-list class="product-list" />
        <home-payment-summary class="payment-summary" />
        <div class="link">
            <a href="/crudProduct">Cadastre um produto</a>
        </div>
    </div>
    
</template>

<script>
import HomeProductList from "./components/HomeProductList";
import HomePaymentSummary from "./components/HomePaymentSummary";

export default {
    name: "Home",
    components: {
        HomeProductList,
        HomePaymentSummary
    }
};
</script>

<style lang="stylus">
.home
    width 100%

.link
    position absolute
    top 120%
    left 0%

@media screen and (min-width: 950px)
    .home
        display flex
        position absolute
        top 50%
        left 50%
        transform translate(-50%, -50%)

    .product-list
        margin-right  2%

@media screen and (min-width: 1300px)
    .home
        display flex
        width 80%
        position absolute
        top 50%
        left 50%
        transform translate(-50%, -50%)

</style>
