<template>
  <div id="app">
    <Header />
    <router-view />
    <MainContent />
    <Footer />
  </div>
</template>

<style lang="scss">
</style>

<script>
import Header from '@/components/pages/header/Header'
import Footer from '@/components/pages/footer/Footer'
import MainContent from '@/components/pages/main-content/MainContent'
export default {
  components: {
    Header,
    Footer,
    MainContent
  }
}
</script>
