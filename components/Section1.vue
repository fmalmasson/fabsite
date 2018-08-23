<template>
  <div>
    <section>
      <v-parallax src="sbc.jpg" height="400">
        <v-layout
          column
          align-center
          justify-center
          class="white--text">
          <h2 class="mb-2 display-3">Développeur Full-Stack</h2>
          <em class="intro">
          </em>
        </v-layout>
      </v-parallax>
    </section>

    <section>
      <v-container fluid>
      <v-layout
        column
        wrap
        class="my-5"
        align-center>
        <v-flex xs12 md8>
            <h2 class="headline" :style="{color: '#50ac91'}">Skills</h2>
        </v-flex>

              <v-flex xs12 md12>
                <v-card class="elevation-0 transparent">
                  <v-card-text >
                    <span class="skills">Vue.js + Laravel</span>
                    <!-- <span class="">Langages :</span><span class="">  {{ languages }}  </span></br>
                  </br><span class="">Frameworks: </span><span> {{ frameworks }}  </span></br>
                </br><span class="">Librairies: </span><span> {{ librairies }}  </span></br>
              </br><span class="">Versionning: </span><span> {{ Versionnings }}  </span> -->
                  </v-card-text>
                </v-card>
              </v-flex>

              <!-- <v-flex xs12 md4>
                <v-card class="elevation-0 transparent">
                  <v-card-text class="text-xs-center">
                    <v-icon x-large class="blue--text text--lighten-2">face</v-icon>
                  </v-card-text>
                  <v-card-title primary-title class="layout justify-center">
                    <h3>soft-skills</h3>
                  </v-card-title>
                  <v-card-text>
  Je suis quelqu'un de fiable et honnête qui n'hésite jamais à se remettre en question afin de progresser. D'humeur constante, je suis autant à l'aise à l'oral qu'à l'écrit. J'aime les challenges, résoudre des problèmes, être intellectuellement sollicité. Mes diverses expériences, tant professionnelles qu'humaines m'ont permis de développer mon ouverture d'esprit, mon sens des priorités et ma flexibilité. De nature autonome, j'aime le travail en équipe quand il est bien fait.                </v-card-text>
                </v-card>
              </v-flex> -->
      </v-layout>
    </v-container>
    </section>
  </div>

</template>

<script>
export default {
  data: () => ({
    languages: '[ HTML, JS, CSS, PHP, SQL ]',
    frameworks: '[ Vuejs, Laravel, Vuetify, Quasar, Element ]',
    BDD: '[ PostgreSQL, MySQL ]',
    librairies: '[ Webpack, Lodash, Babel ]',
    Versionnings: '[ Git, Bitbucket ]'
  }),
  computed: {
    color () {
      return '#50ac91'
    }
  }
}
</script>
<style>
.skills {
  font-size: '30px';
}
</style>
