<template>
  <q-page class="q-pb-xl">
    <q-carousel
      v-model="slide"
      transition-prev="jump-right"
      transition-next="jump-left"
      swipeable
      animated
      control-color="white"
      prev-icon="arrow_left"
      next-icon="arrow_right"
      navigation-icon="radio_button_unchecked"
      navigation
      padding
      arrows
      height="90vh"
      class="bg-purple text-white shadow-1 rounded-borders"
    >
      <q-carousel-slide name="style" class="column no-wrap flex-center">
        <q-icon name="style" size="56px" />
        <div class="q-mt-md text-center">
          {{ lorem }}
        </div>
      </q-carousel-slide>
      <q-carousel-slide name="tv" class="column no-wrap flex-center">
        <q-icon name="live_tv" size="56px" />
        <div class="q-mt-md text-center">
          {{ lorem }}
        </div>
      </q-carousel-slide>
      <q-carousel-slide name="layers" class="column no-wrap flex-center">
        <q-icon name="layers" size="56px" />
        <div class="q-mt-md text-center">
          {{ lorem }}
        </div>
      </q-carousel-slide>
      <q-carousel-slide name="map" class="column no-wrap flex-center">
        <q-icon name="terrain" size="56px" />
        <div class="q-mt-md text-center">
          {{ lorem }}
        </div>
      </q-carousel-slide>
    </q-carousel>

    <div class="q-pa-xl column items-center justify-center">
      <div style="width: 1200px" class="column q-gutter-xl">
        <div class="row">
          <div class="col q-pr-xl">
            <h5 class="text-h5 q-pb-md">부제목 입니다</h5>
            <h3 class="text-h3 q-pb-xl text-bold">제목입니다</h3>
            <spa class="text-body1">
              설명인데요 잘 보이시나요? 설명인데요 잘 보이시나요? 설명인데요 잘
              보이시나요? 설명인데요 잘 보이시나요? 설명인데요 잘 보이시나요?
              설명인데요 잘 보이시나요? 설명인데요 잘 보이시나요? 설명인데요 잘
              보이시나요? 설명인데요 잘 보이시나요? 설명인데요 잘 보이시나요?
              설명인데요 잘 보이시나요? 설명인데요 잘 보이시나요? 설명인데요 잘
              보이시나요? 설명인데요 잘 보이시나요? 설명인데요 잘 보이시나요?
              설명인데요 잘 보이시나요?
            </spa>
          </div>
          <div class="col q-pl-xl">
            <q-img
              class="col-5"
              src="https://cdn.quasar.dev/img/parallax1.jpg"
            />
          </div>
        </div>

        <div class="row">
          <div class="col q-pr-xl">
            <q-img
              class="col-5"
              src="https://cdn.quasar.dev/img/parallax1.jpg"
            />
          </div>
          <div class="col q-pl-xl">
            <h5 class="text-h5 q-pb-md">부제목 입니다</h5>
            <h3 class="text-h3 q-pb-xl text-bold">제목입니다</h3>
            <spa class="text-body1">
              설명인데요 잘 보이시나요? 설명인데요 잘 보이시나요? 설명인데요 잘
              보이시나요? 설명인데요 잘 보이시나요? 설명인데요 잘 보이시나요?
              설명인데요 잘 보이시나요? 설명인데요 잘 보이시나요? 설명인데요 잘
              보이시나요? 설명인데요 잘 보이시나요? 설명인데요 잘 보이시나요?
              설명인데요 잘 보이시나요? 설명인데요 잘 보이시나요? 설명인데요 잘
              보이시나요? 설명인데요 잘 보이시나요? 설명인데요 잘 보이시나요?
              설명인데요 잘 보이시나요?
            </spa>
          </div>
        </div>

        <div class="row q-gutter-xl">
          <div class="col">
            <q-card flat bordered class="my-card">
              <q-card-section>
                <div class="text-h6">Our Changing Planet</div>
              </q-card-section>

              <q-card-section class="q-pt-none">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
                eiusmod tempor incididunt ut labore et dolore magna aliqua.
              </q-card-section>

              <q-separator inset />

              <q-card-section>
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
                eiusmod tempor incididunt ut labore et dolore magna aliqua.
              </q-card-section>
            </q-card>
          </div>
          <div class="col">
            <q-card flat bordered class="my-card">
              <q-card-section>
                <div class="text-h6">Our Changing Planet</div>
              </q-card-section>

              <q-card-section class="q-pt-none">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
                eiusmod tempor incididunt ut labore et dolore magna aliqua.
              </q-card-section>

              <q-separator inset />

              <q-card-section>
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
                eiusmod tempor incididunt ut labore et dolore magna aliqua.
              </q-card-section>
            </q-card>
          </div>
          <div class="col">
            <q-card flat bordered class="my-card">
              <q-card-section>
                <div class="text-h6">Our Changing Planet</div>
              </q-card-section>

              <q-card-section class="q-pt-none">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
                eiusmod tempor incididunt ut labore et dolore magna aliqua.
              </q-card-section>

              <q-separator inset />

              <q-card-section>
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
                eiusmod tempor incididunt ut labore et dolore magna aliqua.
              </q-card-section>
            </q-card>
          </div>
        </div>

        <div class="row">
          <div class="col q-pr-xl">
            <div class="col-5" style="height: 400px">
              <img
                src="https://cdn.pixabay.com/photo/2024/03/19/15/49/woman-8643502_640.png"
                style="height: 100%"
              />
            </div>
          </div>
          <div class="col q-pl-sm">
            <q-form @submit="onSubmit" @reset="onReset" class="q-gutter-md">
              <q-input
                filled
                v-model="name"
                label="Your name *"
                hint="Name and surname"
                lazy-rules
                :rules="[
                  (val) => (val && val.length > 0) || 'Please type something',
                ]"
              />

              <q-input
                filled
                type="number"
                v-model="age"
                label="Your age *"
                lazy-rules
                :rules="[
                  (val) =>
                    (val !== null && val !== '') || 'Please type your age',
                  (val) => (val > 0 && val < 100) || 'Please type a real age',
                ]"
              />

              <q-toggle
                v-model="accept"
                label="I accept the license and terms"
              />

              <div>
                <q-btn label="Submit" type="submit" color="primary" />
                <q-btn
                  label="Reset"
                  type="reset"
                  color="primary"
                  flat
                  class="q-ml-sm"
                />
              </div>
            </q-form>
          </div>
        </div>
      </div>
    </div>

    <q-card-actions
      vertical
      class="justify-around fixed bg-white q-mb-xl"
      style="bottom: 0; right: 0; border: 1px solid"
    >
      <q-btn flat round color="red" icon="favorite" size="xl" />
      <q-btn flat round color="accent" icon="bookmark" size="xl" />
      <q-btn flat round color="primary" icon="share" size="xl" />
    </q-card-actions>
  </q-page>
</template>

<script setup lang="ts">
import { ref } from 'vue';

const slide = ref('style');
const lorem = 'Lorem ipsum dolor sit amet, consectetur adipiscing elit.';

const name = ref(null);
const age = ref(null);
const accept = ref(false);

function onSubmit() {
  if (accept.value !== true) {
    $q.notify({
      color: 'red-5',
      textColor: 'white',
      icon: 'warning',
      message: 'You need to accept the license and terms first',
    });
  } else {
    $q.notify({
      color: 'green-4',
      textColor: 'white',
      icon: 'cloud_done',
      message: 'Submitted',
    });
  }
}

function onReset() {
  name.value = null;
  age.value = null;
  accept.value = false;
}
</script>
