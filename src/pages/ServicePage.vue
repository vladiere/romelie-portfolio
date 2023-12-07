<style lang="sass" scoped>
.q-mt-xl
  margin-top: 3em
</style>

<template>
  <q-page padding class="column q-gutter-y-lg q-pb-xl">
    <!-- content -->
    <span class="text-h3 q-mt-xl text-weight-bold">What I Do</span>

    <div :class="!Platform.is.mobile ? 'q-mt-lg row q-gutter-x-lg justify-center' : 'column q-gutter-y-lg items-center q-mt-lg'">
      <q-card class="col-4 text-dark">
        <q-card-section>
          <div class="text-h6">Todo App using with VUE and Firebase</div>
        </q-card-section>

        <q-card-section>
          Lorem ipsum dolor sit amet, qui minim labore adipisicing minim sint cillum sint consectetur cupidatat.
        </q-card-section>

        <q-separator dark />

        <q-card-actions>
          <q-btn flat rounded icon="mdi-web" />
          <q-btn flat rounded icon="mdi-github" />
        </q-card-actions>
      </q-card>

      <q-card class="col-4 text-dark">
        <q-card-section>
          <div class="text-h6">My Unique Project</div>
        </q-card-section>

        <q-card-section>
          Lorem ipsum dolor sit amet, qui minim labore adipisicing minim sint cillum sint consectetur cupidatat.
        </q-card-section>

        <q-separator dark />

        <q-card-actions>
          <q-btn flat rounded icon="mdi-web" />
          <q-btn flat rounded icon="mdi-github" />
        </q-card-actions>
      </q-card>

    </div>
  </q-page>
</template>

<script setup>
import { defineComponent } from 'vue';
import { Platform } from 'quasar';

defineComponent({
  name: 'ServicePage'
})
</script>
