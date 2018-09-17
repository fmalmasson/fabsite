<template lang="html">
  <div id="xp-pro">
    <section>
      <v-container class="xpContainer" text-xs-center>
        <v-layout row wrap justify-center>
          <v-flex xs12 class="xpElements">
            <v-card class="elevation-0 transparent">
              <v-card-title primary-title class="" style="justify-content: center;">
                <div class="headline pink--text">Développeur Full Stack</div>
              </v-card-title>
              <v-card-text>
                <span class="about">I'm currently working as a full stack developer at Antares, in Nantes.</span>
                <!-- <v-layout fill-height row wrap text-xs-center align-center>
                  <v-flex xs3>
                    <v-avatar
                      tile="false"
                      size="100px"
                      color="white"
                    >
                    <img src="html.png" alt="avatar">
                    </v-avatar>
                  </v-flex>
                  <v-flex>
                    <v-avatar
                      tile="false"
                      size="100px"
                      color="white"
                    >
                    <img src="css.png" alt="avatar">
                    </v-avatar>
                  </v-flex>
                  <v-flex>
                    <v-avatar
                      tile="false"
                      size="100px"
                      color="white"
                    >
                    <img src="vuejs.jpg" alt="avatar">
                    </v-avatar>
                  </v-flex>
                  <v-flex>
                    <v-avatar
                      tile="false"
                      size="100px"
                      color="white"
                    >
                    <img src="laravel.png" alt="avatar">
                    </v-avatar>
                  </v-flex>

                </v-layout> -->
              </v-card-text>
            </v-card>
          </v-flex>
          <!-- <v-flex xs12 sm4 offset-sm1>
            <v-card class="elevation-0 transparent">
              <v-card-title primary-title class="layout justify-center">
                <div class="headline">Dans une autre vie...</div>
              </v-card-title>
              <v-list three-line>
                <template v-for="job in jobs">
                  <v-list-tile>
                    <v-list-tile-content v-if="job.show" @click="job.show = !job.show">
                      <v-list-tile-title v-html="job.headline"></v-list-tile-title>
                      <v-list-tile-sub-title>{{ job.company }}</v-list-tile-sub-title>
                      <v-list-tile-sub-title class="skills">Compétences : {{ skillsList(job) }}</v-list-tile-sub-title>
                    </v-list-tile-content>
                    <v-list-tile-content v-else @click="job.show = !job.show" @mouseleave="job.show = !job.show">
                      <v-list-tile-title v-html="job.headline"></v-list-tile-title>
                      <v-list-tile-sub-title v-html="job.resume"></v-list-tile-sub-title>
                    </v-list-tile-content>
                  </v-list-tile>
                </template>
              </v-list>
            </v-card>
          </v-flex> -->
        </v-layout>
      </v-container>
    </section>
</div>
</template>

<script>
export default {
  name: 'section2',
  data: () => ({
    jobs: [
      {
        company: 'BPA accelerator',
        src: 'bpa.jpg',
        headline: 'Consultant Startups',
        time: 'mai 2015 à septembre 2015',
        type: 'CDI',
        comp: 'Business Plan',
        show: true,
        resume: 'Après leur rencontre, nous faisions pour le compte de jeunes startups ayant déjà fait une levée de fonds, leurs Business Plan et Plan de financement afin de les aider dans l\'obtention de subventions publiques et/ou privées permettant le financement de leur projet innovant.',
        skills: ['Ecoute', 'Analyse', 'esprit de synthèse']
      },
      {
        company: 'MACIF',
        src: 'macif.gif',
        headline: 'Directeur d\'agence',
        time: 'avril 2011 à décembre 2013',
        type: 'CDI',
        comp: 'Management',
        show: true,
        resume: 'Manager d\'une agence de 6 conseillers commerciaux, ma mission était d\'organiser et planifier l\'activité, former les collaborateurs, et commercialiser les produits du groupe Macif.',
        skills: ['Management', 'Sens de la diplomatie', 'pédagogie']
      },
      {
        company: 'MACIF',
        src: 'macif.gif',
        headline: 'Cadre technique',
        time: 'septembre 2010 à avril 2011',
        type: 'CDI',
        comp: 'Management',
        show: true,
        resume: 'Sur un call-center de 80 personnes, je m\'occupais de la régulation des flux téléphoniques, aide aux téléconseillers pour les dossiers techniques ou demandant des dérogations.',
        skills: ['Analyse de risque', 'rapidité de réflexion', 'connaisance de l\'assurance']
      },
      {
        company: 'MACIF',
        src: 'macif.gif',
        headline: 'Téléconseiller',
        time: 'mai 2009 à septembre 2010',
        type: 'CDI',
        comp: 'Management',
        show: true,
        resume: 'Commercialisation par téléphone des produits du groupe Macif après une formation interne au monde de l\'assurance',
        skills: ['Ecoute', 'compréhension du besoin', 'communication orale', 'tenacité']
      },
      {
        company: 'Ambassade de France en Mongolie',
        src: 'macif.gif',
        headline: 'Attaché comptable',
        time: 'août 2007 à août 2008',
        type: 'Volontariat International en Administration',
        comp: 'Management',
        show: true,
        resume: 'Attaché comptable de l\'Ambassade de France de la Mongolie, j\'étais en charge de la réalisation des budgets et de la comptabilité.',
        skills: ['forte adaptibilité', 'autonomie', 'ouverture d\'esprit']
      }
    ]
  }),
  methods: {
    skillsList (job) {
      return job.skills.join(' - ')
    }
  }
}
</script>

<style lang="css">
.about {
  color: #666666;
}
.application.theme--light {
  background-color: white;
}
#xp-pro {
  height: 80vh;
  margin-bottom: 0px;
}

.xpContainer {
  margin-top: 10px;
  padding-bottom: 0px;
  margin-bottom: -10px;
}
.skillsCard {
  z-index: 10;
  margin-top: 0px;
}
.logos {
  height: 150px;
}
.xpElements {
  margin-top: 187px;
}
</style>
