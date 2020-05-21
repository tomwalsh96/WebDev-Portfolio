<template>
  <v-app-bar
    app
    absolute
    clipped-left
    flat
    color="white"
    style="height: 10vh;"
  >
    <v-toolbar-title
      class="
      font-weight-black
      display-1
      ml-2
      ml-sm-12
      mt-8
      "
    >
      <img
        src="../assets/logo.png"
        width="100"
      >
    </v-toolbar-title>
    <v-toolbar-title
      class="
      font-weight-black
      display-1
      ml-10
      mt-8
      d-none
      d-sm-flex
      "
    >
      Tom Walsh
    </v-toolbar-title>
    <v-spacer></v-spacer>
    <v-btn
      color="#6C63FF"
      dark
      class="
      mr-2
      mr-sm-12
      mt-8
      "
    >
      Contact
    </v-btn>
  </v-app-bar>
</template>

<script>
export default {
  name: 'AppBar',
  data: () => ({
  })
}
</script>
