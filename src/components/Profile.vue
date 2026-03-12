<script setup>
 localStorage.setItem('userDetails', JSON.stringify(userDetails))

</script>

<template>
   <v-container width="50%"  style="background-color:#CFD0D6" class="mt-12">
        <v-row>
            <v-col>
                <v-card>
                    <v-img src="" class="h-50" cover></v-img>
                    <v-card-title>{{userDetails.name}}</v-card-title>
                   
                    <v-card-text>{{userDetails.email }}</v-card-text>
                    <v-card-text>{{userDetails.phone }}</v-card-text>
                    <v-card-text>{{userDetails.gymLocation }}</v-card-text>                    
                    <div v-if="userDetails.subscription">
                     <v-card-text>Your current subscription is:{{userDetails.subscription }} at {{userDetails.subscription.prize }}</v-card-text>   
                    </div>
                    <div v-else>
                        <v-btn colon="primary" variant="between"></v-btn>
                    </div>
                </v-card>
            </v-col>
        </v-row>
   </v-container>
    
</template>