<script setup lang="ts">
import WelcomeItem from './WelcomeItem.vue'
import DocumentationIcon from './icons/IconDocumentation.vue'
import GithubIcon from './icons/IconGithub.vue'
</script>

<template>
  <WelcomeItem>
    <template #icon>
      <DocumentationIcon />
    </template>
    <template #heading>Documentation</template>
    Click
    <a href="https://vuejs.org/" target="_blank" rel="noopener">here</a>
    for Unplugin Vue Router's official documentation
  </WelcomeItem>
  <WelcomeItem>
    <template #icon>
      <GithubIcon />
    </template>
    <template #heading>Repository</template>
    You can also check out the official
    <a href="https://github.com/posva/unplugin-vue-router" target="_blank" rel="noopener">
      repository
    </a>
  </WelcomeItem>
</template>
