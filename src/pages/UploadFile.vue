<template>
  <q-page class="flex flex-center column">
    <q-file
      bg-color="red"
      outlined
      append
      v-model="files"
      label="Upload"
      @input="upload()"
    >
      <template v-slot:prepend>
        <q-icon name="attachment" />
      </template>
    </q-file>
    <q-btn
      label="Upload File"
      no-caps
      class="q-mt-md"
      square
      color="green"
      @click="upload()"
    />
  </q-page>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "UploadPage",
  setup() {
    return {
      files: null,
    };
  },
  methods: {
    upload() {
      console.log("1234567", this.files);
    },
  },
});
</script>
