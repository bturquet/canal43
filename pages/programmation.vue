<template>
  <v-layout column justify-center align-center>
    <v-flex xs12 sm8 md6>
          <div
        id="e3"
        style="max-width: 600px; margin: auto;"
        class="grey lighten-3"
      >
        <v-toolbar
          color="primary"
          dark
        >
          <v-toolbar-title>Programmation</v-toolbar-title>
        </v-toolbar>
        <v-card color="black">
          <v-container
            fluid
            grid-list-lg
          >
            <v-layout row wrap>

              <v-flex xs12>
                <v-card color="blue-grey darken-2" class="white--text">
                  <v-card-title primary-title>
                    <div class="headline">Unlimited music now</div>
                    <div>Listen to your favorite artists and albums whenever and wherever, online and offline.</div>
                  </v-card-title>
                  <v-card-actions>
                    <v-btn flat dark>PLUS D'INFOS</v-btn>
                  </v-card-actions>
                </v-card>
              </v-flex>

              <v-flex xs12>
                <v-card color="cyan darken-2" class="white--text">
                  <v-layout>
                    <v-flex xs5>
                      <v-img
                        src="https://cdn.vuetifyjs.com/images/cards/foster.jpg"
                        height="125px"
                        contain
                      ></v-img>
                    </v-flex>
                    <v-flex xs7>
                      <v-card-title primary-title>
                        <div>
                          <div class="headline">ARTISTE 1</div>
                          <div>Présentation</div>
                          <div>(date)</div>
                        </div>
                      </v-card-title>
                    </v-flex>
                  </v-layout>
                  <v-divider light></v-divider>
                  <v-card-actions>
                    <v-btn flat dark>PLUS D'INFOS</v-btn>
                  </v-card-actions>
                </v-card>
              </v-flex>

              <v-flex xs12>
                <v-card color="purple" class="white--text">
                  <v-layout row>
                    <v-flex xs7>
                      <v-card-title primary-title>
                        <div>
                          <div class="headline">ARTISTE 2</div>
                          <div>Présentation</div>
                          <div>(date)</div>
                        </div>
                      </v-card-title>
                    </v-flex>
                    <v-flex xs5>
                      <v-img
                        src="https://cdn.vuetifyjs.com/images/cards/halcyon.png"
                        height="125px"
                        contain
                      ></v-img>
                    </v-flex>
                  </v-layout>
                  <v-divider light></v-divider>
                  <v-card-actions>
                    <v-btn flat dark>PLUS D'INFOS</v-btn>
                  </v-card-actions>
                </v-card>
              </v-flex>

            </v-layout>
          </v-container>
        </v-card>
      </div>
    </v-flex>
  </v-layout>
</template>
