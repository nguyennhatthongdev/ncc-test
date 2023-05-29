<template>
  <div class="post">
    <div class="post__item">
      <h3 class="post__item__title">Lorem ipsum dolor sit amet</h3>
      <div class="post__item__image">
        <img src="@/assets/images/post1.png" alt="post1" />
      </div>
      <p class="post__item__content">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed non dui
        sodales, faucibus libero ut, posuere felis. Donec imperdiet suscipit
        accumsan. Aenean consequat condimentum velit ut tempor. Nam porta massa
        in metus bibendum congue. Pellentesque ultrices liquam egestas nunc at
        ullamcorper ultricies. Donec feugiat velit nulla, vel sodales est
        ullamcorper id. Aenean consequat condimentum velit ut tempor. Nam porta
        massa in metus bibendum congue. Pellentesque ultrices vestibulum mattis.
      </p>
    </div>

    <div class="post__item">
      <h3 class="post__item__title">Lorem ipsum dolor sit amet</h3>
      <div class="post__item__image">
        <img src="@/assets/images/post2.png" alt="post2" />
      </div>
      <p class="post__item__content">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed non dui
        sodales, faucibus libero ut, posuere felis. Donec imperdiet suscipit
        accumsan. Aenean consequat condimentum velit ut tempor. Nam porta massa
        in metus bibendum congue. Pellentesque ultrices liquam egestas nunc at
        ullamcorper ultricies. Donec feugiat velit nulla, vel sodales est
        ullamcorper id. Aenean consequat condimentum velit ut tempor. Nam porta
        massa in metus bibendum congue. Pellentesque ultrices vestibulum mattis.
      </p>
    </div>

    <div class="post__item">
      <h3 class="post__item__title">Lorem ipsum dolor sit amet</h3>
      <div class="post__item__image">
        <img src="@/assets/images/post3.png" alt="post3" />
      </div>
      <p class="post__item__content">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed non dui
        sodales, faucibus libero ut, posuere felis. Donec imperdiet suscipit
        accumsan. Aenean consequat condimentum velit ut tempor. Nam porta massa
        in metus bibendum congue. Pellentesque ultrices liquam egestas nunc at
        ullamcorper ultricies. Donec feugiat velit nulla, vel sodales est
        ullamcorper id. Aenean consequat condimentum velit ut tempor. Nam porta
        massa in metus bibendum congue. Pellentesque ultrices vestibulum mattis.
      </p>
    </div>
  </div>
</template>
<script lang="ts" setup></script>
<style lang="scss">
.post {
  display: flex;
  margin: 0 -25px;

  @media (max-width: 1024px) {
    flex-direction: column;
    margin: 0;
  }

  &__item {
    margin: 0 25px;

    @media (max-width: 767px) {
      margin: 0;
    }

    &__title {
      font-size: 24px;
      font-weight: bold;
      margin-bottom: 18px;

      @media (max-width: 767px) {
        font-size: 18px;
      }
    }

    &__image {
      float: left;
      width: 128px;
      height: 128px;
      margin-right: 16px;
      margin-bottom: 6px;

      img {
        object-fit: contain;
        object-position: center center;
        width: 100%;
        height: 100%;
      }
    }

    &__content {
      font-size: 16px;

      @media (max-width: 767px) {
        font-size: 14px;
      }
    }
  }
}
</style>
