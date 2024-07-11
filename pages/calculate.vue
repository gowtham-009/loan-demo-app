<template>
    <div class="main-container w-100" :style="{height: deviceHeight + 'px'}" >
      <div class="w-100 boxex-1 bg-blue":style="{height:boxex1Height + 'px'}" ></div>
      <div class="w-100 boxex-2":style="{height:boxex2Height + 'px'}" >
        <v-form>
            <v-container class="pa-0">
                <v-row no-gutters>
                <v-col cols="12" >
                    <v-sheet class="pa-1">
                    <p class="text-center font-weight-bold text-h6 text-blue mb-3">Enter Closing Details SF-AA-0020</p>

                    <v-row no-gutters>
                        <v-col cols="5" >
                            <v-sheet class="pa-1">
                                <v-text-field
                                    v-model="loannumber"
                                    :counter="10"
                                    :rules="loannumberRules"
                                    label="Loan_Number:"
                                    placeholder="SF-AA-0020"
                                    hide-details
                                    required
                                    class="w-100"
                                    ></v-text-field>
                            </v-sheet>
                        </v-col>
                        <v-col cols="7" >
                            <v-sheet class="pa-1">
                                <v-text-field
                                    v-model="loantyps"
                                    :counter="10"
                                    :rules="loantypeRules"
                                    label="Loan Type:"
                                    placeholder="Gold"
                                    hide-details
                                    required
                                    class="w-100"
                                    ></v-text-field>
                            </v-sheet>
                        </v-col>
                        <v-col cols="5" class="pa-0" >
                            <v-sheet class="pa-1">
                                <v-date-input label="Loan Date:" prepend-icon=""></v-date-input>
                            </v-sheet>
                        </v-col>
                        <v-col cols="7" >
                            <v-sheet class="pa-1">
                                <v-text-field
                                    v-model="loanvalue"
                                    :counter="10"
                                    :rules="loanvalueRules"
                                    label="Loan value:"
                                    placeholder="0000"
                                    hide-details
                                    required
                                    class="w-100"
                                    ></v-text-field>
                            </v-sheet>
                        </v-col>
                        </v-row>

                    </v-sheet>
                </v-col>

                <v-col cols="12" >
                    <v-sheet class="pa-1">
                        <v-row no-gutters>
                            <v-col cols="5">
                                <v-sheet class="pa-1 d-flex align-end" >
                                    <v-date-input label="Last Date:" prepend-icon=""></v-date-input>
                                </v-sheet>
                            </v-col>
                            <v-col cols="7">
                                <v-sheet class="pa-1" >
                                <v-text-field
                                    v-model="nan"
                                    :counter="10"
                                    :rules="nanRules"
                                    
                                 
                                    hide-details
                                    required
                                    class="w-100"
                                    ></v-text-field>
                                    <v-btn class="bg-blue text-white" block>Total 7946.2</v-btn>
                                </v-sheet>
                            </v-col>
                            </v-row>
                    </v-sheet>
                </v-col>

                <v-col cols="12" class="pa-1" >
                    <v-sheet>
                        <v-row no-gutters class="pa-0">
                            <v-col cols="5" class="pa-0">
                                <v-sheet class="pa-0" >

                                    <v-col cols="12" class="pa-0">
                                        <v-sheet class="pa-1" >
                                        <span>Collected Extra:</span><br>
                                        <span>19955.10:</span>
                                        </v-sheet>
                                    </v-col>

                                    <v-col cols="12" class="pa-0 mt-2">
                                        <v-sheet class="pa-1" >
                                            <span>Intrest:</span><br>
                                            <span>19955.10:</span>
                                        </v-sheet>
                                    </v-col>

                                    <v-col cols="12" class="pa-0 mt-2">
                                        <v-sheet class="pa-1" >
                                            <span>Book Value:</span><br>
                                            <span>7555.10:</span>
                                        </v-sheet>
                                    </v-col>

                                </v-sheet>
                            </v-col>
                            <v-col cols="7">
                                <v-sheet class="pa-0" >
                                    
                                    <v-col cols="12" class="pa-0">
                                        <v-sheet class="pa-1" >
                                            <v-text-field
                                                v-model="nan"
                                                :counter="10"
                                                :rules="nanRules"
                                                placeholder="-5600.00"
                                            
                                                hide-details
                                                required
                                                class="w-100"
                                                ></v-text-field>
                                        </v-sheet>
                                    </v-col>

                                    <v-col cols="12" class="pa-0">
                                        <v-sheet class="pa-1" >
                                            <v-text-field
                                                v-model="nan"
                                                :counter="10"
                                                :rules="nanRules"
                                                placeholder="-5600.00"
                                            
                                                hide-details
                                                required
                                                class="w-100"
                                                ></v-text-field>
                                        </v-sheet>
                                    </v-col>

                                    <v-col cols="12" class="pa-0">
                                        <v-sheet class="pa-1" >
                                            <v-text-field
                                                v-model="nan"
                                                :counter="10"
                                                :rules="nanRules"
                                                placeholder="000"
                                            
                                                hide-details
                                                required
                                                class="w-100"
                                                ></v-text-field>
                                        </v-sheet>
                                    </v-col>

                                </v-sheet>
                            </v-col>
                            </v-row>
                    </v-sheet>
                </v-col>
                
                <v-col cols="12" >
                    <v-sheet class="pa-1">
                        <v-row no-gutters>
                            <v-col cols="5">
                                <v-sheet class="pa-1" >
                                <span>Office Book:</span><br>
                                <span>0.000:</span>
                                </v-sheet>
                            </v-col>
                            <v-col cols="7">
                                <v-sheet class="pa-1" >
                                    <v-text-field
                                    v-model="nan"
                                    :counter="10"
                                    :rules="nanRules"
                                    placeholder="000"
                                
                                    hide-details
                                    required
                                    class="w-100"
                                    ></v-text-field>
                                </v-sheet>
                            </v-col>
                            </v-row>
                    </v-sheet>
                </v-col>
                
                </v-row>
            </v-container>
        </v-form>
      </div>
  
      <div class="w-100 d-flex ga-3 pa-4 align-center" :style="{height:boxex3Height + 'px'}" >
          <div class="w-100"><v-btn class="bg-blue text-white" block>7946.2</v-btn></div>
          <div class="w-100"><nuxt-link to="/dashboard" style="text-decoration: none;"><v-btn class="bg-green text-white" block>Submit & Close</v-btn></nuxt-link></div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        deviceWidth: 0,
        deviceHeight: 0,
        boxex1Height: 0,
        boxex2Height: 0,
        boxex3Height: 0
        
  
      };
    },
    mounted() {
      this.updateDeviceDimensions(); // Initial call to set dimensions on component mount
      window.addEventListener('resize', this.updateDeviceDimensions); // Listen for window resize events
    },
    beforeDestroy() {
      window.removeEventListener('resize', this.updateDeviceDimensions); // Clean up: remove resize event listener
    },
    methods: {
      updateDeviceDimensions() {
        this.deviceWidth = window.innerWidth; // Update device width
        this.deviceHeight = window.innerHeight; // Update device height
  
        // Calculate heights for each boxex based on percentages
        this.boxex1Height = Math.floor(this.deviceHeight * 0.05); // 6% of device height
        this.boxex2Height = Math.floor(this.deviceHeight * 0.90); // 88% of device height
        this.boxex3Height = Math.floor(this.deviceHeight * 0.05); // 6% of device height
       
      },
      
  
    }
  };
  </script>
  
  <style scoped>
  
  
  
  </style>
  