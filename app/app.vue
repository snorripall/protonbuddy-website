<script setup>
useHead({
  meta: [
    { name: 'viewport', content: 'width=device-width, initial-scale=1' }
  ],
  link: [
    { rel: 'icon', href: '/favicon.ico' }
  ],
  htmlAttrs: {
    lang: 'en'
  }
})

const title = 'ProtonBuddy - Optimize Your Linux Gaming Experience'
const description = 'Automatically optimize your Linux games for maximum performance. Fine-tune launch parameters, collect performance statistics, and track improvements across kernel updates, driver changes, and game settings.'

useSeoMeta({
  title,
  description,
  ogTitle: title,
  ogDescription: description,
  ogImage: `${useRuntimeConfig().public.siteUrl}/og-image.png`,
  twitterImage: `${useRuntimeConfig().public.siteUrl}/og-image.png`,
  twitterCard: 'summary_large_image'
})
</script>

<template>
  <UApp>
    <UHeader>
      <template #left>
        <NuxtLink to="/" class="text-xl font-bold text-[#35295A] dark:text-white">
          Proton<span class="text-primary">Buddy</span>
        </NuxtLink>
      </template>

       <template #right>
         <UButton
           to="https://github.com/nuxt-ui-templates/starter"
           target="_blank"
           icon="i-simple-icons-github"
           aria-label="GitHub"
           color="neutral"
           variant="ghost"
         />
       </template>
    </UHeader>

    <UMain>
      <NuxtPage />
    </UMain>

    <UFooter>
      <template #left>
        <p class="text-sm text-muted">
          © {{ new Date().getFullYear() }} ProtonBuddy. Built for Linux gamers.
        </p>
      </template>

      <template #right>
        <UButton
          to="https://github.com/protonbuddy"
          target="_blank"
          icon="i-simple-icons-github"
          aria-label="GitHub"
          color="neutral"
          variant="ghost"
        />
      </template>
    </UFooter>
  </UApp>
</template>
