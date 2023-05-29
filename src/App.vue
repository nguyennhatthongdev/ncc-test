<template>
  <div class="sidebar" :class="{ 'menu-active': active }">
    <ul>
      <li>
        <a href="#" class="active">Home</a>
      </li>
      <li>
        <a href="#">Services</a>
      </li>
      <li>
        <a href="#">News</a>
      </li>
      <li>
        <a href="#">Blog</a>
      </li>
      <li>
        <a href="#">Contact</a>
      </li>
    </ul>
  </div>

  <div
    class="main"
    :class="{ 'menu-active': active }"
    @click="active = !active"
  >
    <label class="toggler" :class="{ 'menu-active': active }">
      <span></span>
      <span></span>
      <span></span>
    </label>

    <!--Logo Component-->
    <LogoComponent />

    <router-view />
  </div>
</template>
<script lang="ts" setup>
import { ref } from "vue";
import LogoComponent from "@/components/LogoComponent.vue";

const active = ref(false);
</script>

<style lang="scss">
body {
  margin: 0;
  color: #000000;
}

#app {
  font-family: "Roboto", sans-serif;
  height: 100vh;
  overflow-y: auto;
}

.sidebar {
  width: 150px;
  background-color: #191718;
  height: 100vh;
  flex-shrink: 0;
  position: fixed;
  left: 0;
  transform: translateX(0);
  transition: all 400ms ease-in-out;

  @media (max-width: 767px) {
    transform: translateX(-150px);
    transition: all 400ms ease-in-out;
  }

  &.menu-active {
    transition: all 400ms ease-in-out;

    @media (max-width: 767px) {
      transform: translateX(0);
      transition: all 400ms ease-in-out;
    }
  }

  ul {
    list-style: none;
    padding-left: 0;

    li {
      a {
        display: block;
        text-decoration: none;
        font-size: 16px;
        color: #aaaaaa;
        padding: 14px 16px 11px 16px;
        font-weight: bold;
        transition: all 400ms ease-in-out;

        @media (max-width: 767px) {
          font-size: 14px;
        }

        &.active {
          color: #ffffff;
        }

        &:hover {
          background-color: #5c5c5c;
        }
      }
    }
  }
}

.main {
  margin-left: 150px;
  padding: 20px 129px;

  @media (max-width: 1024px) {
    padding: 20px 50px;
  }

  @media (max-width: 767px) {
    margin-left: 0;
    padding: 20px;
  }
}

.toggler {
  position: fixed;
  top: 0;
  left: 0;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  width: 40px;
  height: 40px;
  background-color: #191718;
  transform: translateX(0);
  transition: transform 400ms ease-in-out;
  cursor: pointer;
  z-index: 200;
  display: none;

  @media (max-width: 767px) {
    display: flex;
  }

  &.menu-active {
    transition: all 400ms ease-in-out;
    @media (max-width: 767px) {
      transform: translateX(150px);
      transition: all 400ms ease-in-out;
    }
  }

  span {
    position: relative;
    display: block;
    width: 50%;
    height: 2px;
    background-color: #ffffff;
    float: left;
    transform-origin: center center;
    transition: transform 250ms ease;
    z-index: 200;

    &:nth-of-type(1) {
      transform: translateY(-5px);
    }

    &:nth-of-type(3) {
      transform: translateY(5px);
    }
  }
}
</style>
