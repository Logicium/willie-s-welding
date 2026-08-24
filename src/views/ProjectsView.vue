<script setup lang="ts">
import { siteConfig } from '../config/site.config'
import HeroSection from '@apotome/archetype-shared/components/sections/HeroSection.vue'
import ProjectsSection from '../components/sections/ProjectsSection.vue'
import GallerySection from '@apotome/archetype-shared/components/sections/GallerySection.vue'
</script>

<template>
  <HeroSection
    subpage
    :eyebrow="siteConfig.sections.projectsPage.eyebrow"
    :title="siteConfig.sections.projectsPage.title"
    :subtitle="siteConfig.sections.projectsPage.subtitle"
    :image="siteConfig.photos.about.src"
  />

  <ProjectsSection
    :intro="siteConfig.projects.intro"
    :items="siteConfig.projects.items"
  />

  <GallerySection
    :eyebrow="siteConfig.sections.projectsPage.galleryEyebrow"
    :title="siteConfig.sections.projectsPage.galleryTitle"
    :photos="siteConfig.photos.gallery"
  />
</template>
