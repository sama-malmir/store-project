<template>
<body>
    <Header/>
    <Nav/>
    <main>
      <BrandCooperation/>
      <NewCollection/>
      <BestSeller/>   
    </main>
    <Footer/>
    
</body>
</template>
<script>
import { RouterLink, RouterView } from 'vue-router'
import Header from './components/Header.vue'
import Nav from './components/Nav.vue'
import BrandCooperation from './components/BrandCooperation.vue'
import NewCollection from './components/NewCollection.vue'
import BestSeller from './components/BestSeller.vue'
import Footer from './components/Footer.vue'
export default{
  name:"App",
  components:{
    Header,
    Nav,
    BrandCooperation,
    NewCollection,
    BestSeller,
    Footer
  }
};
</script>
<style scoped>

</style>
