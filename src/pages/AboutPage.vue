<style lang="sass" scoped>
.picture
  width: 100%
  height: 500px
  object-fit: cover
  -webkit-filter: brightness(110%) contrast(110%) grayscale(100%)
  filter: brightness(110%) contrast(110%) grayscale(100%)

.q-mt-xl
  margin-top: 3em
</style>

<template>
  <q-page padding class="column q-gutter-y-lg q-pb-xl">
    <span class="text-h3 q-mt-xl text-weight-bold">About Me</span>
    <img items-center src="https://picsum.photos/1200/900" class="picture" />

    <div class="column">
      <span class="text-h6 text-weight-bolder">Romelei Galabin</span>
      <span class="text-subtitle1">Web Developer</span>
    </div>

    <q-separator />

    <span class="text-h6 text-weight-light text-grey-7">I'm a straight-to-the-point person and a mother of two, passionate about web development. With a decade of experience, I craft clean, efficient code to bring digital visions to life. Dedicated to creating seamless, user-centric experiences, I thrive in the dynamic realm of web development, ensuring every project exceeds expectations.</span>

    <q-separator />

    <div class="row q-gutter-x-lg">
      <div class="column q-gutter-y-md">
        <div class="row q-gutter-x-md items-center">
          <span class="text-substitle text-weight-bold">Birthday:</span>
          <span class="text-subtitle1 text-weight-light text-grey-7">December 22, 1994</span>
        </div>
        <div class="row q-gutter-x-md items-center">
          <span class="text-substitle text-weight-bold">Age:</span>
          <span class="text-subtitle1 text-weight-light text-grey-7">26</span>
        </div>
        <div class="row q-gutter-x-md items-center">
          <span class="text-substitle text-weight-bold">Address:</span>
          <span class="text-subtitle1 text-weight-light text-grey-7">Canjulao, Lapu-lapu City, Cebu</span>
        </div>
        <div class="row q-gutter-x-md items-center">
          <span class="text-substitle text-weight-bold">Email:</span>
          <span class="text-subtitle1 text-weight-light text-grey-7">romeliegalabin12@gmail.com</span>
        </div>
        <div class="row q-gutter-x-md items-center">
          <span class="text-substitle text-weight-bold">Phone:</span>
          <span class="text-subtitle1 text-weight-light text-grey-7">(+639)909 - 263 - 7489</span>
        </div>
      </div>

      <div class="column q-gutter-y-md">
        <div class="row q-gutter-x-md items-center">
          <span class="text-substitle text-weight-bold">Nationality:</span>
          <span class="text-subtitle1 text-weight-light text-grey-7">Filipino</span>
        </div>
        <div class="row q-gutter-x-md items-center">
          <span class="text-substitle text-weight-bold">Study:</span>
          <span class="text-subtitle1 text-weight-light text-grey-7">Cordova Public College</span>
        </div>
        <div class="row q-gutter-x-md items-center">
          <span class="text-substitle text-weight-bold">Degree:</span>
          <span class="text-subtitle1 text-weight-light text-grey-7">Bachelor</span>
        </div>
        <div class="row q-gutter-x-md items-center">
          <span class="text-substitle text-weight-bold">Hobbies:</span>
          <span class="text-subtitle1 text-weight-light text-grey-7">Volleyball, KDramas and TikTok</span>
        </div>
      </div>
    </div>
  </q-page>
</template>

<script>
export default {
  // name: 'PageName',
}
</script>
