<template>
  <Layout>
    <section class="container hero is-flex-direction-row px-2">
      <div class="hero-body is-flex pl-2 pr-0 is-flex-direction-column is-justify-content-center">
        <h1 class="title">Comptalib Lunch</h1>
        <p class="subtitle">
          L'outil qui propose un restaurant différent chaque jour pour la team
          Comptalib
        </p>
        <div class="buttons">
          <g-link to="/Restaurant">
            <b-button type="is-info is-light is-medium">
              <strong>Découvrez le restaurant du jour</strong>
            </b-button>
          </g-link>
        </div>
      </div>
      <div class="hero-body is-flex is-justify-content-center is-align-items-center is-hidden-mobile">
        <iframe src="https://embed.lottiefiles.com/animation/4762"></iframe>
      </div>
    </section>
  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: 'Comptlib Lunch'
  }
}
</script>

<style>
.title,
.subtitle {
  font-size: 42px;
  color: #29426f;
}

.hero {
  height: calc(100vh - 96px);
}

.hero-body {
  width: 50%;
}

iframe {
  width: 450px;
  height: 450px;
}
</style>
