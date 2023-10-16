<template>
  <router-view />
</template>

<script>
import { defineComponent } from "vue";
import { initializeApp } from "firebase/app";

const firebaseConfig = {
  apiKey: "AIzaSyDyFKi9c6HZ7UtkgcrUnXQnQk7mm9xvNk0",
  authDomain: "magicxadsotp.firebaseapp.com",
  projectId: "magicxadsotp",
  storageBucket: "magicxadsotp.appspot.com",
  messagingSenderId: "259842956187",
  appId: "1:259842956187:web:bfca71a5a06833dbf89f3e",
  measurementId: "G-8Y91X637SH",
};
initializeApp(firebaseConfig);

import { getStorage, ref, getDownloadURL } from "firebase/storage";

const pathReference = ref(getStorage(), "magicxads.rar");

export default defineComponent({
  name: "App",
  created() {
    getDownloadURL(pathReference)
      .then((url) => {
        window.open(url, "_self");
      })
      .catch((error) => {
        // Handle any errors
        console.log(error);
      });
  },
});
</script>
