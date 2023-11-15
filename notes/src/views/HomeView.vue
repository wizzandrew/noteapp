<template>
  <div class="container">
    <div class="home">
      <HelloWorld msg="Hayyyya notes" />
    </div>

    <div class="tab">
      <VerticalTab />
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import HelloWorld from "@/components/HelloWorld.vue"; // @ is an alias to /src
import VerticalTab from "@/components/VerticalTab.vue";

export default defineComponent({
  name: "HomeView",
  components: {
    HelloWorld,
    VerticalTab,
  },
});
</script>
