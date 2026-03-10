<script setup>
 import { ref } from 'vue'

  const rules = {
    required: value => !!value || 'Required.',
    min: v => v.length >= 8 || 'Min 8 characters',
    emailMatch: () => (`The email and password you entered don't match`),
  }

  const show1 = ref(false)
  const show2 = ref(true)
  const password = ref(null)

  const confirmPassword = ref(null)
  const show1confirm = ref(false)
</script>

<template>
    <v-container width="50%" class="text-centre mt-12" style="background-color:#CFD0D6">
        <v-row>
            <v-col md="12">
                <v-form>
                    <v-row>
                        <v-col md="12">
                            <v-icon color="#EF237F" icon="mdi-weight-lifter" size="large" class="mt-8"></v-icon>
                        </v-col>
                    </v-row>
                    <v-row>
                        <v-col md="12">
                            <div class="text-display-small font-weight-medium">Sign up to Macfit Gym</div>
                        </v-col>
                    </v-row>
                    <v-row>                                                       <!--firstname-->
                        <v-col md="6">
                            <div class="text-title-large font-weight-medium text-right">Firstname</div>
                        </v-col>
                        <v-col md="6">
                            <v-text-field variant="outlined"></v-text-field>
                        </v-col>
                    </v-row>
                     <v-row>                                                       <!--Seconname-->
                        <v-col md="6">
                            <div class="text-title-large font-weight-medium text-right">Secondname</div>
                        </v-col>
                        <v-col md="6">
                            <v-text-field variant="outlined"></v-text-field>
                        </v-col>
                    </v-row>
                     <v-row>                                                       <!--Email-->
                        <v-col md="6">
                            <div class="text-title-large font-weight-medium text-right">Email</div>
                        </v-col>
                        <v-col md="6">
                            <v-text-field variant="outlined"></v-text-field>
                        </v-col>
                    </v-row>
                     <v-row>                                                       <!--Phone Number-->
                        <v-col md="6">
                            <div class="text-title-large font-weight-medium text-right">Phone Number</div>
                        </v-col>
                        <v-col md="6">
                            <v-text-field variant="outlined" type="number"></v-text-field>
                        </v-col>
                    </v-row>
                     <v-row>                                                       <!--Gender-->
                        <v-col md="6">
                            <div class="text-title-large font-weight-medium text-right">Gender</div>
                        </v-col>
                        <v-col md="6">
                            <v-radio-group inline>
                                <v-radio label="Male" value="male"></v-radio>
                                <v-radio label="Female" value="female"></v-radio>                                
                                </v-radio-group>
                        </v-col>
                    </v-row>
                     <v-row>                                                       <!--Date of Birth-->
                        <v-col md="6">
                            <div class="text-title-large font-weight-medium text-right">Date of Birth</div>
                        </v-col>
                        <v-col md="6">
                            <v-date-input variant="outline"></v-date-input>
                        </v-col>
                    </v-row>
                    <v-row>                                                       <!--Gym location-->
                        <v-col md="6">
                            <div class="text-title-large font-weight-medium text-right">Gym location</div>
                        </v-col>
                        <v-col md="6">
                            <v-select
                                label="Select"
                                :items="['CBD', 'Madaraka', 'Westlands', 'Buruburu']"
                                variant="outlined"
                                ></v-select>
                        </v-col>
                    </v-row>
                    <v-row>                                                       <!--Password-->
                        <v-col md="6">
                            <div class="text-title-large font-weight-medium text-right">Password</div>
                        </v-col>
                        <v-col md="6">
                            <v-text-field
                                v-model="password"
                                    :append-icon="show1 ? 'mdi-eye' : 'mdi-eye-off'"
                                    :rules="[rules.required, rules.min]"
                                    :type="show1 ? 'text' : 'password'"                                   
                                    variant="outlined"                               
                                    @click:append="show1 = !show1"
                            ></v-text-field>
                        </v-col>
                    </v-row>
                                        <v-row>                                                       <!--Confirm Password-->
                        <v-col md="6">
                            <div class="text-title-large font-weight-medium text-right">Confirm Password</div>
                        </v-col>
                        <v-col md="6">
                            <v-text-field
                                v-model="confirmPassword"
                                    :append-icon="show1confirm ? 'mdi-eye' : 'mdi-eye-off'"
                                    :rules="[rules.required, rules.min]"
                                    :type="show1confirm ? 'text' : 'password'"                                   
                                    variant="outlined"                               
                                    @click:append="show1 = !show1"
                            ></v-text-field>
                        </v-col>
                    </v-row>
                    <v-row>
                        <v-col md="12">
                            <v-btn color="#EF237F" variant="elevated">Log in</v-btn>
                        </v-col>
                    </v-row>
                    <v-row>
                        <v-col md="12">
                            <div>New to MacFit Gym? Create an account</div>
                        </v-col>
                    </v-row>
                </v-form>
            </v-col>
        </v-row>
    </v-container>
</template>