<script>
export default {
    data() {
        return {
            shop: {
                uomo: 'Uomo',
                donna: 'Donna',
                bambino: 'Bambino'
            }


        }
    }
}

</script>


<template>
    <header class="background-header">
        <nav class="container ">
            <div class="container-header">
                <div class="shop-header">
                    <a v-for="(shops, i) in shop" href="#">{{ shops }}</a>

                </div>
                <a href=""> <img style="width: 100px;" src="/img/boolean-logo.png" alt=""></a>
                <div>Shop</div>

            </div>

        </nav>
    </header>
</template>
<style lang="scss" scoped>
@use '../style/partials/header';
</style>
