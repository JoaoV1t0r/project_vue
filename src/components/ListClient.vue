<template>
    <div class="d-flex align-content-space-around flex-wrap">
        <v-list v-for="(client, i) in clients" :key="i"  dense >
            <v-card
                class="mx-2 px-2 py-2"
                max-width="350"
                outlined
            >
                <v-list-item three-line>
                    <v-list-item-content>
                        <v-list-item-title class="text-h5 mb-1">
                            <h5>
                                {{client.name}}
                            </h5>
                        </v-list-item-title>
                    </v-list-item-content>

                    <v-list-item-avatar>
                        <v-img  :src="client.photo"></v-img>
                    </v-list-item-avatar>
                </v-list-item>
                
                <v-btn
                    color=""
                    outlined
                    rounded
                    text
                    class="mx-auto"
                >
                    Detalhes do Cliente
                </v-btn>

            </v-card>
        </v-list>
    </div>
</template>

<script lang="ts">
import  Vue  from 'vue';


export default Vue.extend({
    name: 'ListClient',

    data:()=>({
        clients:[
            {
                name:"Nome Cliente",
                photo:"https://avatars0.githubusercontent.com/u/3?v=4&s=460"
            },
            {
                name:"Nome Cliente",
                photo:"https://avatars0.githubusercontent.com/u/23?v=4&s=460"
            },
            {
                name:"Nome Cliente",
                photo:"https://avatars0.githubusercontent.com/u/95?v=4&s=460"
            },
            {
                name:"Nome Cliente",
                photo:"https://avatars0.githubusercontent.com/u/1?v=4&s=460"
            },
            {
                name:"Nome Cliente",
                photo:"https://avatars0.githubusercontent.com/u/96851?v=4&s=460"
            },
            {
                name:"Nome Cliente",
                photo:"https://avatars0.githubusercontent.com/u/9641?v=4&s=460"
            },
            {
                name:"Nome Cliente",
                photo:"https://avatars0.githubusercontent.com/u/984?v=4&s=460"
            },
            {
                name:"Nome Cliente",
                photo:"https://avatars0.githubusercontent.com/u/96851?v=4&s=460"
            },
            {
                name:"Nome Cliente",
                photo:"https://avatars0.githubusercontent.com/u/9641?v=4&s=460"
            },
            {
                name:"Nome Cliente",
                photo:"https://avatars0.githubusercontent.com/u/984?v=4&s=460"
            },
        ]
    })
})
</script>