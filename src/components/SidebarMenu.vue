<template>
  <ul class="sidebar-menu">
    <li class="header">Tools</li>
    <router-link tag="li" class="pageLink" to="/vmchooser">
      <a>
        <i class="fa fa-desktop"></i>
        <span class="page">VM T-Shirt Sizes Finder</span>
      </a>
    </router-link>
    <router-link tag="li" class="pageLink" to="/diskchooser">
      <a>
        <i class="fa fa-database"></i>
        <span class="page">Data Disk Configuration</span>
      </a>
    </router-link>
    <router-link tag="li" class="pageLink" to="/backupchooser">
      <a>
        <i class="fa fa-copy"></i>
        <span class="page">Backup Sizing</span>
      </a>
    </router-link>
    <router-link tag="li" class="pageLink" to="/bulkuploader">
      <a>
        <i class="fa fa-sliders-h"></i>
        <span class="page">Bulk Uploader</span>
      </a>
    </router-link>
    <router-link tag="li" class="pageLink" to="/vmoptimizer">
      <a>
        <i class="fa fa-balance-scale"></i>
        <span class="page">VM Optimizer</span>
      </a>
    </router-link>
    <router-link tag="li" class="pageLink" to="/azureredhatopenshift">
      <a>
        <i class="fa fa-coins"></i>
        <span class="page">Azure Red Hat OpenShift</span>
      </a>
    </router-link>
    <router-link tag="li" class="pageLink" to="/azurevmwareservice">
      <a>
        <i class="fa fa-ruler-combined"></i>
        <span class="page">Azure VMware Sizer</span>
      </a>
    </router-link>
    <li class="header">Information</li>
    <li class="pageLink">
      <a href="https://docs.vmchooser.com/" target="_blank">
        <i class="fa fa-book"></i>
        <span class="page">Documentation</span>
      </a>
    </li>
    <li class="pageLink">
      <a href="https://preview.vmchooser.com/" target="_blank">
        <i class="fa fa-book"></i>
        <span class="page">Preview</span>
      </a>
    </li>
    <li class="pageLink">
      <a href="https://github.com/vmchooser" target="_blank">
        <i class="fab fa-github"></i>
        <span class="page">GitHub Repositories</span>
      </a>
    </li>
    <li class="pageLink">
      <a href="https://www.wolkytolk.com/" target="_blank">
        <i class="fas fa-cloud"></i>
        <span class="page">Wolky Tolk</span>
      </a>
    </li>
  </ul>
</template>

<script>
  export default {
    name: 'SidebarMenu'
  }
</script>

<style>
  /* override default */
  .sidebar-menu > li > a {
    padding: 12px 15px 12px 15px;
  }

  .sidebar-menu li.active > a > .fa-angle-left, .sidebar-menu li.active > a > .pull-right-container > .fa-angle-left {
    animation-name: rotate;
    animation-duration: .2s;
    animation-fill-mode: forwards;
  }

  @keyframes rotate {
    0% {
      transform: rotate(0deg);
    }

    100% {
      transform: rotate(-90deg);
    }
  }
</style>
