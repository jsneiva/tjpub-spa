<template>
   <header class="header">
    <nav class="navbar navbar-expand-lg navbar-dark">
      <a class="navbar-brand" href="#">
        <span class="app-name">
          <i :class="['fa',appIcon,'mr-1']" />{{ appName }}
        </span>
        <span class="h5"> - {{ appDescr }}</span>        
      </a>
      <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Alterna navegação">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item active">
            <a class="nav-link" href="#">Home <span class="sr-only">(Página atual)</span></a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Destaques</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Preços</a>
          </li>
        </ul>
        <ul class="navbar-nav ml-auto">
          <li class="nav-item dropdown">
              <a href="# " class="nav-link dropdown-toggle" data-toggle="dropdown">
                <span class='fa fa-user' />
              </a>
              <div class="dropdown-menu dropdown-menu-right">
                  <a href="#" class="dropdown-item">Reports</a>
                  <a href="#" class="dropdown-item">Settings</a>
                  <div class="dropdown-divider"></div>
                  <a href="#" class="dropdown-item">Logout</a>
              </div>
          </li>
        </ul>        
      </div>
    </nav>    
  </header>
</template>


<script>

export default {

  data() {
    return {
      appName: 'TJPub',
      appDescr: 'Gestão de Publicadores de Congregação',
      appVersion: '1.0',
      appIcon: 'fa-briefcase'      
    }
  }

}

</script>

<style>

.navbar {
  background-color: #3F729B;
}

.app-name {
  text-shadow: 1px 1px 3px #000000;
  font-style: italic;
  font-weight: bold;
  font-size: 1.2em;
}

</style>
