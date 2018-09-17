<template>

  <div style="position:relative; z-index:10">
    <div class="parallax" v-scroll="onScroll">
      <v-toolbar fixed id="toolbar" color="white" height="50px" v-if="toolbarDisplay">
        <v-avatar
          tile="false"
          size="50px"
          color="white"
        >
        <img src="fm.png" alt="avatar">
        </v-avatar>
        <v-spacer></v-spacer>
        <v-toolbar-items class="hidden-sm-and-down">
          <v-btn flat>Expérience Pro</v-btn>
          <v-btn flat>Formation</v-btn>
          <v-btn flat>Contact</v-btn>
        </v-toolbar-items>
      </v-toolbar>
      <v-container text-xs-center fill-height>
        <v-layout row wrap align-center>
          <v-flex class="white--text" xs12 justify-center>
            <span class="hello" v-scroll-reveal.reset="{ delay: 0 }">Hello :)</span><span v-scroll-reveal.reset="{ delay: 1100 }"> my name is</span></br>
            <span class="name" v-scroll-reveal.reset="{ delay: 1500 }">Fabien MALMASSON</span>
          </br>
          </br>
          <span class="whoAmI" v-scroll-reveal.reset="{ delay: 2500 }">I'm a Full Stack DEVELOPER @ </span><span class="pink--text whoAmI" v-scroll-reveal.reset="{ delay: 2500 }">Antares</span>

          </v-flex>
        </v-layout>
      </v-container>
    </div>
  </div>

</template>

<script>
export default {
  data: () => ({
    toolbarDisplay: false,
    color: 'white',
    textColorClass: 'white--text',
    languages: '[ HTML, JS, CSS, PHP, SQL ]',
    frameworks: '[ Vuejs, Laravel, Vuetify, Quasar, Element ]',
    BDD: '[ PostgreSQL, MySQL ]',
    librairies: '[ Webpack, Lodash, Babel ]',
    Versionnings: '[ Git, Bitbucket ]'
  }),
  computed: {
  },
  methods: {
    onScroll () {
      if (window.pageYOffset <= 50) {
        this.toolbarDisplay = false
      } else {
        this.toolbarDisplay = true
      }
    }
  }
}
</script>
<style lang="css">
.name {
  font-size: 65px;
  font-weight: 700;
}
.hello {
  font-size: 25px;
}
.whoAmI {
  font-weight: 400;
  font-size: 18px;
}
.parallax {
  height: 100vh;
  background-image: url("/static/orion.jpg");

  /* Create the parallax scrolling effect */
    background-attachment: fixed;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
}

.skills {
  font-size: '30px';
}

.theme--light .toolbar {
  z-index: 10;
  background-color: transparent;
}
</style>
