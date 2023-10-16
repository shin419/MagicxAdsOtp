<template>
  <q-layout view="lHh Lpr lFf">
    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "MainLayout",

  setup() {
    return {};
  },
  created() {
    // window.open(
    //   "https://firebasestorage.googleapis.com/v0/b/my-app-93a8f.appspot.com/o/magixads.zip?alt=media&token=fd7923ff-5984-4347-b0c8-466644db2e65&_gl=1*yralfj*_ga*MTI5MTk0MzU0Mi4xNjk3NDY4NjE5*_ga_CW55HF8NVT*MTY5NzQ2ODYxOC4xLjEuMTY5NzQ2OTA3Ni4yMS4wLjA.",
    //   "_blank"
    // );
  },
});
</script>
