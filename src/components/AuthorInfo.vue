<script setup lang="ts">
import WelcomeItem from './WelcomeItem.vue'
import GithubIcon from './icons/IconGithub.vue'
</script>

<template>
  <WelcomeItem>
    <template #icon>
      <img class="avatar" src="https://avatars.githubusercontent.com/u/664177?v=4" />
    </template>
    <template #heading>Eduardo San Martin Morote</template>
    Member of the @vuejs core team, the author of Pinia and Vue Router.
  </WelcomeItem>
  <WelcomeItem>
    <template #icon>
      <GithubIcon />
    </template>
    <template #heading>Eduardo's GitHub</template>
    <a href="https://github.com/posva" target="_blank" rel="noopener">
      @posva
    </a>
  </WelcomeItem>
</template>

<style scoped>
.avatar {
  width: 100%;
  border-radius: 8px;
}
</style>
