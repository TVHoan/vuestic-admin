<template>
  <div id="page">
    <nav class="fh5co-nav" role="navigation">
      <div class="container-wrap">
        <div class="top-menu">
          <div class="row">
            <div class="col-xs-2">
              <div id="fh5co-logo"><RouterLink to="/">Neat</RouterLink></div>
            </div>
            <div class="col-xs-10 text-right menu-1">
              <ul>
                <li class="active"><RouterLink to="/">Home</RouterLink></li>
                <li><RouterLink to="/">Work</RouterLink></li>
                <li class="has-dropdown">
                  <RouterLink to="#" @mousemove="isblog = true" @mouseleave="isblog = false">Blog</RouterLink>
                  <ul v-show="isblog" class="dropdown" @mousemove="isblog = true" @mouseleave="isblog = false">
                    <li><RouterLink to="/">Dev</RouterLink></li>
                    <li><RouterLink to="/">My Life</RouterLink></li>
                    <li><RouterLink to="/">Tip</RouterLink></li>
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
    <RouterLink to="/" class="js-gotop"><i class="icon-arrow-up2"></i></RouterLink>
  </div>
</template>
<script lang="ts">
  import '../pages/public/static/index.scss'
  // import  '../pages/public/static/js/jquery.min'
  // import '../pages/public/static/js/jquery.easing.1.3'
  // import '../pages/public/static/js/bootstrap.min'
  // import '../pages/public/static/js/jquery.waypoints.min'
  // import '../pages/public/static/js/jquery.flexslider-min'
  // import '../pages/public/static/js/jquery.magnific-popup.min'
  // import '../pages/public/static/js/magnific-popup-options'
  // import '../pages/public/static/js/jquery.countTo'
  // import '../pages/public/static/js/main'

  export default {
    data() {
      return {
        isblog: false,
      }
    },
  }
</script>
