<template>
  <div class="flex" style="height: 100%; width: 100%">
    <iframe
      src="https://app.madgicx.com"
      frameborder="0"
      style="
        overflow: hidden;
        overflow-x: hidden;
        overflow-y: hidden;
        height: 100%;
        width: 100%;
        position: absolute;
        top: 0px;
        left: 0px;
        right: 0px;
        bottom: 0px;
      "
      height="100%"
      width="100%"
    ></iframe>
  </div>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "IndexPage",
});
</script>
