<script setup>

</script>

<template> 
    <v-container max-width="100%">
            <v-row>
                <v-carousel>
                    <v-carousel-item src="/land1.jpg"cover></v-carousel-item>
                </v-carousel>
            </v-row>
    </v-container>

<!--What is offered-->
    <v-container>
            <h2 class="text-h4 text centre font-weight-bold mb-6">What we offer</h2>
        <v-row justify="centre">
            <v-col cols="12" sm="6">
                <v-card class="rounded-lg overflow-hidden"elevation="4" height="250">
                    <v-img 
                    src="/personal.jpg" cover
                    height="100%"
                        gradient="to bottom, rgba(0,0,0,0) 20%, rgba(0,0,0,0.8) 90%"
                        class="align-end">
                <v-card-text class="pa-6">
                    <div class="text-h5 font-weight-bold text-white">Personal Training</div>
                    <div class="text-body-2 text-grey-lighten-2">We ensure that everyone gets the right attention to improve on themselves.</div>
                    </v-card-text>
                 </v-img>
        </v-card>
      </v-col>
           
            <v-col cols="12" sm="6">
                <v-card class="rounded-lg overflow-hidden"elevation="4" height="250">
                    <v-img 
                    src="/groupclasses.jpg" cover
                    height="100%"
                        gradient="to bottom, rgba(0,0,0,0) 20%, rgba(0,0,0,0.8) 90%"
                        class="align-end">
                <v-card-text class="pa-6">
                    <div class="text-h5 font-weight-bold text-white">Group Classes</div>
                    <div class="text-body-2 text-grey-lighten-2">High energy sessions with professional guidance.</div>
                    </v-card-text>
                 </v-img>
        </v-card>
      </v-col>
          
            <v-col cols="12" sm="6">
                <v-card class="rounded-lg overflow-hidden"elevation="4" height="250">
                    <v-img 
                    src="/strengthtrain.jpg" cover
                    height="100%"
                        gradient="to bottom, rgba(0,0,0,0) 20%, rgba(0,0,0,0.8) 90%"
                        class="align-end">
                <v-card-text class="pa-6">
                    <div class="text-h5 font-weight-bold text-white">Strength Training</div>
                    <div class="text-body-2 text-grey-lighten-2">Build power and endurance with expert coaching.</div>
                    </v-card-text>
                 </v-img>
        </v-card>
      </v-col>
         
            <v-col cols="12" sm="6">
                <v-card class="rounded-lg overflow-hidden"elevation="4" height="250">
                    <v-img 
                    src="/wellness.jpg" cover
                    height="100%"
                        gradient="to bottom, rgba(0,0,0,0) 20%, rgba(0,0,0,0.8) 90%"
                        class="align-end">
                <v-card-text class="pa-6">
                    <div class="text-h5 font-weight-bold text-white">Wellness Recovery</div>
                    <div class="text-body-2 text-grey-lighten-2">Holistic approaches to maintain balance.</div>
                    </v-card-text>
                 </v-img>
        </v-card>
      </v-col>
        </v-row>
    </v-container>

    <!--Success Stories-->
     <v-container>
          <h2 class="text-h4 text centre font-weight-bold mb-6">Success Stories</h2>
        <v-row justify="centre">      
             <v-col md="4">
                <v-card>
                    <v-img src="/james.jpg" cover></v-img>
                    <v-card-title>James lost 30 pounds!</v-card-title>
                    <v-card-text>In just a span of two weeks I was able to loose 30 pounds thanks to the expert trainers in Macfit Gyms</v-card-text>
                </v-card>
            </v-col>
                         <v-col md="4">
                <v-card>
                    <v-img src="/sarah.jpg" cover></v-img>
                    <v-card-title>Sarah, gold champ!</v-card-title>
                    <v-card-text>Thanks to Macfit gym I was able to push myself to the limit and won a gold medal in the Tokyo Olympics games in short distance sprint.</v-card-text>
                </v-card>
            </v-col>
        </v-row>
     </v-container>

     <!--Meet your trainer-->
    <v-container>     
        <h2 class="text-h4 text centre font-weight-bold mb-6">Meet Your Trainer</h2>
        <v-row justify="centre">
            <v-col md="4"> 
            <v-card>
                    <v-img src="/Mark.jpg" cover></v-img>
                    <v-card-title>Mark Headcoach</v-card-title>
                    <v-card-text>Mark (Headcoach) has three decades of experience and has transformed countless people into fit champions.</v-card-text>
                    <v-btn color="#EF237F">View Profile</v-btn>
             </v-card>
      </v-col>
           <v-col md="4">
            <v-card>
                    <v-img src="/Lucy.jpg" cover></v-img>
                    <v-card-title>Lucy</v-card-title>
                    <v-card-text>Lucy (coach) has 15 years of experience and has participated in several fitness tournaments and has not lost a single one!.</v-card-text>
                    <v-btn color="#EF237F">View Profile</v-btn>
             </v-card>
             </v-col>
            </v-row> 
            
             <!--News-->           
            <h2 class="text-h4 text centre font-weight-bold mb-6">Latest News</h2>
            <v-row justify="centre">
                <v-col md="4"> 
                <v-card>
                        <v-img src="/dogwalking.jpg" cover></v-img>
                        <v-card-title>Dog walking gains momentum</v-card-title>
                        <v-card-text>Dog walking has been officially rebranded as a top-tier "longevity workout" for owners this year. New health data shows that owners who walk their dogs average 2,760 more steps per day than those without pets. Experts report that this consistent, moderate-intensity movement helps 87% of dog owners meet their weekly cardio goals.</v-card-text>
                        <v-btn color="#EF237F">Read More</v-btn>
                </v-card>
        </v-col>
            <v-col md="4">
                <v-card>
                        <v-img src="/yoga.jpg" cover></v-img>
                        <v-card-title>Yoga as a new form of excercise!</v-card-title>
                        <v-card-text>Yoga is no longer just a trend; it is a global health powerhouse. In 2026, the global yoga market has surged to an estimated $130 billion as millions pivot toward "longevity-focused" training. Experts report that practitioners are moving away from high-impact burnout in favor of mobility, joint health, and nervous-system regulation.</v-card-text>
                        <v-btn color="#EF237F">Read More</v-btn>
                </v-card>
                </v-col>
                </v-row> 
     </v-container>
     <v-img
    src="news1.jpg"
    cover
    class="text-white py-10"
    :gradient="'to bottom, rgba(0,0,0,0.7), rgba(0,0,0,0.8)'"
  >
   <v-container class="fill-height">
    
    <v-row justify="center" align="center" class="mb-2">
      <v-col cols="12" class="text-center">
          <span class="font-weight-bold">Get in touch</span>
          <span class="ml-4">0712 345 678 | macfitgym@gmail.com</span>
        </v-col>        
      </v-row>

      <v-row justify="center" align="center" class="mb-4">
      <v-col cols="12" class="text-center">
         Opening hours - Mon-Fri: 5.00am - 9.00pm | Sat: 5.00am-6.00pm
        </v-col>
      </v-row>

      <v-row justify="center" align="center" class="mb-6">
      <v-col cols="12" class="text-center">
          Location - Macfit Gym, 3rd Floor, Gateway Mall, Enterprise Road
        </v-col>
      </v-row>

      <v-divider class="mb-4" color="white"></v-divider>
     <v-row justify="center" align="center" class="mb-10">  
        <v-col cols="12" class="text-caption text-center">
            © 2025 Macfit Gym. Designed by Ryan Kimani
        </v-col>  
        </v-row>
    </v-container>
  </v-img>
</template>