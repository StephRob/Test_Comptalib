<template>
  <section :class="[isActive ? 'is-flex-direction-row' : 'is-flex-direction-row-reverse']" class="container restaurant-card px-2 is-flex is-align-items-center">
    <div class="px-2">
      <h1 class="title is-2">Le Madelaine C</h1>
      <p class="subtitle is-4">
        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Quasi
        consequuntur harum similique provident doloremque laborum, quae eaque.
        Dolore eos labore vel dolorem provident non eveniet debitis, vitae
        placeat saepe ipsa.
      </p>
      <p class="subtitle is-4">5 Rue de Castellane, 75008 Paris</p>
      <div class="buttons">
        <a href="https://www.google.com/maps/dir//Restaurant+Le+Madeleine+C.,+5+Rue+de+Castellane,+75008+Paris/@48.872241,2.2902034,13z/data=!3m1!4b1!4m9!4m8!1m0!1m5!1m1!1s0x47e66e349a458473:0x5b59a471293769d8!2m2!1d2.3252285!2d48.8721988!3e2"
          target="_blank">
          <b-button type="is-info is-light mr-4">
            <strong>Voir sur la carte</strong>
          </b-button>
        </a>
        <b-button type="is-light" @click="toggleClass" class="is-hidden-mobile">
            <strong>Switcher la position de l'image</strong>
          </b-button>
      </div>
    </div>
    <div class="px-2 is-hidden-mobile">
      <b-image
        src="https://www.lemadeleinec.fr/i/le-madeleine-c-418566/3/4/8/9/6/5/1/5/0/4/3/9/2/1540217519_260/347028c51056e5123cfc8b205482643c.clandscape_hd.jpg">
      </b-image>
    </div>

  </section>
</template>

<script>
  export default {
    name: "Card",
    data: () => ({
      isActive: true,
    }),
    
    methods: {
        toggleClass() {
        this.isActive = !this.isActive;
      }
    }
  };
</script>

<style>
  .restaurant-card {
    height: calc(100vh - 96px);
    flex-direction: row;
  }

</style>