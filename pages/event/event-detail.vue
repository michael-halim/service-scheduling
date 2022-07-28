<template>
  <div class="container">
    <div class="row">
      <div class="col-1">
        <img
          src="https://images.unsplash.com/photo-1658728942259-fca77c5b5231?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1887&q=80"
          alt=""
          width="600"
          height="337"
          style="width: 100px; height: 80px; object-fit: cover"
        />
      </div>
      <div class="col-6">
        <h4>Ibadah Yunus</h4>
        <h6>Hidden</h6>
      </div>
    </div>
    <div class="row my-2">
      <div class="col-1">
        <button
          type="button"
          @click="section = 'overview'"
          class="btn btn-success"
        >
          Overview
        </button>
      </div>
      <div class="col-1">
        <button
          type="button"
          @click="section = 'activity'"
          class="btn btn-info"
        >
          Activity
        </button>
      </div>
      <div class="col-1">
        <button
          type="button"
          @click="section = 'group'"
          class="btn btn-warning"
        >
          Group
        </button>
      </div>
      <div class="col-1">
        <button
          type="button"
          @click="section = 'settings'"
          class="btn btn-secondary"
        >
          Settings
        </button>
      </div>
    </div>

    <div class="row" style="border: 1px solid black">
      <EventOverview v-if="section == 'overview'" />
      <EventActivity v-if="section == 'activity'" />
      <EventGroup v-if="section == 'group'" />
      <EventSettings v-if="section == 'settings'" />
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      section: "overview",
    };
  },
};
</script>
<style scoped>
/* img{
    max-width: 100px;
} */
</style>
