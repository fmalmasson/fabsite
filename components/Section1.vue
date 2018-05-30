<template>
  <div>
    <section>
      <v-parallax src="hero.jpeg" height="400">
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
      <v-layout
        column
        wrap
        class="my-5"
        align-center>
        <v-flex xs12 sm4 class="my-3">
          <div class="text-xs-center">
            <h2 class="headline">Compétences</h2>
          </div>
        </v-flex>

        <v-flex xs12>
          <v-container grid-list-xl>
            <v-layout row wrap justify-center>

              <v-flex xs12 md4>
                <v-card class="elevation-0 transparent">
                  <v-card-text class="text-xs-center">
                    <v-icon x-large class="blue--text text--lighten-2">code</v-icon>
                  </v-card-text>
                  <v-card-title primary-title class="layout justify-center">
                    <div class="headline">Langages, frameworks et librairies</div>
                  </v-card-title>
                  <v-card-text>
                    <span class="body-2">Langages :</span><span class="body-1" v-for="language in languages">  {{ language }}  </span></br>
                    </br><span class="body-2">Frameworks: </span><span v-for="framework in frameworks"> {{ framework }}  </span></br>
                    </br><span class="body-2">Librairies: </span><span v-for="library in librairies"> {{ library }}  </span></br>
                    </br><span class="body-2">Versionning: </span><span v-for="versionning in Versionnings"> {{ versionning }}  </span>
                  </v-card-text>
                </v-card>
              </v-flex>

              <v-flex xs12 md4>
                <v-card class="elevation-0 transparent">
                  <v-card-text class="text-xs-center">
                    <v-icon x-large class="blue--text text--lighten-2">face</v-icon>
                  </v-card-text>
                  <v-card-title primary-title class="layout justify-center">
                    <div class="headline text-xs-center">soft-skills</div>
                  </v-card-title>
                  <v-card-text>
  Je suis quelqu'un de fiable et honnête qui n'hésite jamais à se remettre en question afin de progresser. D'humeur constante, je suis autant à l'aise à l'oral qu'à l'écrit. J'aime les challenges, résoudre des problèmes, être intellectuellement sollicité. Mes diverses expériences, tant professionnelles qu'humaines m'ont permis de développer mon ouverture d'esprit, mon sens des priorités et ma flexibilité. De nature autonome, j'aime le travail en équipe quand il est bien fait.                </v-card-text>
                </v-card>
              </v-flex>
            </v-layout>
          </v-container>
        </v-flex>
      </v-layout>
    </section>
  </div>

</template>

<script>
export default {
}
</script>
