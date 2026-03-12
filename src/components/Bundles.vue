<script setup>
 import { ref } from 'vue'
 import {useRouter} from "vue-router";

const router =useRouter();
const showBundleDialog = ref(false)
const isLoggedIn = localStorage.getItem( "isLoggedIn")
const selectedBundle = ref(null)
const selectedPrice =ref(null)

function showBundle(name, price){
    if(isLoggedIn){
        selectedBundle.value = name
        selectedPrice.value = price
        showBundleDialog.value = true  //open popup       
    }
    else{
        router.push('/login')
    }
}

    function subscribe(){
    const userDetails= JSON.parse(localStorage.getItem('userDetails'))
  userDetails.subscription ={
    name: selectedBundle.value,
     name: selectedPrice.value
  }    
     localStorage.setItem('userDetails', JSON.stringify(userDetails))
     showBundleDialog.value = false
}

</script>

<template>
    <v-container style="background-color:#CFD0D6" class="mt-12">
        <v-row>
            <div class="text-display-medium md-12">Bundles and Pricing</div>             
        </v-row> 
            <v-row>
         <div class="text-label-medium font-italic">Click on a bundle to subscribe</div>
        </v-row>     
         <v-row>
            <v-col md="3">
                <v-card class="text-center" @click="showBundle('Daily Pass', 500)">
                    <v-icon color="#EF237F" icon="mdi-calendar-today-outline" size="large" class="mt-8"></v-icon>
                    <v-card-title color="#EF237F">Daily Pass</v-card-title>
                    <v-card-text>500 Ksh</v-card-text> 
                </v-card>
            </v-col>
            <v-col md="3">
                <v-card class="text-center" @click="showBundle('Month', 15000)">
                    <v-icon color="#EF237F" icon="mdi-calendar-month-outline" size="large" class="mt-8"></v-icon>
                    <v-card-title color="#EF237F">Month</v-card-title>
                    <v-card-text>15000 Ksh</v-card-text> 
                </v-card>
            </v-col>
            <v-col md="3">
                <v-card class="text-center" @click="showBundle('3 Months', 45000)">
                    <v-icon color="#EF237F" icon="mdi-circle-slice-3" size="large" class="mt-8"></v-icon>
                    <v-card-title color="#EF237F">3 Months</v-card-title>
                    <v-card-text>45000 Ksh</v-card-text> 
                </v-card>
            </v-col>
            <v-col md="3">
                <v-card class="text-center" @click="showBundle('6 Months', 90000)">
                    <v-icon color="#EF237F" icon="mdi-circle-slice-6" size="large" class="mt-8"></v-icon>
                    <v-card-title color="#EF237F">6 Months</v-card-title>
                    <v-card-text>90000 Ksh</v-card-text> 
                </v-card>
            </v-col>
        </v-row>       
         <v-row>
           <v-col md="12">
               <v-card class="text-center" @click="showBundle('12 months', 100000)">
                <v-icon color="#EF237F" icon="mdi-calendar-check-outline" size="large"class="mt-8"></v-icon>
                <v-card-title color="#EF237F">12 months</v-card-title>
                <v-card-text>100000 Ksh</v-card-text> 
            </v-card> 
            </v-col>
        </v-row>
    </v-container>
   <!--What's included--> 
   <v-container style="background-color:#CFD0D6" class="mt-12">
    <v-row>
        <v-col md="12">
             <div class="text-display-medium mb-12">What is included in your bundle?</div>
        </v-col>
    </v-row>

      <v-row>
        <v-col md="3">
          <v-card class="text-center">
           <v-icon color="#EF237F" icon="mdi-clock" size="large" class="mt-8"></v-icon>
           <v-card-title color="#EF237F">24/7 gym access</v-card-title>
          </v-card>
        </v-col>
        <v-col md="3">
          <v-card class="text-center">
           <v-icon color="#EF237F" icon="mdi-dumbbell" size="large" class="mt-8"></v-icon>
           <v-card-title color="#EF237F">Dedicated Men's & Ladies' Training</v-card-title>
          </v-card>
        </v-col>
        <v-col md="3">
          <v-card class="text-center">
           <v-icon color="#EF237F" icon="mdi-circle-slice-3" size="large" class="mt-8"></v-icon>
           <v-card-title color="#EF237F">3 Months</v-card-title>
          </v-card>
        </v-col>
        <v-col md="3">
          <v-card class="text-center">
           <v-icon color="#EF237F" icon="mdi-spoon-sugar" size="large" class="mt-8"></v-icon>
           <v-card-title color="#EF237F">Personalized Diet</v-card-title>
          </v-card>
        </v-col>
    </v-row>
    <v-row>
        <v-col md="3">
          <v-card class="text-center">
           <v-icon color="#EF237F" icon="mdi-locker-multiple" size="large" class="mt-8"></v-icon>
           <v-card-title color="#EF237F">Free locker rooms</v-card-title>
          </v-card>
        </v-col>
        <v-col md="3">
          <v-card class="text-center">
           <v-icon color="#EF237F" icon="mdi-shower-head" size="large" class="mt-8"></v-icon>
           <v-card-title color="#EF237F">Hot and cold showers</v-card-title>
          </v-card>
        </v-col>
    </v-row>
   </v-container>
   <!--How to join-->
   <v-container style="background-color:#CFD0D6" class="mt-12">
    <v-row>
        <v-col md="12">
             <div class="text-display-medium mb-12">How to join</div>
        </v-col>
    </v-row>
    <v-row>
        <v-col>
           <v-list>
            <v-list-item>1.Select your preferred bundle.</v-list-item>
            <v-list-item>2.Visit us at our main branch or fill out the online form provided.</v-list-item>
            <v-list-item>3.Make a secure payment at the front desk or via online and send the confirmation message to us via our email.</v-list-item>
            <v-list-item>4.Begin your fitness journey immediately!</v-list-item>
           </v-list>
        </v-col>
    </v-row>
   </v-container>
   <!--dialog-->
     <v-dialog v-model="showBundleDialog" max-width="600" >

      <v-card prepend-icon="mdi-account" title="Subscribe to Bundle" >
        <v-card-text>
          You are about to subscribe to {{ selectedBundle }} at {{ selectedPrice }}. Click on the button below to complete payment
        </v-card-text>

        <v-divider></v-divider>

        <v-card-actions>
         <v-spacer></v-spacer>
          <v-btn text="Close" variant="plain" @click="showBundleDialog = false" ></v-btn>
          <v-btn color="primary" variant="tonal" @click="subscribe()" >Subscribe</v-btn>
        </v-card-actions>
      </v-card>
    </v-dialog>
</template>