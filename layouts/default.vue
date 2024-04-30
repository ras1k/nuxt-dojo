<template>
  <div>
    <header class="shadow-lg bg-white">
      <nav class="container flex mx-auto p-4 justify-between">
        <NuxtLink to="/" class="font-bold">Nuxt Dojo</NuxtLink>
        <ul class="flex gap-4 items-center">
          <li><NuxtLink to="/">Home</NuxtLink></li>
          <li><NuxtLink to="/about">About</NuxtLink></li>
          <li><NuxtLink to="/products">Products</NuxtLink></li>
        </ul>
      </nav>
    </header>

    <div class="container px-[5%] py-[2%]">
      <slot />
    </div>
  </div>
</template>

<style scoped>
  .router-link-exact-active {
    color: rgb(77, 165, 42);
  }
</style>
