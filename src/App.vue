<template>

  <div id="wrapper">
    <SidebarVue />
    <div id="content-wrapper" class="d-flex flex-column">
      <!-- Main Content -->
      <div id="content">
        <NavBarVue />
        <PageContent />
      </div>
        <PageFooter />
    </div>
  </div>
  <a class="scroll-to-top rounded" href="#page-top">
     <i class="fas fa-angle-up"></i>
  </a>
  <LogoutModal />

</template>

<script>
import NavBarVue from './components/NavBar/NavBarVue.vue'
import SidebarVue from "./components/SideBar/SidebarVue.vue"
import PageContent from "./components/PageContent.vue"
import PageFooter from "./components/PageFooter.vue"
import LogoutModal from "./components/LogoutModal.vue"

export default {
  name: 'App',
  components: {
    NavBarVue,
    SidebarVue,
    PageContent,
    PageFooter,
    
    LogoutModal

  }
}
</script>

<style>
/* #app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
} */
</style>
