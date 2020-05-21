<template>
  <v-container
    fluid
    class="pa-0"
    no-gutters
  >
    <LandingPage />
    <PortfolioProjects />
    <AboutMe />
    <Footer />
  </v-container>
</template>

<script>
import LandingPage from '../components/LandingPage'
import PortfolioProjects from '../components/PortfolioProjects'
import AboutMe from '../components/AboutMe'
import Footer from '../components/Footer'

export default {
  name: 'Home',
  components: {
    LandingPage,
    PortfolioProjects,
    AboutMe,
    Footer
  }
}
</script>
