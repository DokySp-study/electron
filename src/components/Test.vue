<template>
    <v-layout row wrap>
        <v-flex xs12 sm4>
            <v-chip color="red" text-color="white">
                {{msg1}}
            </v-chip>
        </v-flex>
        <v-flex xs12 sm4>
            <v-chip color="orange" text-color="white">
                {{msg2}}
            </v-chip>
        </v-flex>
        <v-flex xs12 sm4>
            <v-chip color="green" text-color="white">
                {{msg3}}
            </v-chip>
        </v-flex>
    </v-layout>
</template>

<script>
    export default {
        name: "test",
        data() {
            return {
                msg1: "asdf",
                msg2: "sasdf",
                msg3: "asdf",
            }
        },
    }
</script>

<style>
    
</style>
