<template>
  <q-layout view="hHh lpR fFf">
    <q-header reveal class="text-black">
      <q-toolbar class="absolute-center">
        <!--<q-btn dense flat round icon="menu" @click="toggleLeftDrawer" />-->

        <q-btn flat rounded size="xl" eager label="Avadaka">
          <q-img
            src="src/static/avadaka.png"
            ratio="4/3"
            style="height: 40px; width: 40px"
          />
        </q-btn>
        <q-btn-group rounded flat class="absolute-center">
          <q-btn-dropdown
            rounded
            no-caps
            flat
            label="Features"
            dropdown-icon="expand_more"
          >
            <q-list>
              <q-item clickable v-close-popup @click="onItemClick">
                <q-item-section>
                  <q-item-label size="xl">Elements</q-item-label>
                </q-item-section>
              </q-item>

              <q-item clickable v-close-popup @click="onItemClick">
                <q-item-section>
                  <q-item-label>Prebuilt Websites</q-item-label>
                </q-item-section>
              </q-item>

              <q-item clickable v-close-popup @click="onItemClick">
                <q-item-section>
                  <q-item-label>Reviews</q-item-label>
                </q-item-section>
              </q-item>
            </q-list>
          </q-btn-dropdown>
          <q-btn no-caps flat label="Elements" />
          <q-btn no-caps flat label="Prebuilt Websites" />
          <q-btn no-caps flat label="Reviews" />
        </q-btn-group>
        <q-btn
          rounded
          class="absolute-right q-mr-lg"
          outline
          label="What's new"
          icon="auto_awesome"
        ></q-btn>
      </q-toolbar>
    </q-header>

    <q-drawer
      :width="300"
      :breakpoint="2000"
      persistent
      show-if-above
      v-model="leftDrawerOpen"
      side="left"
    >
      <!-- drawer content -->
    </q-drawer>
    <q-drawer
      :width="300"
      :breakpoint="2000"
      persistent
      show-if-above
      v-model="rightDrawerOpen"
      side="right"
    >
      <!-- drawer content -->
    </q-drawer>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
import { ref } from 'vue';

export default {
  setup() {
    const leftDrawerOpen = ref(false);

    return {
      leftDrawerOpen,
      toggleLeftDrawer() {
        leftDrawerOpen.value = !leftDrawerOpen.value;
      },
    };
  },
};
</script>

<style lang="scss">
.q-btn {
  letter-spacing: 0.2em;
  font-size: 1rem;
}
.q-header {
  height: 100px;
  background-color: transparent;
  color: black;
}
/* hide headeer on small screens */
@media only screen and (max-width: 1155px) {
  .q-toolbar {
    display: none;
  }
}
.q-toolbar {
  width: 1200px;
}
</style>
