<template>
  <div class="home-page">
    <!--Overview-->
    <OverviewComponent />

    <!--Post List-->
    <PostListComponent />
  </div>
</template>

<script lang="ts" setup>
import OverviewComponent from "@/components/OverviewComponent.vue";
import PostListComponent from "@/components/PostListComponent.vue";
</script>
<style lang="scss"></style>
