<template>
  <div class="container-fluid mx-0 px-0">
    <Navbar />
    <Hero />
    <CourseTypes />
    <TenYears />
    <WhyLearna />
    <Partners />
    <Footer />
  </div>
</template>

<script>
import Navbar from '~/components/Navbar.vue'
import Hero from '~/components/Hero.vue'
import CourseTypes from '~/components/CourseTypes.vue'
import TenYears from '~/components/TenYears.vue'
import WhyLearna from '~/components/WhyLearna.vue'
import Partners from '~/components/Partners.vue'
import Footer from '~/components/Footer.vue'

export default {
  components: {
    Navbar,
    Hero,
    CourseTypes,
    TenYears,
    WhyLearna,
    Partners,
    Footer
  }
}
</script>

<style>

</style>
