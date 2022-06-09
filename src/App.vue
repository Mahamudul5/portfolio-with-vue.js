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
            <v-subheader>I am Mahamudul hasan. I am a frontend developer ,work with react.js, vue.js ,vuetify ,tailwind
              etc.</v-subheader>
            <br />
            <br />
            <v-btn large elevation="5" color="green" class="white--text mt-10 px-10 py-5">Hire me</v-btn>
            <v-btn large elevation="5" color="green" class="white--text mt-10 ml-10 px-10 py-5">contact me</v-btn>
            <v-row class="mt-16">
              <v-chip class="px-4 ma-3" color="success">
                <v-icon left size="20">mdi-whatsapp</v-icon>
                what's app
              </v-chip>
              <v-chip class="px-4 ma-3" color="success">
                <v-icon left size="20">mdi-github</v-icon>
                github
              </v-chip>
              <v-chip class="px-4 ma-3" color="success">
                <v-icon left size="20">mdi-linkedin</v-icon>
                linkedIn
              </v-chip>
              <v-chip class="px-4 ma-3" color="success">
                <v-icon left size="20">mdi-facebook</v-icon>
                facebook
              </v-chip>
            </v-row>
          </v-col>
          <v-col lg="6" cols="6">
            <v-img src="../public/images/myProfileR.png"></v-img>
          </v-col>
        </v-row>
      </v-section>
      <v-section class="about-me" id="about">
        <v-img class="pa-10" height="400" gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
          src="../public/images/officePhoto.jpg">
          <v-row justify="center" class="align-center">
            <v-col lg="6" cols="6">
              <v-card class="text-center pa-6 rounded-lg" color="#e1e0e0c9" elevation="6">
                <v-card-subtitle class="green--text ">ABOUT MYSELF</v-card-subtitle>
                <h2 class="display-1 font-weight-regular">I am frontend web developer. I already complete some projects.
                  I am working with react.js, vue.js, tailwind, vuetify etc.</h2>

                <v-btn large elevation="5" color="green" class="white--text mt-10 px-10 py-5">Download Resume
                  <v-icon>mdi-download</v-icon>
                </v-btn>
              </v-card>
            </v-col>
            <v-col lg="6" cols="6">
              <v-card class="pa-6 rounded-lg" color="#e1e0e0c9" elevation="6">
                <div class="py-1" v-for="(item, index) in items" :key="index">
                  <label>{{ item.title }}</label>
                  <v-progress-linear :color="item.color" height="10" :value="item.value">

                  </v-progress-linear>

                </div>

              </v-card>
            </v-col>


          </v-row>

        </v-img>

      </v-section>


    </v-main>

  </v-app>


</template>

<script>
export default {
  name: 'App',
  data: () => ({
    drawer: null,
    items: [
      { title: 'HTML', value: 100, color: 'light-blue' },
      { title: 'CSS', value: 85, color: 'deep-orange' },
      { title: 'JAVASCRIPT', value: 70, color: 'light-green' },
      { title: 'VUE.JS', value: 80, color: 'blue' },
      { title: 'VUETIFY', value: 65, color: 'black' },
      { title: 'REACT.JS', value: 90, color: 'red' },
      { title: 'TAILWIND', value: 90, color: 'yellow' },
    ]

  }),
};
</script>
