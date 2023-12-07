<style lang="sass" scoped>
.upper-div
  a
    text-decoration: none
    color: #101010

.highlight
  a
    text-decoration: underline
    color: #ffd1dc

</style>

<template>
  <q-layout view="hhh LpR fFf">
    <q-header v-if="Platform.is.mobile" class="bg-transparent">
      <q-btn flat dense rounded icon="mdi-menu" color="dark" class="q-ma-md" @click="toggleLeftDrawer" />
    </q-header>

    <q-drawer :width="360" show-if-above v-model="leftDrawerOpen" side="left" bordered elevated>
      <q-btn v-if="Platform.is.mobile" @click="leftDrawerOpen = !leftDrawerOpen" flat dense icon="mdi-menu" color="dark" class="q-ma-md absolute-top-right"/>
      <div class="column q-gutter-y-md text-h6 text-weight-light content-center window-height flex flex-center upper-div">
        <router-link to="/" :style="routeName === 'home' ? 'border-bottom: 1px solid #ffd1dc; color: #101010' : 'color: grey'" class="q-px-md">Home</router-link>
        <router-link to="about" :style="routeName === 'about' ? 'border-bottom: 1px solid #ffd1dc; color: #101010' : 'color: grey'" class="q-px-md">About</router-link>
        <router-link to="service" :style="routeName === 'service' ? 'border-bottom: 1px solid #ffd1dc; color: #101010' : 'color: grey'" class="q-px-md">Service</router-link>
        <router-link to="contact" :style="routeName === 'contact' ? 'border-bottom: 1px solid #ffd1dc; color: #101010' : 'color: grey'" class="q-px-md">Contact</router-link>
        <span class="text-grey-7 text-subtitle1 q-mt-xl">@2023</span>
      </div>
    </q-drawer>

    <q-page-container>
      <router-view />
    </q-page-container>

  </q-layout>
</template>

<script setup>
import { ref, watch, onMounted } from 'vue';
import { Platform } from 'quasar'
import { useRouter } from 'vue-router';

const leftDrawerOpen = ref(false)
const router = useRouter()
const routeName = ref('');

const toggleLeftDrawer = () => {
  leftDrawerOpen.value = !leftDrawerOpen.value
}

onMounted(() => {
  routeName.value = router.currentRoute.value.name;
})

watch(() => router.currentRoute.value.name, () => {
  routeName.value = router.currentRoute.value.name;
})
</script>
