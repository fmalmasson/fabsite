<template lang="html">
  <div id="formation">
    <section>
      <div class="parallax2">
        <v-container text-xs-center fill-height>
          <v-layout row wrap align-center>
            <v-flex class="white--text" xs12 justify-center>
              <span class="name">Formation</span>
            </v-flex>
          </v-layout>
        </v-container>
      </div>

      <v-container grid-list-xl class="fullContainer">
        <v-layout  wrap justify-center class="">
          <v-flex xs6>
            <v-card class="elevation-0 transparent">
              <v-card-title primary-title class="layout justify-center">
                <div class="headline pink--text" v-scroll-reveal.reset="{ viewFactor: 0.2 }">IMIE Nantes, Bac +2</div>

              </v-card-title>
              <v-card-text v-scroll-reveal.reset="{ viewFactor: 0.4 }">
                <strong v-scroll-reveal.reset="{ viewFactor: 0.2 }"class="headline">Développeur Logiciel</strong>
              </br></br>
                Titre de niveau 3 réalisé en 9 mois dont 3 mois de stage.
                <p>J'ai choisi cette formation car l'IMIE proposait des cours et un stage qui, de mon point de vue, allait être le tremplin idéal pour ma reconversion.
                  La formation a débuté par 6 mois de cours où j'ai appris les bases indispensables du développement.
                  J'ai travaillé sur les technologies suivantes : </br> <strong>HTML & CSS, PHP, SYMPHONY, MYSQL, JAVASCRIPT, NODEJS, JQUERY, MONGODB ...</strong></br></br>
                  J'ai ensuite intégré l'agence digitale Léo by Antares pour un <strong>stage de 3 mois</strong> en tant que développeur front-end.
                </p>
              </v-card-text>
            </v-card>
          </v-flex>
          <v-flex xs6>
          </v-flex>
          <v-flex xs6 offset-xs6>
            <v-card class="elevation-0 transparent">
              <v-card-title primary-title class="layout justify-center">
                <div class="headline pink--text" v-scroll-reveal.reset="{ viewFactor: 0.2 }">Inseec Bordeaux, Bac +4</div>
              </v-card-title>
              <v-card-text v-scroll-reveal.reset="{ viewFactor: 0.4 }">
                <strong class="headline">Bachelor in Business Administration</strong></br></br>
                Cursus international, 15 mois de stages en entreprise
                <p>Je suis extrêmement content d'avoir réalisé ce parcours à vocation internationale qui a grandement construit la personne que je suis devenue.
                Au delà de m'avoir apporté des connaissances techniques en Marketing, Finance et <strong>Management</strong>, l'Inseec m'a permis de m'ouvrir sur le monde, sur les personnes, et m'a fait rencontré des amis pour la vie.
               J'ai eu la chance d'aller étudier <strong>un semestre académique à Hong-Kong</strong>, un mois à la Fac en <strong>Espagne</strong>, de réaliser un stage à <strong>Londres</strong> et deux stages à Paris. </p>
              </v-card-text>
            </v-card>
          </v-flex>
        </v-layout>
      </v-container>
    </section>
</div>
</template>

<script>
export default {
  name: 'section2',
  data: () => ({
    skills:
    [
      {
        name: 'HTML'
      },
      {
        name: 'CSS'
      },
      {
        name: 'Javascript'
      },
      {
        name: 'PHP'
      },
      {
        name: 'Versioning'
      },
      {
        name: 'DevTools'
      },
      {
        name: 'Command Line'
      }
    ]
  })
}
</script>

<style scoped lang="css">
.fullContainer {
  height: 100vh;
}
.formation {
  margin-top: -50px;
  background-color: white;
}
.title {
  font-size: 65px !important;
  font-weight: 700 !important;
}
.parallax2 {
  height: 80vh;
  background-image: url("/static/macpro.jpg");

  /* Create the parallax scrolling effect */
    background-attachment: fixed;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
}
section {
  height: 100vh;
}

</style>
