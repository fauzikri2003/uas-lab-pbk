<template>
  <q-layout view="lHr lpR lfr" class="background-image">
    <q-header class="bg-black text-white" height-hint="98">
      <q-toolbar>
        <div class="q-toolbar-title-wrapper">
          <q-toolbar-title class="uas-title">Uas Lab PBK</q-toolbar-title>
          <span class="fauzikri-ghifari">Fauzikri Ghifari</span>
        </div>
        <q-tabs align="left">
          <q-route-tab to="/" label="Weather" />
        </q-tabs>
      </q-toolbar>
    </q-header>
    <q-page-container>
      <router-view />
    </q-page-container>
    <q-footer class="bg-black text-white" height-hint="98">
      <q-toolbar class="justify-center">
        <q-toolbar-title class="footer-title">
          Copyright © Fauzikri Ghifari. All rights reserved.
        </q-toolbar-title>
      </q-toolbar>
    </q-footer>
  </q-layout>
</template>

<script setup>
</script>

<style>
.background-image {
  background-image: url('src/assets/image2.png'); /* Ensure this path is correct */
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  min-height: 100vh; /* Ensure the background covers the entire viewport */
}

.q-toolbar {
  padding: 0 75px !important;
}

.q-toolbar__title:first-child {
  padding-left: 32px !important;
}

.q-tab {
  padding: 0 20px !important;
  min-height: 75px !important;
}

.q-toolbar-title-wrapper {
  display: flex;
  align-items: center;
}

.uas-title {
  margin-right: 10px;
}

.fauzikri-ghifari {
  font-size: 16px;
  color: #f7f6f6;
}

.justify-center {
  justify-content: center !important;
}

.footer-title {
  text-align: center;
  width: 100%;
}
</style>
