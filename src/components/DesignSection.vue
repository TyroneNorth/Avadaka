<template>
  <div class="row justify-center">
    <q-img
      class="img-center"
      :src="'src/static/avadaka.png'"
      style="height: 140px; max-width: 150px"
    ></q-img>
  </div>
  <div class="text-center text-bold text-h3">
    Design Anything, Build Everything
  </div>
  <div class="text-center text-subtitle1 q-mt-md">
    Design and launch your website fast & no coding knowledge is required.
  </div>

  <div class="row text-bold q-ma-lg">
    <div
      class="class-buttons column justify-start items-start col-md-4 col-sm-12 col.auto"
    >
      <q-btn
        flat
        rounded
        class="q-pa-lg"
        icon="grid_view"
        label="Live Visual Builder"
      ></q-btn
      ><q-btn
        flat
        rounded
        class="q-pa-lg"
        icon="space_dashboard"
        label="Layout Builder"
      ></q-btn
      ><q-btn
        flat
        rounded
        class="q-pa-lg"
        icon="dashboard_customize"
        label="Header Builder"
      ></q-btn
      ><q-btn
        flat
        rounded
        class="q-pa-lg"
        icon="vertical_split"
        label="Footer Builder"
      ></q-btn
      ><q-btn
        flat
        rounded
        class="q-pa-lg"
        icon="view_sidebar"
        label="Form Builder"
      ></q-btn
      ><q-btn
        flat
        rounded
        class="q-pa-lg"
        icon="view_cozy"
        label="Performance Wizard"
      ></q-btn>
    </div>

    <div class="col-sm-12 col-md-8 col.auto">
      <q-img class="img-center" src="src/static/builder1.png"></q-img>
    </div>
  </div>
</template>

<script setup lang="ts"></script>

<style scoped>
@media only screen and (max-width: 991px) {
  .class-buttons {
    align-content: center;
  }
}
</style>
