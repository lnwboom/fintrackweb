<template>
  <div id="app" class="min-h-screen flex flex-col">
    <Navbar />
    <HeroSection />
    <GuidesSection />
  <FeaturesSection/>
  </div>
</template>

<script>
import Navbar        from './components/Navbar.vue'
import HeroSection   from './components/HeroSection.vue'
import GuidesSection from './components/GuidesSection.vue'
import FeaturesSection from './components/FeaturesSection.vue'

export default {
  name: 'App',
  components: { Navbar, HeroSection, GuidesSection , FeaturesSection }
}
</script>
