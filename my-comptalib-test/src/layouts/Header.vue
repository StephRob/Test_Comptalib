<template>
  <header>
    <b-navbar class="container">
      <template #brand>
        <b-navbar-item fixed-top tag="router-link" :to="{ path: '/' }">
          <img src="../assets/logo_comptalib.svg" alt="logo Comptalib" />
          <span class="logo-text blue">Lunch</span>
        </b-navbar-item>
      </template>

      <template #end>
        <b-navbar-item tag="div">
          <div class="buttons">
            <g-link to="/Restaurant">
              <b-button type="is-info is-light">
                <strong>Voir le restaurant</strong>
              </b-button>
            </g-link>
          </div>
        </b-navbar-item>
      </template>
    </b-navbar>
  </header>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style scoped>
.logo-text {
  font-size: 27px;
  font-style: italic;
}

.blue,
.background-blue {
  color: #1854f2;
}
</style>