<template>
  <q-layout view="lHh Lpr lFf">
    <q-header class="bg-white text-dark" height-hint="98">
      <q-toolbar class="q-py-md q-px-lg">
        <q-btn flat no-caps no-wrap class="q-ml-xs" to="/" v-if="$q.screen.gt.xs">
          <q-icon name="dashboard" color="primary" size="28px" />
          <q-toolbar-title shrink class="text-weight-bold row items-center no-wrap">
            CMS<span class="text-primary">PRO</span>
          </q-toolbar-title>
        </q-btn>
        <q-btn flat no-caps no-wrap class="q-ml-xs" to="/" v-else>
          <q-icon name="dashboard" color="primary" size="28px" />
        </q-btn>

        <q-space />

        <div class="q-gutter-sm row items-center no-wrap" v-if="$q.screen.gt.sm">
          <q-btn to="/" flat label="Home" class="text-weight-bold" />
          <q-btn to="#features" flat label="Features" class="text-weight-bold" />
          <q-btn to="#pricing" flat label="Pricing" class="text-weight-bold" />
        </div>

        <q-space />

        <div class="q-gutter-sm row items-center no-wrap">
          <q-btn flat label="Log In" class="text-weight-bold" no-caps />
          <q-btn color="primary" label="Sign Up" unelevated class="q-px-md" no-caps />
        </div>
      </q-toolbar>
    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>

    <q-footer class="bg-secondary text-white q-pa-xl">
      <div class="row justify-between items-center">
        <div class="col-12 col-md-auto text-center q-mb-md-none">
          <div class="text-h6 text-weight-bold">CMS<span class="text-red">PRO</span></div>
          <div class="text-grey-5 text-caption">Manage your customers with ease.</div>
        </div>
        <div class="col-12 col-md-auto text-center">
          <q-btn flat round icon="adb" size="sm" class="opacity-50" />
          <q-btn flat round icon="wifi" size="sm" class="opacity-50" />
          <q-btn flat round icon="bluetooth" size="sm" class="opacity-50" />
        </div>
        <div class="col-12 col-md-auto text-center text-grey-5 text-caption q-mt-md-none">
          &copy; {{ new Date().getFullYear() }} CMS Pro. All rights reserved.
        </div>
      </div>
    </q-footer>
  </q-layout>
</template>

<script setup>
// Modern landing page layout
</script>
