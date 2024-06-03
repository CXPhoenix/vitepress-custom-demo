<script setup></script>

<template>
  <div :class="$style.IntroLayout">
    <Content />
  </div>
</template>

<style module>
.IntroLayout {
  @apply mx-auto w-full p-6 md:max-w-[80%];
}

.IntroLayout h1 {
  @apply mb-4 border-b-2 border-slate-200 pb-4 text-5xl font-bold;
}

.IntroLayout p {
  @apply text-xl text-red-600;
}
</style>
