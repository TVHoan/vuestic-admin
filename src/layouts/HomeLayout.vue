<template>
  <div id="page">
    <nav class="fh5co-nav" role="navigation">
      <div class="container-wrap">
        <div class="top-menu">
          <div class="row">
            <div class="col-xs-2">
              <div id="fh5co-logo"><RouterLink to="index.html">Neat</RouterLink></div>
            </div>
            <div class="col-xs-10 text-right menu-1">
              <ul>
                <li class="active"><RouterLink to="/">Home</RouterLink></li>
                <li><RouterLink to="/">Work</RouterLink></li>
                <li class="has-dropdown">
                  <RouterLink to="/">Blog</RouterLink>
                  <ul class="dropdown">
                    <li><RouterLink to="/">Web Design</RouterLink></li>
                    <li><RouterLink to="/">eCommerce</RouterLink></li>
                    <li><RouterLink to="/">Branding</RouterLink></li>
                    <li><RouterLink to="/">API</RouterLink></li>
                  </ul>
                </li>
                <li><RouterLink to="/">About</RouterLink></li>
                <li><RouterLink to="/">Contact</RouterLink></li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </nav>
    <router-view />
  </div>

  <div class="gototop js-top">
    <RouterLink to="#" class="js-gotop"><i class="icon-arrow-up2"></i></RouterLink>
  </div>

  <!-- jQuery -->
  <!--  <script src="js/jquery.min.js"></script>-->
  <!--  &lt;!&ndash; jQuery Easing &ndash;&gt;-->
  <!--  <script src="js/jquery.easing.1.3.js"></script>-->
  <!--  &lt;!&ndash; Bootstrap &ndash;&gt;-->
  <!--  <script src="js/bootstrap.min.js"></script>-->
  <!--  &lt;!&ndash; Waypoints &ndash;&gt;-->
  <!--  <script src="js/jquery.waypoints.min.js"></script>-->
  <!--  &lt;!&ndash; Flexslider &ndash;&gt;-->
  <!--  <script src="js/jquery.flexslider-min.js"></script>-->
  <!--  &lt;!&ndash; Magnific Popup &ndash;&gt;-->
  <!--  <script src="js/jquery.magnific-popup.min.js"></script>-->
  <!--  <script src="js/magnific-popup-options.js"></script>-->
  <!--  &lt;!&ndash; Counters &ndash;&gt;-->
  <!--  <script src="js/jquery.countTo.js"></script>-->
  <!--  &lt;!&ndash; Main &ndash;&gt;-->
  <!--  <script src="js/main.js"></script>-->
</template>
<script setup lang="ts">
  import '../pages/public/static/index.scss'
</script>
