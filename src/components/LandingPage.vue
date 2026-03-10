<script setup>

</script>

<template>
    <v-container max-width="100%">
        <v-row>
            <v-carousel>
                <v-carousel-item src="/land1.jpg"cover></v-carousel-item>
                <v-carousel-item src="/land2.jpg"cover></v-carousel-item>
                <v-carousel-item src="/land3.jpg"cover></v-carousel-item>
            </v-carousel>
        </v-row>
    </v-container>

<!-- About Us -->
     <v-container style="background-color:#CFD0D6" max width="100%">
        <v-row >
            <v-col md="6" class="text-centre">
                <div class="text-display-medium mb-12">MacFit: Elevate Your Standard</div>
                <div class="text-title-large font-weight-light text-medium-emphasis mb-8">At MacFit, fitness is a lifestyle. We provide a high-energy sanctuary where beginners and athletes alike push their limits.</div>
                <div class="text-title-large font-weight-light text-medium-emphasis mb-8">Train with world-class strength and cardio technology. Our certified trainers bring expert guidance, offering the perfect balance of group energy and personalized coaching.</div>
                <div class="text-title-large font-weight-light text-medium-emphasis mb-8">We focus on sustainable progress in a modern, grit-driven environment. At MacFit, we don’t just build muscle; we build the consistency you need to be better than yesterday.</div>
                <v-btn color="#EF237F">LEARN MORE</v-btn>
            </v-col>
            <v-col md="6">
            <v-container class="d-flex align-center justify-center fill-height">
                <v-img src="/aboutus.jpg"></v-img>
            </v-container>
            </v-col>
        </v-row>
     </v-container>

       <v-container>
        <v-row>
            <v-col md="4">
                <v-card>
                    <v-img src="/news1.jpg" cover></v-img>
                    <v-card-title>Have you tried the treadmill?</v-card-title>
                    <v-card-text>It enables you to build more on your leg muscles while getting a good run. Join us to get the best equipment and training.</v-card-text>
                    <v-btn color="#EF237F">READ MORE</v-btn>
                </v-card>
            </v-col>
             <v-col md="4">
                <v-card>
                    <v-img src="/news2.jpg" cover></v-img>
                    <v-card-title>Time to build those triceps</v-card-title>
                    <v-card-text>Not only do we provide the best equipment but also the trainers with decades of knowledge to help you achive your dream of a perfect body.</v-card-text>
                    <v-btn color="#EF237F">READ MORE</v-btn>
                </v-card>
            </v-col>
             <v-col md="4">
                <v-card>
                    <v-img src="/news3.jpg" cover></v-img>
                    <v-card-title>Outdoors excercise</v-card-title>
                    <v-card-text>Not an indoor guy but still want to be fit? We offer outdoor activities such as planed bicycle rides, hicking and much more.</v-card-text>
                    <v-btn color="#EF237F">READ MORE</v-btn>
                </v-card>
            </v-col>
        </v-row>
    </v-container>

    <!--Reviews-->
    <v-container>
        <v-row>
            <v-col md="3">
                <v-card color="#CFD0D6">
                <v-card-text>Best gym in Nairobi.I have no regrets joining it. </v-card-text>
                <v-rating :lenght="5" :size="32" :model-value="4" active-colour="primary"></v-rating>
                </v-card>
            </v-col>
            <v-col md="3">
                <v-card color="#CFD0D6">
                <v-card-text>I am impressed by the quality of services and equipment they have to offer. </v-card-text>
                <v-rating :lenght="5" :size="32" :model-value="5" active-colour="primary"></v-rating>
                </v-card>
            </v-col>
            <v-col md="3">
                <v-card color="#CFD0D6">
                <v-card-text> Not bad.The community in MacFit is the best and it helps in motivation to better than before.  </v-card-text>
                <v-rating :lenght="5" :size="32" :model-value="4" active-colour="primary"></v-rating>
                </v-card>
            </v-col>
        </v-row>
    </v-container>

<!--Contact Us-->
     <v-container style="background-color:#CFD0D6" max width="100%">
        <v-row class="text-centre">
            <div class="text-title-large font-weight-light text-medium-emphasis mb-8">Get in touch</div>
            <div class="text-title-large font-weight-light text-medium-emphasis mb-8">0712 345 678 | macfitgym@gmail.com</div>
            <div class="text-title-large font-weight-light text-medium-emphasis mb-8">Opening hours</div>
            <div class="text-title-large font-weight-light text-medium-emphasis mb-8">Mon-Fri: 5.00am - 9.00pm | Sat: 5.00am-6.00pm</div>
            <div class="text-title-large font-weight-light text-medium-emphasis mb-8">Location - Macfit Gym,3rd Floor,Gateway Mall, Enterprise Road</div>
            <div class="text-title-large font-weight-light text-medium-emphasis mb-8">&copy; 2025 Macfit Gym. Designed by Ryan Kimani</div>
        </v-row>
     </v-container>
        

</template>