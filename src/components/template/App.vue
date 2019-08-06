<template>
  <div id="app">
    <SideBar />    
    <div id="content">
      <Header />      
      <Main />
      <Footer />    
    </div>
  </div>
</template>

<script>

import Header  from './Header'
import Footer  from './Footer'
import SideBar from './SideBar'
import Main    from './Main'

export default {

  components: {Header, Footer, SideBar, Main}

}
</script>

<style>


#app {
  display: flex;
  flex-flow: row nowrap;
  height: var(--app-height);
}

#content {
  flex-grow: 1;
  display: flex;
  flex-flow: column nowrap;
}


</style>
