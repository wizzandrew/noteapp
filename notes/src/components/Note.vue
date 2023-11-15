<template>
  <div class="note">
    <div class="col-sm-4">
      <div class="card">
        <div class="card-body">
          <h5 class="card-title">{{ title }}</h5>
          <p class="card-text">
            {{ text }}
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import type { PropType } from "vue";
import type { Category } from "@/models/models";

export default defineComponent({
  name: "Note",
  props: {
    title: String,
    text: String,
    category: Object as PropType<Category>,
  },
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss"></style>
