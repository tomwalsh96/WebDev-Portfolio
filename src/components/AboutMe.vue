<template>
  <v-row
    justify="center"
    align="start"
    style="width: 100vw; margin-top:40vh;  background-color: #6C63FF;"
  >
    <v-col
      cols="12"
    >
      <v-row
        justify="center"
        style="margin-top: -24vh;"
      >
        <v-img
          src="../assets/bio.png"
          height="250"
          contain
        ></v-img>
      </v-row>
      <v-container
        class="my-10"
      >
        <v-row
          justify="center"
          class="mb-3"
        >
          <h1
            style="color: white;"
            class="text-center display-2 font-weight-medium"
          >
            About Me
          </h1>
        </v-row>
        <v-row
          justify="center"
        >
          <h4
            style="color: white;"
            class="text-center mx-12"
          >
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
          </h4>
        </v-row>
      </v-container>
      <v-row
        justify="center"
        class="d-none d-md-flex"
      >
        <v-card
          width="70vw"
          outlined
          tile
          style="border-radius: 20px 20px 0 0; border: solid 2px #000;"
        >
          <v-col>
            <v-row>
               <v-col
                  cols="6"
                >
                  <v-row
                    class="fill-height"
                    justify="center"
                    style="border-right: solid 2px #000;"
                  >
                    <v-col
                      cols="8"
                    >
                      <v-row
                        justify="center"
                      >
                        <img
                          src="../assets/logo.png"
                          width="100"
                          class="mt-3"
                        >
                      </v-row>
                      <v-row
                        justify="center"
                      >
                        <h1
                          class="text-center display-2 font-weight-medium mt-10"
                        >
                          Designer
                        </h1>
                      </v-row>
                      <v-row
                        justify="center"
                      >
                        <p
                          class="text-center mt-5"
                        >
                          {{ designer.blurb }}
                        </p>
                      </v-row>
                      <v-row
                        justify="center"
                      >
                        <h1
                          style="color: #6C63FF;"
                          class="text-center display-1 font-weight-medium mt-12"
                        >
                          Platforms:
                        </h1>
                      </v-row>
                      <v-row
                        justify="center"
                      >
                        <p
                          class="text-center mt-3"
                        >
                          <span
                            v-for="(item, index) in designer.platforms" :key="index"
                          >
                            {{ item }}
                            <br>
                          </span>
                        </p>
                      </v-row>
                      <v-row
                        justify="center"
                      >
                        <h1
                          style="color: #6C63FF;"
                          class="text-center display-1 font-weight-medium mt-12"
                        >
                          Resources:
                        </h1>
                      </v-row>
                      <v-row
                        justify="center"
                      >
                        <p
                          class="text-center mt-3"
                        >
                          <span
                            v-for="(item, index) in designer.resources" :key="index"
                          >
                            {{ item }}
                            <br>
                          </span>
                        </p>
                      </v-row>
                    </v-col>
                  </v-row>
                </v-col>
                <v-col
                  cols="6"
                >
                  <v-row
                    class="fill-height"
                    justify="center"
                  >
                    <v-col
                      cols="8"
                    >
                      <v-row
                        justify="center"
                      >
                        <img
                          src="../assets/logo.png"
                          width="100"
                          class="mt-3"
                        >
                      </v-row>
                      <v-row
                        justify="center"
                      >
                        <h1
                          class="text-center display-2 font-weight-medium mt-10"
                        >
                          Developer
                        </h1>
                      </v-row>
                      <v-row
                        justify="center"
                      >
                        <p
                          class="text-center mt-5"
                        >
                          {{ developer.blurb }}
                        </p>
                      </v-row>
                      <v-row
                        justify="center"
                      >
                        <h1
                          style="color: #6C63FF;"
                          class="text-center display-1 font-weight-medium mt-12"
                        >
                          Languages:
                        </h1>
                      </v-row>
                      <v-row
                        justify="center"
                      >
                        <p
                          class="text-center mt-3"
                        >
                          <span
                            v-for="(item, index) in developer.languages" :key="index"
                          >
                            {{ item }}
                            <br>
                          </span>
                        </p>
                      </v-row>
                      <v-row
                        justify="center"
                      >
                        <h1
                          style="color: #6C63FF;"
                          class="text-center display-1 font-weight-medium mt-12"
                        >
                          Tools:
                        </h1>
                      </v-row>
                      <v-row
                        justify="center"
                      >
                        <p
                          class="text-center mt-3"
                        >
                          <span
                            v-for="(item, index) in developer.tools" :key="index"
                          >
                            {{ item }}
                            <br>
                          </span>
                        </p>
                      </v-row>
                    </v-col>
                  </v-row>
                </v-col>
            </v-row>
          </v-col>
        </v-card>
      </v-row>
      <v-row
        justify="center"
        class="d-flex d-md-none"
      >
        <v-card
          width="70vw"
          outlined
          tile
          style="border-radius: 20px 20px 0 0; border: solid 2px #000;"
        >
          <v-col>
            <v-row>
               <v-col
                  cols="12"
                >
                  <v-row
                    class="fill-height"
                    justify="center"
                  >
                    <v-col
                      cols="8"
                    >
                      <v-row
                        justify="center"
                      >
                        <img
                          src="../assets/logo.png"
                          width="100"
                          class="mt-3"
                        >
                      </v-row>
                      <v-row
                        justify="center"
                      >
                        <h1
                          class="text-center display-2 font-weight-medium mt-10"
                        >
                          Designer
                        </h1>
                      </v-row>
                      <v-row
                        justify="center"
                      >
                        <p
                          class="text-center mt-5"
                        >
                          {{ designer.blurb }}
                        </p>
                      </v-row>
                      <v-row
                        justify="center"
                      >
                        <h1
                          style="color: #6C63FF;"
                          class="text-center display-1 font-weight-medium mt-12"
                        >
                          Platforms:
                        </h1>
                      </v-row>
                      <v-row
                        justify="center"
                      >
                        <p
                          class="text-center mt-3"
                        >
                          <span
                            v-for="(item, index) in designer.platforms" :key="index"
                          >
                            {{ item }}
                            <br>
                          </span>
                        </p>
                      </v-row>
                      <v-row
                        justify="center"
                      >
                        <h1
                          style="color: #6C63FF;"
                          class="text-center display-1 font-weight-medium mt-12"
                        >
                          Resources:
                        </h1>
                      </v-row>
                      <v-row
                        justify="center"
                      >
                        <p
                          class="text-center mt-3"
                        >
                          <span
                            v-for="(item, index) in designer.resources" :key="index"
                          >
                            {{ item }}
                            <br>
                          </span>
                        </p>
                      </v-row>
                    </v-col>
                  </v-row>
                </v-col>
                <v-col
                  cols="12"
                >
                  <v-row
                    class="fill-height"
                    justify="center"
                    style="border-top: solid 2px #000; padding-top: 20px;"
                  >
                    <v-col
                      cols="8"
                    >
                      <v-row
                        justify="center"
                      >
                        <img
                          src="../assets/logo.png"
                          width="100"
                          class="mt-3"
                        >
                      </v-row>
                      <v-row
                        justify="center"
                      >
                        <h1
                          class="text-center display-2 font-weight-medium mt-10"
                        >
                          Developer
                        </h1>
                      </v-row>
                      <v-row
                        justify="center"
                      >
                        <p
                          class="text-center mt-5"
                        >
                          {{ developer.blurb }}
                        </p>
                      </v-row>
                      <v-row
                        justify="center"
                      >
                        <h1
                          style="color: #6C63FF;"
                          class="text-center display-1 font-weight-medium mt-12"
                        >
                          Languages:
                        </h1>
                      </v-row>
                      <v-row
                        justify="center"
                      >
                        <p
                          class="text-center mt-3"
                        >
                          <span
                            v-for="(item, index) in developer.languages" :key="index"
                          >
                            {{ item }}
                            <br>
                          </span>
                        </p>
                      </v-row>
                      <v-row
                        justify="center"
                      >
                        <h1
                          style="color: #6C63FF;"
                          class="text-center display-1 font-weight-medium mt-12"
                        >
                          Tools:
                        </h1>
                      </v-row>
                      <v-row
                        justify="center"
                      >
                        <p
                          class="text-center mt-3"
                        >
                          <span
                            v-for="(item, index) in developer.tools" :key="index"
                          >
                            {{ item }}
                            <br>
                          </span>
                        </p>
                      </v-row>
                    </v-col>
                  </v-row>
                </v-col>
            </v-row>
          </v-col>
        </v-card>
      </v-row>
      <v-row
        style="height: 60vh; min-height: 400px; width: 100vw; margin-top:-300px;  background-color: white;"
      >
      </v-row>
    </v-col>
  </v-row>
</template>

<script>

export default {
  name: 'AboutMe',
  data: () => ({
    designer: {
      blurb: `Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. 
        Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. 
        Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.`,
      platforms: ['Figma'],
      resources: ['colorsinspo.com', 'fontfabric.com', 'logomoose.com', 'endlessicons.com', 'unsplash.com',
        'reallygoodemails.com', 'freedesignresources.net', 'graphicburger.com', 'background.bg', 'compressor.io']
    },
    developer: {
      blurb: `Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. 
              Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. 
              Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.`,
      languages: ['HTML', 'CSS', 'Javascript', 'Python'],
      tools: ['VS Code', 'GitHub', 'Vue', 'Vuetify']
    }
  })
}
</script>
