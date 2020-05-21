<template>
  <v-row
    justify="center"
    style="width: 100vw;  background-color: #6C63FF;"
  >
    <v-col
      cols="12"
    >
      <v-row
        justify="center"
      >
        <v-col>
          <v-row
            justify="center"
          >
            <img
              src="../assets/logo-white.png"
              alt="Logo"
              width="100"
            >
          </v-row>
          <v-row
            justify="center"
            class="my-10 mx-7"
          >
            <h1
              style="color: white;"
              class="display-1 font-weight-medium text-center"
            >
              “To move a mountain, start by moving stones”
            </h1>
          </v-row>
          <v-row
            justify="center"
            class="my-10"
          >
            <v-btn
              fab
              text
              elevation="3"
              large
              class="mx-5"
              style="border: solid 3px white;"
            >
              <img
                src="../assets/linkedin.png"
                alt="Linkedin"
                width="30"
              >
            </v-btn>
            <v-btn
              fab
              text
              elevation="3"
              large
              dark
              class="mx-5"
              style="border: solid 3px white;"
            >
              <img
                src="../assets/github.png"
                alt="GitHub"
                width="40"
              >
            </v-btn>
            <v-btn
              fab
              text
              elevation="3"
              large
              class="mx-5"
              style="border: solid 3px white;"
            >
              <img
                src="../assets/email.png"
                alt="Linkedin"
                width="30"
              >
            </v-btn>
          </v-row>
        </v-col>
      </v-row>
    </v-col>
  </v-row>
</template>

<script>

export default {
  name: 'Footer'
}
</script>
