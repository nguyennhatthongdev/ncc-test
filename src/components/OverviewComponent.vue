<template>
  <div class="overview">
    <div class="wrap">
      <h4>Lorem ipsum dolor sit asmet?</h4>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed tristique
        consequat placerat. Vestibulum auctor pellentesque sem, eu posuere erat
        hendrerit quis. Maecenas vel consequat turpis. Nam facilisis, ligula in
        mattis sodales, augue justo tristique nulla, sed lacinia ante eros ut
        mi. Morbi vitae diam augue. Aliquam vel mauris a nibh auctor commodo.
        Praesent et nisi eu justo eleifend convallis. Quisque suscipit maximus
        vestibulum. Phasellus congue mollis orci, sit amet luctus augue
        tristique eu. Donec vulputate odio neque, sed semper turpis pellentesque
        a.
      </p>
    </div>
  </div>
</template>
<script lang="ts" setup></script>
<style lang="scss">
.overview {
  text-align: center;
  background-color: #efefef;
  margin-bottom: 40px;
  padding: 38px;

  @media (max-width: 767px) {
    padding: 20px;
    margin-bottom: 20px;
  }

  .wrap {
    width: 100%;
    max-width: 972px;
    margin: 0 auto;
  }

  h4 {
    font-size: 18px;
    margin-bottom: 18px;
  }
}
</style>
