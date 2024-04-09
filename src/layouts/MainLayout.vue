<template>
  <q-layout view="lHh Lpr lFf">
    <q-header
      elevated
      @mouseenter="activateNav"
      @mouseleave="deactivateNav"
      class="bg-white text-black fixed"
      style="height: 88px; z-index: 1"
    >
      <q-toolbar class="row justify-between">
        <div class="row">
          <div
            class="row items-center justify-center q-mr-lg"
            style="height: 88px; width: 130px"
          >
            <q-img src="../assets/logo.png" spinner-color="white" />
          </div>
          <ul
            class="row q-ma-none q-pa-none"
            style="height: 88px; list-style: none"
          >
            <li
              class="full-height"
              style="width: 120px"
              v-for="(item, index) in menuItems"
              :key="index"
            >
              <div class="full-height row items-center justify-center q-px-md">
                <span class="text-h6">{{ item.title }}</span>
              </div>
              <ul v-if="navActive" class="q-pt-sm" style="color: black">
                <li
                  class="q-px-none q-py-sm text-center"
                  v-for="(subItem, subIndex) in item.subMenu"
                  :key="`subItem-${subIndex}`"
                >
                  <a :href="subItem.link">{{ subItem.name }}</a>
                </li>
              </ul>
            </li>
          </ul>
        </div>

        <q-btn
          flat
          dense
          round
          icon="menu"
          aria-label="Menu"
          @click="toggleLeftDrawer"
        />
      </q-toolbar>
      <div
        class="full-width bg-white"
        style="height: 15rem"
        v-if="navActive"
      ></div>
    </q-header>

    <q-drawer v-model="rightDrawerOpen" bordered side="right"> </q-drawer>

    <q-page-container>
      <router-view />
    </q-page-container>

    <div class="text-h6 bg-black text-white full-width">Footer</div>
  </q-layout>
</template>

<script setup lang="ts">
import { ref } from 'vue';

const navActive = ref(false);

const rightDrawerOpen = ref(false);

function toggleLeftDrawer() {
  rightDrawerOpen.value = !rightDrawerOpen.value;
}

const menuItems = ref([
  {
    title: '병원소개',
    subMenu: [
      { name: '리팅의원소개', link: '#' },
      { name: '대표원장 스토리', link: '#' },
      { name: '의료진 소개', link: '#' },
      { name: '진료안내/오시는길', link: '#' },
      { name: '병원둘러보기', link: '#' },
    ],
  },
  {
    title: '실리프팅',
    subMenu: [
      { name: '리팅 실 리프팅', link: '#' },
      { name: '슬리핑실', link: '#' },
    ],
  },
  {
    title: '줄기세포',
    subMenu: [
      { name: '셀프팅', link: '#' },
      { name: '셀스킨주사', link: '#' },
    ],
  },
  {
    title: '쁘띠리프팅',
    subMenu: [
      { name: '레이저 리프팅', link: '#' },
      { name: '리팅부스터', link: '#' },
    ],
  },
  {
    title: '필러보톡스',
    subMenu: [{ name: '필러보톡스', link: '#' }],
  },
  {
    title: '지방흡입',
    subMenu: [{ name: '초음파 지방흡입', link: '#' }],
  },
  {
    title: '커뮤니티',
    subMenu: [
      { name: '공지사항', link: '#' },
      { name: '리팅뉴스', link: '#' },
      { name: '전후사진', link: '#' },
      { name: '자필후기', link: '#' },
    ],
  },
  {
    title: '상담예약',
    subMenu: [
      { name: '온라인상담', link: '#' },
      { name: '비용상담', link: '#' },
      { name: '이벤트', link: '#' },
    ],
  },
]);

const activateNav = () => {
  navActive.value = true;
};

const deactivateNav = () => {
  navActive.value = false;
};
</script>
