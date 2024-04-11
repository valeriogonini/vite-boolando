<template>
    <div class="col-1">
        <div class="foto">
            <img :src="`/img/${item.frontImage}`" alt="">

            <span v-for="(badge, i) in item.badges" :key="i"
                :class="badge.type === 'discount' ? 'sconto' : 'sostenibilita'">
                {{ badge.value }}</span>



            <span class="cuore">&hearts;</span>
            <div class="overlay">
                <img :src="`/img/${item.backImage}`" alt="">
                <span class="cuore-red">&hearts;</span>
            </div>
        </div>
        <p>{{ item.brand }}</p>
        <h3>{{ item.name }}</h3>
        <span class="soldi-sconto">14,99$</span>
        <span class="textdecoretion">{{ item.price }}</span>
    </div>
</template>

<script>
export default {
    props: {
        item: {
            type: Object
        }
    }
}
</script>

<style lang="scss" scoped></style>