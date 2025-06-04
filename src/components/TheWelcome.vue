<script setup lang="ts">
import WelcomeItem from './WelcomeItem.vue'
import DocumentationIcon from './icons/IconDocumentation.vue'
import ToolingIcon from './icons/IconTooling.vue'
import EcosystemIcon from './icons/IconEcosystem.vue'
import CommunityIcon from './icons/IconCommunity.vue'
import SupportIcon from './icons/IconSupport.vue'

const openReadmeInEditor = () => fetch('/__open-in-editor?file=README.md')
</script>

<template>
  <WelcomeItem>
    <template #icon>
      <a class="img" href="https://github.com/AntGir" target="_blank" rel="noopener">
        <img
          alt="github-logo"
          class="logo"
          src="../assets/github-mark-white.svg"
          width="30"
          height="30"
        />
      </a>
    </template>
    <template #heading
      ><a href="https://github.com/AntGir" target="_blank" rel="noopener">My git-hub</a></template
    >
    Hi there! Feel free to explore my projects and connect with me!
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <a
        class="img"
        href="https://www.linkedin.com/in/antoine-gires-23571a122/"
        target="_blank"
        rel="noopener"
      >
        <img
          alt="github-logo"
          class="logo"
          src="../assets/linkedin-logo.svg"
          width="30"
          height="30"
        />
      </a>
    </template>
    <template #heading
      ><a href="https://www.linkedin.com/in/antoine-gires-23571a122/" target="_blank" rel="noopener"
        >LinkedIn</a
      ></template
    >
    Actuellement a la recherche pour une alternance en Concepteur Développeur 3D VR
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <a
        class="img"
        href="https://drive.google.com/drive/folders/1HdrRmcGvsnev47FSvI6nrmfYHTSAR2QD?usp=sharing"
        target="_blank"
        rel="noopener"
      >
        <img
          alt="github-logo"
          class="logo"
          src="../assets/Google-Drive-icon-logo.svg"
          width="30"
          height="30"
        />
      </a>
    </template>
    <template #heading
      ><a
        href="https://drive.google.com/drive/folders/1HdrRmcGvsnev47FSvI6nrmfYHTSAR2QD?usp=sharing"
        target="_blank"
        rel="noopener"
        >Informations Formation Simplon</a
      >
    </template>
    Dans ce drive vous allez retrouver la planning de la formation ainsi que la plaquette de
    celle-ci.
  </WelcomeItem>
</template>
<style scoped>
.img {
  display: flex;
  align-items: center;
}
</style>
