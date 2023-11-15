<template>
  <div class="tab">
    <div class="row">
      <div class="col-2">
        <!-- Tab navs -->
        <div
          class="nav flex-column nav-pills text-center"
          id="v-pills-tab"
          role="tablist"
          aria-orientation="vertical"
        >
          <a
            class="nav-link active"
            id="v-pills-link1-tab"
            data-bs-toggle="pill"
            href="#v-pills-link1"
            role="tab"
            aria-controls="v-pills-link1"
            aria-selected="true"
            >Quick</a
          >
          <a
            class="nav-link"
            id="v-pills-link2-tab"
            data-bs-toggle="pill"
            href="#v-pills-link2"
            role="tab"
            aria-controls="v-pills-link2"
            aria-selected="false"
            >Work</a
          >
          <a
            class="nav-link"
            id="v-pills-link3-tab"
            data-bs-toggle="pill"
            href="#v-pills-link3"
            role="tab"
            aria-controls="v-pills-link3"
            aria-selected="false"
            >Home</a
          >
        </div>
        <!-- Tab navs -->
      </div>

      <div class="col-10">
        <!-- Tab content -->
        <div class="tab-content" id="v-pills-tabContent">
          <div
            class="tab-pane fade show active"
            id="v-pills-link1"
            role="tabpanel"
            aria-labelledby="v-pills-link1-tab"
          >
            <Note
              title="Grocery"
              text="Milk, Eggs, Bacon, Mochi"
              category="Quick"
            />
          </div>
          <div
            class="tab-pane fade"
            id="v-pills-link2"
            role="tabpanel"
            aria-labelledby="v-pills-link2-tab"
          >
            Work
          </div>
          <div
            class="tab-pane fade"
            id="v-pills-link3"
            role="tabpanel"
            aria-labelledby="v-pills-link3-tab"
          >
            Home
          </div>
        </div>
        <!-- Tab content -->
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import Note from "./Note.vue";

export default defineComponent({
  name: "VerticalTab",
  components: {
    Note,
  },
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss"></style>
