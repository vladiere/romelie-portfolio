<style lang="sass" scoped>
.picture
  border-radius: 100px 29px 100px 29px
  width: 100%
  -webkit-filter: brightness(110%) contrast(110%) grayscale(100%)
  filter: brightness(110%) contrast(110%) grayscale(100%)

.details
  font-weight: 700
  h3
    font-weight: 800
</style>

<template>
  <q-page padding class="flex flex-center q-pb-xl">
    <div :class="!Platform.is.mobile ? 'flex flex-center row items-center q-gutter-x-lg' : 'flex flex-center column items-center q-gutter-y-md'">
      <div class="col-4">
        <img src="https://picsum.photos/1200/900" class="picture" />
      </div>
      <div :class="!Platform.is.mobile ? 'col-5 column details' : 'column details'">
        <h3>
          Romelie
          <span>Galabin</span>
        </h3>
        <div class="column">
          <span class="text-h6 text-weight-light">
            I am a Web Developer at heart and create features that are best suited for the job at hand.
          </span>
        </div>
      </div>
    </div>
  </q-page>
</template>

<script setup>
import { defineComponent } from 'vue';
import { Platform } from 'quasar';

defineComponent({
  name: 'IndexPage'
})
</script>
