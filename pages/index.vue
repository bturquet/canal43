<template>
  <v-layout column justify-center align-center>
    <v-flex xs12 sm8 md6>
      <div class="text-xs-center">
        <iframe width="620" height="315"
          src="https://www.youtube.com/embed/dBNKhHGQTk0">
        </iframe>
      </div>
      <v-jumbotron>
        <v-container fill-height>
          <v-layout align-center>
            <v-flex>
              <h3 class="display-3">CENTRAL43</h3>

              <span class="subheading">Le rendez-vous musical du Champ de Mars - Lille, les 14 et 15 décembre 2018.</span>

              <v-divider class="my-3"></v-divider>

              <div class="title mb-3">Plus d'infos !</div>

              <v-btn
                class="mx-0"
                color="primary"
                large
                nuxt to="/infos"
              >
                PLUS
              </v-btn>
            </v-flex>
          </v-layout>
        </v-container>
      </v-jumbotron>
    </v-flex>
  </v-layout>
</template>
