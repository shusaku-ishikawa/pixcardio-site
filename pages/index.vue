<template>
  <div>
    <section
    style="position: relative">
      <v-img
      style="width: 100%"
      src="/top.jpg"></v-img>
      <div
      class="text-md-h5 text-xs-body-2 white--text"
      style="position: absolute; bottom: 1rem; left:1rem">
        Artificial intelligence assistance for everyone<br v-if="$vuetify.breakpoint.smAndUp"> who analyzes intracoronary imaging.
      </div>
    </section>
    <v-container>
      <v-row class="justify-center">
        <v-col cols="12">
          <section class="mb-10">
            <div class="text-body-1 text-sm-h5 text-md-h4 font-weight-bold grey--text text--darken-1">
              <i>PIXCARDIO provides a web-based AI-powered software to analyze intracoronary imaging
              including intravascular ultrasound (IVUS) and optical coherence tomography (OCT).</i>
            </div>
          </section>
          <section class="mb-10 text-center">
            <v-btn
            color="primary"
            dark
            x-large
            rounded
            @click="goToApp()">
            Get Started - Sign up</v-btn>
          </section>
          <section class="mb-10">
            <div class="text-h4 text-center font-weight-bold">
              Features
            </div>
            <v-card>
              <v-card-text class="text-body-1 text-sm-h6 text-md-h6 font-weight-bold px-10" >
                <v-list>
                  <v-list-item>
                    <v-icon color="success">done_outline</v-icon>
                    <div class="ml-3 grey--text text--darken-2">Auto Segmentation</div>
                  </v-list-item>
                  <v-list-item>
                    <v-icon color="success">done_outline</v-icon>
                    <div class="ml-3 grey--text text--darken-2">Manual Editing</div>
                  </v-list-item>
                  <v-list-item>
                    <v-icon color="success">done_outline</v-icon>
                    <div class="ml-3 grey--text text--darken-2">Reporting</div>
                  </v-list-item>
                </v-list>
              </v-card-text>
            </v-card>
          </section>
          <section class="mb-10">
            <div class="text-h4 text-center font-weight-bold">
              Why PIXCARDIO?
            </div>
            <v-row>
              <v-col cols="12" sm="4" md="4">
                <v-card elevation="3">
                  <v-card-text class="text-h6 font-weight-bold text-center">
                    <div class="text-center">
                      <v-icon color="success">language</v-icon>
                      <div>All Web-Based</div>
                    </div>
                  </v-card-text>
                </v-card>
              </v-col>
              <v-col cols="12" sm="4" md="4">
                <v-card elevation="3">
                  <v-card-text class="text-h6 font-weight-bold text-center">
                    <div class="text-center">
                      <v-icon color="success">bubble_chart</v-icon>
                      <div>Essential Analysis</div>
                    </div>
                  </v-card-text>
                </v-card>
              </v-col>
              <v-col cols="12" sm="4" md="4">
                <v-card elevation="3">
                  <v-card-text class="text-h6 font-weight-bold text-center">
                    <div class="text-center">
                      <v-icon color="success">attach_money</v-icon>
                      <div>Affordable</div>
                    </div>
                  </v-card-text>
                </v-card>
              </v-col>
            </v-row>
          </section>
          <section class="mb-10">
            <div class="text-h4 text-center font-weight-bold">
              Pricing
            </div>
            <v-row>
              <v-col cols="12" sm="6" md="6">
                <div class="pricing-block ">
                  <div class="price-header">
                      <h4 class="price"><small>$</small>0</h4>
                      <h5>FREE</h5>
                  </div>
                  <div class="line"></div>
                  <ul>
                      <li>Max. 3 cases.</li>
                      <li>Unlimited Auto segmentations</li>
                      <li>Analytic Report(extra charge)</li>
                  </ul>
                </div>
              </v-col>
              <v-col cols="12" sm="6" md="6">
                <div class="pricing-block ">
                  <div class="price-header">
                      <h4 class="price"><small>$</small>9</h4>
                      <h5>ECONOMY</h5>
                  </div>
                  <div class="line"></div>
                  <ul>
                      <li>Max. 50 cases.</li>
                      <li>Unlimited Auto segmentations</li>
                      <li>Analytic Report(No charge)</li>
                  </ul>
                </div>
              </v-col>
              <!-- <v-col cols="12" sm="4" md="4">
               <div class="pricing-block">
                    <div class="price-header">
                      <h4 class="price"><small>$</small>30</h4>
                      <h5>PRO</h5>
                    </div>
                    <div class="line"></div>
                    <ul>
                        <li>Unlimited cases.</li>
                        <li>Unlimited Auto segmentations</li>
                        <li>Analytic Report(no charge)</li>
                    </ul>

                </div>
              </v-col> -->
            </v-row>
          </section>
          <section class="text-center">
            <div class="text-h4 text-center font-weight-bold">
              About us
            </div>
            <h3>PIXCARDIO LLC</h3>
            <h4>
              <v-icon>mail</v-icon>
              <a href="mailto:info@pixcardio.com">info@pixcardio.com</a>
            </h4>
            <h4>
              <i class="fas fa-location-arrow"></i>
              651 N Broad St, Suite 205 #2319
              Middletown, Delaware 19709
            </h4>
          </section>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>
<style scoped>
@import url('@/assets/pricing.css');
</style>

<script>
export default {
  components: {
  },
  methods: {
    goToApp() {
      window.open('https://pixcardio.com/', '_blank')
    }
  }
}
</script>
