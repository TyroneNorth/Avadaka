<template>
  <q-page-container>
    <q-page>
      <div class="row q-ma-md q-pa-md">
        <div class="col.auto col-md-5 custom-trans">
          <div class="text-h2 q-mb-md text-weight-bold">
            The Ultimate Website Builder
          </div>
          <div class="text-h5 q-mb-md">
            Trusted by beginners, marketers & professionals; Built with
            usability and performance in mind.
          </div>
          <div>
            <q-btn
              rounded
              class="q-pa-md"
              dense
              color="black"
              label="Start Building"
              icon-right="arrow_forward"
            ></q-btn>
          </div>
          <q-separator class="q-mt-lg q-mb-lg"></q-separator>
          <div class="row">
            <div class="text-h4 text-bold q-mr-lg col">800k+</div>

            <div class="text-h4 text-bold col">24k+</div>
          </div>
          <div class="row">
            <div class="text-subtitle col q-mr-sm">People Trust Avadaka</div>

            <div class="text-subtitle col">Average 5-Star Reviews</div>
          </div>
        </div>
        <div class="col.auto col-md-7">
          <q-img src="src/static/hero.png" />
        </div>
      </div>
      <marketing-cards class="q-mb-xl q-mt-xl"></marketing-cards>
      <design-section class="q-ma-xl"></design-section>
      <a-i-o-section></a-i-o-section>
      <f-a-q class="q-ma-xl"></f-a-q>
      <success-section class="q-ma-xl"></success-section>
      <footer-section></footer-section>
    </q-page>
  </q-page-container>
</template>

<script setup lang="ts">
import MarketingCards from 'src/components/MarketingCards.vue';
import DesignSection from 'src/components/DesignSection.vue';
import AIOSection from '../components/AIOSection.vue';
import FAQ from '../components/FAQ.vue';
import SuccessSection from '../components/SuccessSection.vue';
import FooterSection from '../components/FooterSection.vue';
</script>

<style scoped lang="scss">
/* animate row */
</style>
