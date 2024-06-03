<script setup>
import { useData } from "vitepress";

import Navbar from "./components/Navbar.vue";
import NotFound from "./layouts/NotFound.vue";

import HomePage from "./layouts/HomePage.vue";
import IntroPage from "./layouts/IntroPage.vue";


// https://vitepress.dev/reference/runtime-api#usedata
const { page, frontmatter } = useData();
</script>

<template>
  <Navbar />
  <NotFound v-if="page.isNotFound" />
  <HomePage v-if="frontmatter.home" />
  <IntroPage v-if="frontmatter.intro" />
</template>
