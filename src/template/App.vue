<template>
  <!-- <div>
    <style>
      .container {
          position: absolute;
          width: 100%;
          height: 100%;
      }
      .left {
          float: left;
          width: 200px;
          height: 100%;
          background-color: #ffffff;
      }
      .right {
          float: none;
          width: 100%;
          height: 100%;
          background-color: #ffffff;
      }
    </style>
    <div class="container">
      <div class="left">
        <ul v-for="name in menu" v-bind:key="name">
          <li><a :href="'/' + name">{{name}}</a></li>
        </ul>
      </div>
      <div class="right" v-html="markdown"></div>
    </div>
  </div>-->

  <link rel="stylesheet" href="/assets/adminlte.min.css" />
  <div class="wrapper">
    <!-- Main Sidebar Container -->
    <aside class="main-sidebar sidebar-dark-primary elevation-4">
      <!-- Sidebar -->
      <div class="sidebar">
        <!-- Sidebar user panel (optional) -->
        <div class="user-panel mt-3 pb-3 mb-3 d-flex">
          <div class="image">
            <img src="/assets/logo.png" class="img-circle elevation-2" alt="User Image" />
          </div>
          <div class="info">
            <a href="#" class="d-block">Joseph Xia</a>
          </div>
        </div>
        <!-- Sidebar Menu -->
        <nav class="mt-2">
          <ul
            class="nav nav-pills nav-sidebar flex-column"
            data-widget="treeview"
            role="menu"
            data-accordion="false"
          >
            <!-- Add icons to the links using the .nav-icon class
            with font-awesome or any other icon font library-->
            <li class="nav-item has-treeview menu-open">
              <ul class="nav nav-treeview">
                <li class="nav-item" v-for="name in menu" v-bind:key="name">
                  <a :href="'/' + name" class="nav-link">
                    <i class="far fa-circle nav-icon"></i>
                    <p>{{name}}</p>
                  </a>
                </li>
              </ul>
            </li>
          </ul>
        </nav>
        <!-- /.sidebar-menu -->
      </div>
      <!-- /.sidebar -->
    </aside>

    <!-- Content Wrapper. Contains page content -->
    <div class="content-wrapper">
      <!-- Main content -->
      <div class="content" >
        <div v-html="markdown"></div>
        <!-- <h1>AAACCC</h1> -->
      </div>
      <!-- /.content -->
    </div>
    <aside class="control-sidebar control-sidebar-dark"></aside>
    <footer class="main-footer">
      <strong>
        Copyright &copy; 2020-2080
        <a href="https://adminlte.io">Smart Press</a>.
      </strong>
      All rights reserved.
      <div class="float-right d-none d-sm-inline-block">
        <b>Version</b> 0.0.1
      </div>
    </footer>
  </div>
  <script src="/assets/jquery.min.js"></script>
  <script src="/assets/adminlte.min.js"></script>
</template>
<script>
</script>