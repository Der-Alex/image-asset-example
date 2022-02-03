<template>
  <div>
    <!-- Not working when running npm 'run dev' -->
    <picture>
      <source srcset="~/assets/img/test-img.jpg" media="(max-width: 2000px)">
      <img src="~/assets/img/test-img.jpg" alt="test image">
    </picture>

    <!-- Not working when running npm 'run dev' -->
    <picture>
      <source srcset="~assets/img/test-img.jpg" media="(max-width: 2000px)">
      <img src="~assets/img/test-img.jpg" alt="test image">
    </picture>

    <!-- Works with 'npm run dev' and 'npm run start' -->
    <picture>
      <source srcset="assets/img/test-img.jpg" media="(max-width: 2000px)">
      <img src="assets/img/test-img.jpg" alt="test image">
    </picture>

    <!-- Works with 'npm run dev' and 'npm run start' -->
    <picture>
      <source srcset="/assets/img/test-img.jpg" media="(max-width: 2000px)">
      <img src="/assets/img/test-img.jpg" alt="test image">
    </picture>
  </div>
</template>
