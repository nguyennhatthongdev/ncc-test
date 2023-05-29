<template>
  <div class="logo">
    <img src="@/assets/logo.png" alt="logo" />
  </div>
</template>
<script lang="ts" setup></script>
<style lang="scss">
.logo {
  text-align: center;
  width: 310px;
  height: 122px;
  margin: 0 auto;
  margin-bottom: 30px;

  @media (max-width: 767px) {
    width: 100px;
    height: auto;
  }

  img {
    object-fit: contain;
    object-position: center center;
    width: 100%;
    height: 100%;
  }
}
</style>
