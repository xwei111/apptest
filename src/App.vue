<template>
  <div id="app">
  	<Header />
  	<Main />
  	<Footer />
    <!-- <img src="./assets/logo.png"> -->
    <!-- <router-view/> -->
  </div>
</template>

<script>
import Header from 'components/header/Header'
import Main from 'components/main/Main'
import Footer from 'components/footer/Footer'
export default {
  name: 'App',
  components:{
  	Header,
  	Main,
  	Footer
  }
}
</script>

