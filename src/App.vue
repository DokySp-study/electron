<template>
  <v-app>
    <v-app-bar app>
      <v-toolbar-title class="headline text-uppercase">
        <span>ELECTRON </span>
        <span class="font-weight-light">TEST APP</span>
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn text href="https://github.com/vuetifyjs/vuetify/releases/latest" target="_blank">
        <v-icon>mdi-anchor</v-icon> &nbsp;
        <!-- v-icon: https://vuetifyjs.com/ko/components/icons -->
        <!-- icon forge: https://material.io/resources/icons/?icon=attachment&style=baseline -->
        <span class="mr-2">최신 릴리즈</span>
      </v-btn>
    </v-app-bar>
  
    <v-content>
      <HelloWorld/>
    </v-content>
  </v-app>
</template>

<script>
  import HelloWorld from './components/HelloWorld';
  
  export default {
    name: 'App',
    components: {
      HelloWorld,
    },
    data: () => ({
      //
    }),
  };
</script>
