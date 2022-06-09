<template>
  <v-app id="inspire">
    <v-app-bar app elevation="0">
      <v-subheader>
        <h1 class="green--text">mahamudul.h</h1>
      </v-subheader>
      <v-tabs center-active right background-color="transparent" active-class="active-tab">
        <v-tab href="#home">Home</v-tab>
        <v-tab>About</v-tab>
        <v-tab>Blog</v-tab>
        <v-tab>projects</v-tab>
        <v-tab>contact</v-tab>

      </v-tabs>
      <v-btn large color="green" class="white--text ml-10">Fire me an Email</v-btn>
    </v-app-bar>
    <v-main style="background-color:#F5F5F5">
      <v-section class="intro-section" id="home">
        <v-row class="align-center px-10" style="height:690px">
          <v-col lg="6" cols="6" class="pa-6 font-weight-bold py-16">
            <h2 class="display-3 green--text">Frontend Web Developer.</h2>

          </v-col>

        </v-row>

      </v-section>

    </v-main>

  </v-app>


</template>

<script>
export default {
  name: 'App',
  data: () => ({
    //
  }),
};
</script>
