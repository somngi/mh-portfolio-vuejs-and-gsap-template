<template>
  <div>

    <div class="cookies" v-if="cookies == false">This website use cookies to ensure that I give you the best experience on my website.<br><span class="green"><span class="link" @click="allowCookies()">OK, CLOSE</span> this message or see <router-link :to="'/imprint'" exact>imprint</router-link> for more infos.</span></div>

    <nav class="navigation" v-if="$route.name !== 'Home'">
      
      <!-- navigation:logo START -->
      <div class="logo">
        <router-link :to="'/'" exact>
          <img width="380" height="199" class="logo-txt" src="/static/logo.png" alt="MH - Web Designer & Developer - Logo" />
          <div class="logo-bg-holder">
            <div class="logo-bg oval-big"></div>
            <div class="logo-bg oval-small"></div>
            <div class="logo-bg circle"></div>
          </div>
        </router-link>
      </div>
      <!-- navigation:logo END -->

      <!-- navigation:nav:main START -->
      <div class="main-navigation">
        <ul>
          <li>
            <router-link :to="'/author'" exact>
              author<span>.</span>
            </router-link>
          </li>
          <li>
            <router-link :to="'/works'" exact>
              works<span>.</span>
            </router-link>
          </li>
          <li>
            <router-link :to="'/contact'" exact>
              contact<span>.</span>
            </router-link>
          </li>
        </ul>
      </div>
      <!-- navigation:nav:main START -->

    </nav>
    
  </div>
</template>

<script>
  
  // gsap
  import { TweenMax } from "gsap"
  // scrollmagic
  import ScrollMagic from "scrollmagic"
  // jquery
  import $ from "jquery";

  export default {
    name: 'Navigation',
    data () {
      return {
        cookies: false
      }
    },
    created () {
      this.animateNavigation()
    },
    updated () {
      this.animateNavigation()
    },
    mounted () {
      this.animateNavigation()
    },
    watch: {
      '$route' (to, from) {
        this.animateNavigation()
      }
    },
    methods: {
      allowCookies: function () {
        this.cookies = true;
      },
      animateNavigation: function() {
        // comon -> sidebar -> navigation timeline
        let controller = new ScrollMagic.Controller(),
            timeline = new TimelineMax(); 

        $('.navigation .oval-big').removeClass('rotating-fast');
        $('.navigation .oval-small').removeClass('rotating-slow');

        timeline.set($('.navigation .circle'), { scale:0, z: 0.01 } );
        timeline.set($('.navigation .oval-small'), { autoAlpha: 0, scale:0, z: 0.01 } );
        timeline.set($('.navigation .oval-big'), { autoAlpha: 0, scale:0, z: 0.01 } );
        timeline.set($('.navigation .logo-txt'), { autoAlpha: 0, z: 0.01 } );
        timeline.set($('.navigation .main-navigation'), { autoAlpha: 0, z: 0.01 } );
        timeline.set($('.cookies'), { autoAlpha: 0 } );

        timeline.fromTo( $('.navigation .circle'), 3, { scale: 0, transformOrigin:"50% 50%" }, { force3D:true, scale: 1, transformOrigin:"50% 50%", ease: Back.easeOut.config(2.25) } )
        timeline.fromTo( $('.navigation .oval-small'), 2.5, { autoAlpha: 0, scale: 0, transformOrigin:"50% 50%" }, { force3D:true, autoAlpha: 0.45, scale: 1, transformOrigin:"50% 50%", ease: Back.easeOut.config(2.25) }, '-=2.25' )
        timeline.fromTo( $('.navigation .oval-big'), 2.5, { autoAlpha: 0, scale: 0, transformOrigin:"50% 50%" }, { force3D:true, autoAlpha: 0.25,scale: 1, transformOrigin:"50% 50%", ease: Back.easeOut.config(2.25) }, '-=2.25' ) 
        timeline.fromTo( $('.navigation .logo-txt'), 2.5, { autoAlpha: 0, x: -80 }, { autoAlpha: 1, x: 0, ease: Expo.easeOut }, '-=2.65' )
        timeline.fromTo( $('.navigation .main-navigation'), 2.5, { autoAlpha: 0, x: -80 }, { autoAlpha: 1, x: 0, ease: Expo.easeOut }, '-=2.5' )
        timeline.fromTo( $('.fade-component'), 2.5, { autoAlpha: 0 }, { autoAlpha: 1, ease: Expo.easeOut }, '-=2.5' )
        timeline.fromTo( $('.cookies'), 2.5, { autoAlpha: 0 }, { autoAlpha: 1, ease: Expo.easeOut }, '-=0.25' )
        // timeline.to( $('.navigation .oval-big'), 0.35, { className:"+=rotating-fast", ease: Expo.easeOut }, '+=2.35' ) 
        // timeline.to( $('.navigation .oval-small'), 0.35, { className:"+=rotating-slow", ease: Expo.easeOut }, '+=2.35' )
        setTimeout(function() {
          $('.navigation .oval-big').addClass('rotating-fast');
          $('.navigation .oval-small').addClass('rotating-slow'); 
        }, 3650)
        
      }

    }
  }
</script>

<style lang="scss" scoped>
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
  .cookies {
    position: fixed;
    display: block;
    width: 100%;
    width: calc( 100% - 64px);
    // max-width: 1360px;
    height: auto;
    bottom: 16px;
    left: 50%;
    transform: translate(-50%);
    text-align: center;
    font-size: 12px;
    line-height: 22px;
    z-index: 1000;
    background-color: #a5d6a7;
    padding: 16px;
    span {
      &.green {
        font-weight: 700;
      }
      &.link {
        cursor: pointer;
        text-transform: uppercase;
      }
    }
    a {
      cursor: pointer;
      text-transform: uppercase;
    }
  }
  nav {
    &.navigation {
      position: relative;
      display: block;
      width: 98%;
      width: calc( 100% - 32px );
      height: auto;
      padding: 84px 16px;
      // logo
      .logo {
        position: relative;
        display: block;
        max-width: 120px;
        height: auto;
        float: left;
        @include maxquery( 640px ) {
          width: 260px;
          height: auto;
        }
        .logo-txt {
          position: relative;
          z-index: 4;
          width: 60px;
          height: auto;
          margin: 0;
          opacity: 0;
          visibility: hidden;
        }
        .logo-bg-holder {
          position: absolute;
          display: block;
          width: 256px;
          height: auto;
          margin-top: -25px;
          left: -68px;
        }
        .logo-bg {
          position: absolute;
          display: block;
          width: 100%;
          height: 100%;
          -moz-border-radius: 50%;
          -webkit-border-radius: 50%;
          border-radius: 50%;
          top: 50%; left: 50%;
          box-shadow: 0 0 7px rgba(0, 0, 0, 0.015), 0 0 7px rgba(0, 0, 0, 0.05);
          &.oval-big {
            width: 76px;
            height: 82px;
            background: #a5d6a7;
            margin-top: -41px; margin-left: -38px;
            z-index: 1;
            opacity: 0;
            visibility: hidden;
          }
          &.oval-small {
            width: 68px;
            height: 60px;
            background: #a5d6a7;
            margin-top: -30px; margin-left: -34px;
            z-index: 2;
            opacity: 0;
            visibility: hidden;
          } 
          &.circle {
            width: 48px;
            height: 48px;
            background: #a5d6a7;
            transform: translate( -50%, -50% );
            z-index: 3;
          }
        }
      }
      // navigation main
      .main-navigation {
        position: relative;
        z-index: 5;
        opacity: 0;
        visibility: hidden;
        ul {
          position: relative;
          display: block;
          overflow: hidden;
          width: 100%;
          max-width: 224px;
          list-style-type: none;
          padding: 0;
          margin: 0;
          right: -10px;
          float: right;
          @include maxquery( 640px ) {
            max-width: 124px;
            top: -24px;
          }
          li {
            position: relative;
            display: block;
            float: left;
            padding: 8px;
            @include maxquery( 640px ) {
              width: calc( 100% - 16px );
              display: block;
              text-align: right;
              padding-top: 0;
              padding-bottom: 0;
            }
            a {
              font-family: 'Cardo', serif;
              text-decoration: none;
              color: #363636;
            }
          }
        }
      }
    }
  }

  @-webkit-keyframes rotating /* Safari and Chrome */ {
    from {
      -webkit-transform: rotate(0deg);
      -o-transform: rotate(0deg);
      transform: rotate(0deg);
    }
    to {
      -webkit-transform: rotate(360deg);
      -o-transform: rotate(360deg);
      transform: rotate(360deg);
    }
  }
  @keyframes rotating {
    from {
      -ms-transform: rotate(0deg);
      -moz-transform: rotate(0deg);
      -webkit-transform: rotate(0deg);
      -o-transform: rotate(0deg);
      transform: rotate(0deg);
    }
    to {
      -ms-transform: rotate(360deg);
      -moz-transform: rotate(360deg);
      -webkit-transform: rotate(360deg);
      -o-transform: rotate(360deg);
      transform: rotate(360deg);
    }
  }
  .rotating-fast {
    -webkit-animation: rotating 12s linear infinite;
    -moz-animation: rotating 12s linear infinite;
    -ms-animation: rotating 12s linear infinite;
    -o-animation: rotating 12s linear infinite;
    animation: rotating 12s linear infinite;
  }
  @-webkit-keyframes rotating-inverse /* Safari and Chrome */ {
    from {
      -webkit-transform: rotate(0deg);
      -o-transform: rotate(0deg);
      transform: rotate(0deg);
    }
    to {
      -webkit-transform: rotate(-360deg);
      -o-transform: rotate(-360deg);
      transform: rotate(-360deg);
    }
  }
  @keyframes rotating-inverse {
    from {
      -ms-transform: rotate(0deg);
      -moz-transform: rotate(0deg);
      -webkit-transform: rotate(0deg);
      -o-transform: rotate(0deg);
      transform: rotate(0deg);
    }
    to {
      -ms-transform: rotate(-360deg);
      -moz-transform: rotate(-360deg);
      -webkit-transform: rotate(-360deg);
      -o-transform: rotate(-360deg);
      transform: rotate(-360deg);
    }
  }
  .rotating-slow {
    -webkit-animation: rotating-inverse 16s linear infinite;
    -moz-animation: rotating-inverse 16s linear infinite;
    -ms-animation: rotating-inverse 16s linear infinite;
    -o-animation: rotating-inverse 16s linear infinite;
    animation: rotating-inverse 16s linear infinite;
  }
</style>