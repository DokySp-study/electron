<template>
    <v-app>
        <v-app-bar app>
            <v-toolbar-title class="headline text-uppercase">
                <span>ELECTRON </span>
                <span class="font-weight-light">TEST</span>
            </v-toolbar-title>
            <v-spacer></v-spacer>
            <v-btn text href="https://github.com/vuetifyjs/vuetify/releases/latest" target="_blank">
                <span class="mr-2">홈</span>
            </v-btn>
            &nbsp;
            <v-btn text href="https://github.com/vuetifyjs/vuetify/releases/latest" target="_blank">
                <span class="mr-2">테스트</span>
            </v-btn>
            &nbsp;
            <v-btn text href="https://github.com/vuetifyjs/vuetify/releases/latest" target="_blank">
                <span class="mr-2">릴리즈</span>
            </v-btn>
        </v-app-bar>
    
        <v-content>
            <Test/>
            <HelloWorld/>
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
        data: () => ({
            //
        }),
    };
</script>
