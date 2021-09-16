<template>
  <div>
    <Header />
    <Nuxt />
    <Footer />
  </div>
</template>

<script>
import Header from '/components/Header'
import Footer from '/components/Footer'

export default {
  components: {
    Header,
    Footer
  }
}
</script>


<style lang="scss">
@font-face {
  font-family: Raleway-Bold;
  src: local('RalewayBold'),
url("./../assets/fonts/Raleway-Bold.ttf");
}
@font-face {
  font-family: Raleway-Medium;
  src: local('RalewayMedium'),
  url("./../assets/fonts/Raleway-Medium.ttf");
}

html, body {
  font-size: var(--fontSize);
  padding: 0;
  margin: 0;
  font-family: Raleway-Bold, sans-serif;
}
ul, li {
  list-style-type: none;
}
.container {
  width: 120rem;
  margin: auto;
}
</style>
