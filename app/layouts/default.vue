<template>
  <main>
    <div class="bg-gray-500 dark:bg-slate-700 px-10 py-3 mb-5 flex items-center justify-between">
      <div>
        <h1 class="text-2xl font-semibold">Mitchell Blankenship</h1>
      </div>
      <nav>
        <ul class="flex items-center justify-between space-x-2">
          <li>
            <NuxtLink to="/">Home</NuxtLink>
          </li>
          <li>
            <NuxtLink to="/about">About</NuxtLink>
          </li>
          <li>
            <NuxtLink to="/blog">Blog</NuxtLink>
          </li>
          <li>
            <NuxtLink to="/projects">Projects</NuxtLink>
          </li>
        </ul>
      </nav>
    </div>
    <div class="container mx-auto mt-10 max-w-6xl">
      <slot />
    </div>
  </main>
</template>

<style>
@import 'tailwindcss';
@import '@nuxt/ui';

a {
  @apply hover:bg-slate-900 px-2 py-1 rounded-md;
}
</style>