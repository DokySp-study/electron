<template>
    <v-app>
        <v-app-bar app>
            <v-toolbar-title class="headline text-uppercase">
                <span>일렉트론 </span>
                <span class="font-weight-light">APP</span>
            </v-toolbar-title>
            <v-spacer></v-spacer>

            <v-btn v-on:click="chgView(0)" text>
                HOME
            </v-btn>
            &nbsp;
            <v-btn v-on:click="chgView(1)" text>
                TEST
            </v-btn>
            &nbsp;

            <v-btn text href="https://github.com/vuetifyjs/vuetify/releases/latest" target="_blank">
                <v-icon>mdi-anchor</v-icon> &nbsp;
                <!-- v-icon: https://vuetifyjs.com/ko/components/icons -->
                <!-- icon forge: https://material.io/resources/icons/?icon=attachment&style=baseline -->
                <span class="mr-1">최신 릴리즈</span>
            </v-btn>
        </v-app-bar>
    
        <v-content>
            <Test v-show="count == 1"></Test>
            <HelloWorld v-show="count == 0"/>
        </v-content>
    </v-app>
</template>

<script>
    import HelloWorld from './components/HelloWorld';
    import Test from './components/Test'
    
    export default {
        name: 'App',
        components: {
            HelloWorld,
            Test,
        },
        methods: {
            chgView: function(input){
                this.count = input
                console.log(this.count + "/" + input)
            }
        },  
        data: () => ({
            count: 0,
        }),
    };
</script>
