<style lang="sass" scoped>
.q-mt-xl
  margin-top: 3em
</style>

<template>
  <q-page padding class="column q-gutter-y-lg q-pb-xl">
    <span class="text-h3 q-mt-xl text-weight-bold">Get in touch</span>

    <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d7851.17813792122!2d123.93518013742012!3d10.294656115468802!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x33a99986352e5ba1%3A0xd07b40adbd217233!2sCanjulao%2C%20Lapu-Lapu%20City%2C%20Cebu!5e0!3m2!1sen!2sph!4v1701941288369!5m2!1sen!2sph" width="100%" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>

    <div class="column q-gutter-y-lg">
      <q-input outlined square placeholder="Name" v-model="form.name"/>
      <q-input outlined square placeholder="Email" v-model="form.email"/>
      <div class="text-message">
        <q-input outlined square placeholder="Message" v-model="form.message" type="textarea"/>
      </div>
      <q-btn square class="self-start" label="Send Message" no-caps padding="15px 30px" color="pink-11"/>
    </div>
  </q-page>
</template>

<script setup>
import { defineComponent, ref } from 'vue';
import { Platform } from 'quasar';

defineComponent({
  name: 'ContactPage'
});

const form = ref({
name: '',
email: '',
message: ''
})
</script>
