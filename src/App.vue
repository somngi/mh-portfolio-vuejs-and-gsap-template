<template>
  <div id="app">
    
    <!-- navigation START -->
    <navigation/>
    <!-- navigation END -->

    <!-- view START -->
    <transition name="fade">
      <router-view/>
    </transition>
    <!-- view END -->

    <!-- navigation START -->
    <app-footer/>
    <!-- navigation END -->

  </div>
</template>

<script>
  import Navigation from '@/components/Navigation'
  import AppFooter from '@/components/Footer'
  export default {
    name: 'App',
    data () {
      return {

      }
    },
    components: {
      Navigation,
      AppFooter
    }
  }
</script>

<style lang="scss">
  // mixins - media query
  @mixin maxquery($width, $ratio: false) {
    @if $ratio {
        @media
            only screen and (max-width: $width) and  (min--moz-device-pixel-ratio: $ratio),
            only screen and (max-width: $width) and  (-webkit-min-device-pixel-ratio: $ratio),
            only screen and (max-width: $width) and  (min-device-pixel-ratio: $ratio) {
            @content;
        }
    } @else {
        @media only screen and (max-width: $width) {
            @content;
        }
    }
  }
  // variables
  $black : #363636;
  // common
  html,
  body {
    margin: 0;
    padding: 0;
    overflow-x: hidden !important;
    background-size: cover;
    background-position: center center;
    min-height: 100%;
    min-height: 100vh;
    -webkit-transition: background-color .45s ease-in-out;
    -moz-transition: background-color .45s ease-in-out;
    transition: background-color .45s ease-in-out;
  }
  // styles
  #app {
    font-family: 'Montserrat', sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    font-size: 18px;
    line-height: 28px;
    font-weight: 300;
    color: $black;
    width: 100%;
    max-width: 1360px;
    margin: 0 auto;
    // main navigation
    nav {
      font-family: 'Cardo', serif;
      .router-link-active {
        font-weight: 700;
      }
    }
    // headlines
    h1 {
      font-family: 'Cardo', serif;
      font-size: 36px;
      line-height: 46px;
      font-weight: 400;
    }
    h2 {
      width: 100% !important;
      position: relative;
      display: block;
      float: none;
      font-family: 'Montserrat', sans-serif;
      text-align: center;
      text-transform: uppercase;
      margin-top: 12px;
      padding: 0 !important;
      // divider line
      &.divider-line {
        position: relative;
        font-size: 14px;
        font-weight: 300;
        span {
          position: relative;
          color: #ccc;
          letter-spacing: 2px;
          &:before, &:after {
            content: '';
            border-top: 1px solid #ccc;
            opacity: .45;
            width: 100%;
            width: 100vw;
            position: absolute;
            top: 51%;
          }
          &:before { right: calc( 100% + 1.5rem); }
          &:after { left: calc( 100% + 1.5rem); }
        }
      }
      // divider
      &.divider {
        position: relative;
        font-size: 14px;
        font-weight: 300;
        span {
          position: relative;
          color: #ccc;
          letter-spacing: 2px;
          &:before, &:after {
            content: '';
            border-top: 1px solid #ccc;
            opacity: .45;
            width: 100%;
            width: 100vw;
            position: absolute;
            top: 51%;
          }
          &:before { right: 0; }
          &:after { left: 0; }
        }
      }
    }
    // styles
    .through {
      text-decoration: line-through;
    }
    a {
      text-decoration: none;
      color: $black;
      transition: all .45s cubic-bezier(1.0, 0.5, 0.8, 1.0);
      &:hover {
        // color: #a5d6a7 !important;
      }
    }
    // components
    .fade-component {
      width: 98%;
      width: calc( 100% - 32px );
      padding: 0 16px;
    }
  }
  // page transitions
  .fade-enter-active, .fade-leave-active {
    transition: all 0s cubic-bezier(1.0, 0.5, 0.8, 1.0);
  }
  .fade-enter, .fade-leave-to {
    opacity: 0;
  }
</style>

