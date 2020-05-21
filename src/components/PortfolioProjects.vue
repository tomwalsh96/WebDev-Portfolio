<template>
  <v-row
    justify="center"
    align="center"
    style="min-height: 100vh; width: 100vw; background-color: #6C63FF;"
  >
    <v-col
      cols="12"
    >
      <v-row
        justify="center"
        class="mt-7"
      >
        <h1
          style="color: white;"
          class="display-3 font-weight-medium mt-3"
        >
          Portfolio
        </h1>
      </v-row>
      <v-row
        justify="center"
      >
        <h4
          style="color: white;"
          class="mx-12"
        >
          This is a collection of my most recent projects.
        </h4>
      </v-row>
      <v-row
        justify="center"
      >
        <v-container
          class="mt-5 mx-0"
        >
          <v-row
          justify="center"
          >
            <v-hover
              v-for="n in this.projects"
              :key="n"
              v-slot:default="{ hover }"
              open-delay="200"
            >
              <v-card
                class="ma-4"
                width="360"
                height="200"
                :img="n.src"
                :elevation="hover ? 16 : 2"
                style="border-radius: 20px;"
              >
                <v-overlay
                  :absolute="true"
                  :opacity="0.5"
                  :value="hover"
                  z-index="0"
                >
                  <v-container>
                  <v-row
                    justify="center"
                    align="center"
                  >
                    <p>{{ n.hovertext }}</p>
                  </v-row>
                  <v-row
                    justify="center"
                    align="center"
                  >
                    <v-btn
                      color="orange lighten-2"
                      @click="overlay = false"
                    >
                      Visit website
                    </v-btn>
                  </v-row>
                  </v-container>
                </v-overlay>
              </v-card>
            </v-hover>
          </v-row>
        </v-container>
      </v-row>
      <v-row
        justify="center"
        class="mt-5 mb-7"
      >
        <v-btn
          large
        >
          See more
        </v-btn>
      </v-row>
    </v-col>
  </v-row>
</template>

<script>

export default {
  name: 'PortfolioProjects',
  data: () => ({
    overlay: false,
    projects: [
      { src: 'https://cdn.vuetifyjs.com/images/parallax/material.jpg', hovertext: 'hello 1' },
      { src: 'https://cdn.vuetifyjs.com/images/parallax/material.jpg', hovertext: 'hello 2' },
      { src: 'https://cdn.vuetifyjs.com/images/parallax/material.jpg', hovertext: 'hello' },
      { src: 'https://cdn.vuetifyjs.com/images/parallax/material.jpg', hovertext: 'hello' },
      { src: 'https://cdn.vuetifyjs.com/images/parallax/material.jpg', hovertext: 'hello' },
      { src: 'https://cdn.vuetifyjs.com/images/parallax/material.jpg', hovertext: 'hello' }
    ]
  })
}
</script>
