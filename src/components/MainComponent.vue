<script>

import ComponentCard from './ComponentCard.vue';


export default {
  components: {
    ComponentCard
  },
  data() {
    return {
      products: [
        {
          id: 1,
          frontImage: "1.webp",
          backImage: "1b.webp",
          brand: "Levi's",
          name: "Relaxed Fit",
          price: 29.99,
          isInFavorites: true,
          badges: [
            {
              type: "tag",
              value: "Sostenibilità"
            },
            {
              type: "discount",
              value: "-50%"
            }
          ]
        },
        {
          id: 2,
          frontImage: "2.webp",
          backImage: "2b.webp",
          brand: "Guess",
          name: "Roses Tee",
          price: 20.99,
          isInFavorites: true,
          badges: [
            {
              type: "discount",
              value: "-30%"
            }
          ]
        },
        {
          id: 3,
          frontImage: "3.webp",
          backImage: "3b.webp",
          brand: "Come Zucchero Filato",
          name: "Voglia di colori pastello",
          price: 129.99,
          isInFavorites: false,
          badges: [
            {
              type: "discount",
              value: "-30%"
            }
          ]
        },
        {
          id: 4,
          frontImage: "4.webp",
          backImage: "4b.webp",
          brand: "Levi's",
          name: "Tee Unisex",
          price: 14.99,
          isInFavorites: false,
          badges: [
            {
              type: "tag",
              value: "Sostenibilità"
            },
            {
              type: "discount",
              value: "-50%"
            }
          ]
        },
        {
          id: 5,
          frontImage: "5.webp",
          backImage: "5b.webp",
          brand: "Maya Deluxe",
          name: "Stripe Bodice",
          price: 99.99,
          isInFavorites: true,
          badges: [
            {
              type: "tag",
              value: "Sostenibilità"
            },
            {
              type: "discount",
              value: "-50%"
            }
          ]
        },
        {
          id: 6,
          frontImage: "6.webp",
          backImage: "6b.webp",
          brand: "Esprit",
          name: "Maglione - Black",
          price: 29.99,
          isInFavorites: true,
          badges: [
            {
              type: "tag",
              value: "Sostenibilità"
            }
          ]
        }
      ]


    }
  }
}

</script>

<template>
  <main>
    <section>
      <div class="container">
        <div class="row">

          <ComponentCard v-for="(product, i) in products" :item="product" :key="product.id" />
          <!-- <div class="col-1">
            <div class="foto">
              <img src="/img/1.webp" alt="">
              <span class="sconto">30%</span>
              <span class="sostenibilita">Sostenibilita</span>
              <span class="cuore">&hearts;</span>
              <div class="overlay">
                <img src="/img/1b.webp" alt="">
                <span class="cuore-red">&hearts;</span>
              </div>
            </div>
            <p>Levi's</p>
            <h3>RELAXED FIT TEE UNISEX</h3>
            <span class="soldi-sconto">14,99$</span>
            <span class="textdecoretion"> 29,99$</span>
          </div> -->
          <!-- <div class="col-1">
            <div class="foto">
              <img src="/img/2.webp" alt="">
              <span class="sconto">30%</span>
              <span class="cuore">&hearts;</span>
              <div class="overlay">
                <img src="/img/2b.webp" alt="">
                <span class="cuore-red">&hearts;</span>

              </div>
            </div>
            <p>Levi's</p>
            <h3>RELAXED FIT TEE UNISEX</h3>
            <span class="soldi-sconto">14,99$</span>
            <span class="textdecoretion"> 29,99$</span>
          </div>
          <div class="col-1">
            <div class="foto">
              <img src="/img/3.webp" alt="">
              <span class="sconto">30%</span>
              <span class="cuore">&hearts;</span>
              <div class="overlay">
                <img src="/img/3b.webp" alt="">
                <span class="cuore-red">&hearts;</span>

              </div>
            </div>
            <p>Levi's</p>
            <h3>RELAXED FIT TEE UNISEX</h3>
            <span class="soldi-sconto">14,99$</span>
            <span class="textdecoretion"> 29,99$</span>
          </div>
          <div class="col-1">
            <div class="foto">
              <img src="/img/4.webp" alt="">
              <span class="sconto">30%</span>
              <span class="sostenibilita">Sostenibilita</span>
              <span class="cuore">&hearts;</span>
              <div class="overlay">
                <img src="/img/4b.webp" alt="">
                <span class="cuore-red">&hearts;</span>

              </div>
            </div>
            <p>Levi's</p>
            <h3>RELAXED FIT TEE UNISEX</h3>
            <span class="soldi-sconto">14,99$</span>
            <span class="textdecoretion"> 29,99$</span>
          </div>
          <div class="col-1">
            <div class="foto">
              <img src="/img/5.webp" alt="">

              <span class="cuore">&hearts;</span>
              <div class="overlay">
                <img src="/img/5b.webp" alt="">
                <span class="cuore-red">&hearts;</span>

              </div>
            </div>
            <p>Levi's</p>
            <h3>RELAXED FIT TEE UNISEX</h3>
            <span class="soldi-sconto">14,99$</span>
            <span class="textdecoretion"> 29,99$</span>
          </div>
          <div class="col-1">
            <div class="foto">
              <img src="/img/6.webp" alt="">
              <span class="sostenibilita-only">Sostenibilita</span>
              <span class="cuore">&hearts;</span>
              <div class="overlay">
                <img src="/img/6b.webp" alt="">
                <span class="cuore-red">&hearts;</span>

              </div>
            </div>
            <p>Levi's</p>
            <h3>RELAXED FIT TEE UNISEX</h3>
            <span class="soldi-sconto">14,99$</span>
            <span class="textdecoretion"> 29,99$</span>
          </div> -->


        </div>
      </div>
    </section>
    <section>
      <div class="container">
        <div class="row">

        </div>
      </div>
    </section>
  </main>
</template>

<style lang="scss" scoped>
@use '../style/partials/main';
</style>
