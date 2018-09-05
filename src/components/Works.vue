<template>
  <div>

    <div class="works-common-holder fade-component">
      
      <!-- headline START -->
      <h1>Every. Project.<br>Matters.</h1>
      <!-- headline END -->

      <!-- content START -->
      <div class="content">
        <p>Topping tart marshmallow. Muffin icing bear claw ice cream marzipan caramels. Sweet apple pie cotton candy gummies. Brownie icing marzipan.</p>

        <p>Oat cake gingerbread tootsie roll ice cream dragée gummies biscuit pudding fruitcake. Lollipop jelly-o pudding lollipop lemon drops jelly-o lemon drops fruitcake jelly. Dessert sweet roll croissant oat cake muffin carrot cake lemon drops muffin dessert. Sweet dessert ice cream croissant pudding.</p>
      </div>
      <!-- content END -->

    </div>

    <h2 class="divider-line fade-component"><span>MORE</span></h2>

    <div class="works-holder fade-component">
      
      <div class="work" data-image="#D22C22" @mouseenter="over($event)" @mouseleave="leave($event)" :key="0">
        <img class="logo" src="/static/coidea-logo-work.png" alt="MH - Web Designer & Developer - Works - COIDEA" />
        <div class="logo-bg-holder">
          <div class="logo-bg work-oval-big rotating-fast" style="background-color: #FFF !important"></div>
          <div class="logo-bg work-oval-small rotating-slow" style="background-color: #FFF !important"></div>
          <div class="logo-bg work-circle" style="background-color: #FFF !important"></div>
        </div>
        <div class="content">
          <p><strong>FAVORITE #01</strong><br>Client</p>
          <p><strong>DEVELOPMENT</strong><br>SCSS - VUE.JS - WORDPRESS</p>
          <p><strong>ENDPOINT</strong><br>WEB & iOS - ANDROID</p>
          <p><strong>LIVE WEB</strong><br><a href="https://coidea.website" target="_blank">VISIT</a></p>
          <p class="copyright"><span>@ lorem media</span></p>
        </div>
      </div>

      <div class="work" data-image="#777777" @mouseenter="over($event)" @mouseleave="leave($event)" :key="1">
        <img class="logo" src="/static/coidea-logo-work.png" alt="MH - Web Designer & Developer - Works - COIDEA" />
        <div class="logo-bg-holder">
          <div class="logo-bg work-oval-big rotating-fast" style="background-color: #FFFFFF !important"></div>
          <div class="logo-bg work-oval-small rotating-slow" style="background-color: #FFFFFF !important"></div>
          <div class="logo-bg work-circle" style="background-color: #FFFFFF !important"></div>
        </div>
        <div class="content">
          <p><strong>FAVORITE #02</strong><br>Client</p>
          <p><strong>DEVELOPMENT</strong><br>SCSS - GSAP - PIMCORE</p>
          <p><strong>ENDPOINT</strong><br>WEB</p>
          <p class="copyright"><span>@ lorem media</span></p>
        </div>
      </div>

      <div class="work" data-image="#178ED3" @mouseenter="over($event)" @mouseleave="leave($event)" :key="2">
        <img class="logo" src="/static/coidea-logo-work.png" alt="MH - Web Designer & Developer - Works - COIDEA" />
        <div class="logo-bg-holder">
          <div class="logo-bg work-oval-big rotating-fast" style="background-color: #FFFFFF !important"></div>
          <div class="logo-bg work-oval-small rotating-slow" style="background-color: #FFFFFF !important"></div>
          <div class="logo-bg work-circle" style="background-color: #FFFFFF !important"></div>
        </div>
        <div class="content">
          <p><strong>FAVORITE #03</strong><br>Client</p>
          <p><strong>DEVELOPMENT</strong><br>SCSS - GSAP - WORDPRESS</p>
          <p><strong>ENDPOINT</strong><br>WEB</p>
          <p><strong>LIVE</strong><br><a href="https://coidea.website" target="_blank">VISIT</a></p>
          <p class="copyright"><span>@ lorem media</span></p>
        </div>
      </div>

      <div class="work" data-image="#ED7102" @mouseenter="over($event)" @mouseleave="leave($event)" :key="3">
        <img class="logo" src="/static/coidea-logo-work.png" alt="MH - Web Designer & Developer - Works - COIDEA" />
        <div class="logo-bg-holder">
          <div class="logo-bg work-oval-big rotating-fast" style="background-color: #FFFFFF !important"></div>
          <div class="logo-bg work-oval-small rotating-slow" style="background-color: #FFFFFF !important"></div>
          <div class="logo-bg work-circle" style="background-color: #FFFFFF !important"></div>
        </div>
        <div class="content">
          <p><strong>FAVORITE #04</strong><br>Client</p>
          <p><strong>DEVELOPMENT</strong><br>SCSS - GSAP - WOOCOMMERCE</p>
          <p><strong>ENDPOINT</strong><br>WEB</p>
          <p><strong>LIVE</strong><br><a href="https://coidea.website" target="_blank">COMING SOON</a></p>
          <p class="copyright"><span>@ lorem media</span></p>
        </div>
      </div>

      <div class="work" data-image="#7ac3db" @mouseenter="over($event)" @mouseleave="leave($event)" :key="4">
        <img class="logo" src="/static/coidea-logo-work.png" alt="MH - Web Designer & Developer - Works - COIDEA" />
        <div class="logo-bg-holder">
          <div class="logo-bg work-oval-big rotating-fast" style="background-color: #FFFFFF !important"></div>
          <div class="logo-bg work-oval-small rotating-slow" style="background-color: #FFFFFF !important"></div>
          <div class="logo-bg work-circle" style="background-color: #FFFFFF !important"></div>
        </div>
        <div class="content">
          <p><strong>FAVORITE #05</strong><br>Client</p>
          <p><strong>DEVELOPMENT</strong><br>SCSS - VUE.JS - WORDPRESS</p>
          <p><strong>ENDPOINT</strong><br>WEB & iOS - ANDROID</p>
          <p><strong>LIVE WEB</strong><br><a href="https://coidea.website" target="_blank">COMING SOON</a></p>
          <p class="copyright"><span>@ lorem media</span></p>
        </div>
      </div>

      <div class="work" data-image="#62bbc1" @mouseenter="over($event)" @mouseleave="leave($event)" :key="5">
        <img class="logo" src="/static/coidea-logo-work.png" alt="MH - Web Designer & Developer - Works - COIDEA" />
        <div class="logo-bg-holder">
          <div class="logo-bg work-oval-big rotating-fast" style="background-color: #FFFFFF !important"></div>
          <div class="logo-bg work-oval-small rotating-slow" style="background-color: #FFFFFF !important"></div>
          <div class="logo-bg work-circle" style="background-color: #FFFFFF !important"></div>
        </div>
        <div class="content">
          <p><strong>FAVORITE #06</strong><br>Client</p>
          <p><strong>DEVELOPMENT</strong><br>SCSS - VUE.JS - THREE.JS</p>
          <p><strong>ENDPOINT</strong><br>WEB & iOS - ANDROID</p>
          <p><strong>LIVE</strong><br><a href="https://coidea.website" target="_blank">COMING SOON</a></p>
          <p class="copyright"><span>@ lorem media</span></p>
        </div>
      </div>

      <div class="work" data-image="#9c9d9e" @mouseenter="over($event)" @mouseleave="leave($event)" :key="6">
        <img class="logo" src="/static/coidea-logo-work.png" alt="MH - Web Designer & Developer - Works - COIDEA" />
        <div class="logo-bg-holder">
          <div class="logo-bg work-oval-big rotating-fast" style="background-color: #FFFFFF !important"></div>
          <div class="logo-bg work-oval-small rotating-slow" style="background-color: #FFFFFF !important"></div>
          <div class="logo-bg work-circle" style="background-color: #FFFFFF !important"></div>
        </div>
        <div class="content">
          <p><strong>FAVORITE #07</strong><br>Client</p>
          <p><strong>DEVELOPMENT</strong><br>SCSS - ANGULAR - IONIC</p>
          <p><strong>ENDPOINT</strong><br>iOS</p>
          <p class="copyright"><span>@ lorem media</span></p>
        </div>
      </div>

      <div class="work" data-image="#027d2d" @mouseenter="over($event)" @mouseleave="leave($event)" :key="7">
        <img class="logo" src="/static/coidea-logo-work.png" alt="MH - Web Designer & Developer - Works - COIDEA" />
        <div class="logo-bg-holder">
          <div class="logo-bg work-oval-big rotating-fast" style="background-color: #FFFFFF !important"></div>
          <div class="logo-bg work-oval-small rotating-slow" style="background-color: #FFFFFF !important"></div>
          <div class="logo-bg work-circle" style="background-color: #FFFFFF !important"></div>
        </div>
        <div class="content">
          <p><strong>FAVORITE #08</strong><br>Client</p>
          <p><strong>DEVELOPMENT</strong><br>CSS3 - JQUERY - WORDPRESS</p>
          <p><strong>ENDPOINT</strong><br>WEB</p>
          <p><strong>LIVE</strong><br><a href="https://coidea.website" target="_blank">VISIT</a></p>
          <p class="copyright"><span>@ lorem media</span></p>
        </div>
      </div>

      <div class="work" data-image="#f2c849" @mouseenter="over($event)" @mouseleave="leave($event)" :key="8">
        <img class="logo" src="/static/coidea-logo-work.png" alt="MH - Web Designer & Developer - Works - COIDEA" />
        <div class="logo-bg-holder">
          <div class="logo-bg work-oval-big rotating-fast" style="background-color: #FFFFFF !important"></div>
          <div class="logo-bg work-oval-small rotating-slow" style="background-color: #FFFFFF !important"></div>
          <div class="logo-bg work-circle" style="background-color: #FFFFFF !important"></div>
        </div>
        <div class="content">
          <p><strong>FAVORITE #09</strong><br>Client</p>
          <p><strong>DEVELOPMENT</strong><br>CSS3 - JQUERY - WORDPRESS</p>
          <p><strong>ENDPOINT</strong><br>WEB</p>
          <p><strong>LIVE</strong><br><a href="https://coidea.website" target="_blank">VISIT</a> & <a href="https://coidea.website" target="_blank">VISIT</a></p>
          <p class="copyright"><span>@ lorem media</span></p>
        </div>
      </div>

    </div>
    
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
    name: 'Works',
    data () {
      return {
        controller: new ScrollMagic.Controller(),
        timeline: new TimelineMax({ paused:true })
      }
    },
    mounted () {
      
    },
    methods: {
      animateWork: function(thisEvent, action) {
        console.log(thisEvent);
        // common
        // init variables
        this.timeline.set(thisEvent.querySelector('.work-circle'), { autoAlpha: 0, scale:0, z: 0.01 } );
        this.timeline.set(thisEvent.querySelector('.work-oval-small'), { autoAlpha: 0, scale:0, z: 0.01 } );
        this.timeline.set(thisEvent.querySelector('.work-oval-big'), { autoAlpha: 0, scale:0, z: 0.01 } );
        // animate
        this.timeline.fromTo( thisEvent.querySelector('.work-circle'), 1.25, { autoAlpha: 0, scale: 0, transformOrigin:"50% 50%" }, { force3D:true, autoAlpha: 1, scale: 1, transformOrigin:"50% 50%", ease: Back.easeOut.config(1.25) } )
        this.timeline.fromTo( thisEvent.querySelector('.work-oval-small'), 1.25, { autoAlpha: 0, scale: 0, transformOrigin:"50% 50%" }, { force3D:true, autoAlpha: .25, scale: 1, transformOrigin:"50% 50%", ease: Back.easeOut.config(1.25) }, '-=0.75' )
        this.timeline.fromTo( thisEvent.querySelector('.work-oval-big'), 1.25, { autoAlpha: 0, scale: 0, transformOrigin:"50% 50%" }, { force3D:true, autoAlpha: .45,scale: 1, transformOrigin:"50% 50%", ease: Back.easeOut.config(1.25) }, '-=0.75' ) 
        this.timeline.to( thisEvent.querySelector('.work-oval-big'), 0, { className:"+=rotating-fast", ease: Expo.easeOut }, '+=0.35' ) 
        this.timeline.to( thisEvent.querySelector('.work-oval-small'), 0, { className:"+=rotating-slow", ease: Expo.easeOut }, '+=0.35' )
        
        if( action === 'play' ) {
          this.timeline.play();
        }

        if( action === 'reverse' ) {
          this.timeline.reverse();
        }

      },
      over: function(event) {
        let dataImage = event.target.dataset.image;
        $('body').attr('style','background-color: ' + dataImage )
        // this.animateWork(event.target, 'play');
                
      },
      leave: function(event) {
        $('body').attr('style','background-color: #FFFFFF')
        // this.animateWork(event.target, 'reverse');
        
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
  // infos
  .works-common-holder {
    .content {
      position: relative;
      display: block;
      overflow: hidden;
      width: 100%;
      width: calc( 100vw - 120px );
      max-width: 760px;
      padding-bottom: 20px;
      padding-left: 60px;
      @include maxquery( 640px ) {
        width: calc( 100% - 32px );
        padding-left: 0px;
        padding-right: 0px;
      }
    }
  }
  // works
  .works-holder {
    position: relative;
    display: table;
    overflow: hidden;
    .work {
      position: relative;
      display: table;
      overflow: visible;
      width: 31.3333%;
      width: calc( 33.3333% - 32px );
      height: auto;
      min-height: 400px;
      padding: 16px;
      float: left;
      @include maxquery( 992px ) {
        width: 48.3333%;
        width: calc( 50% - 32px );
      }
      @include maxquery( 768px ) {
        width: 98%;
        width: calc( 100% - 32px );
      }
      .content {
        position: absolute;
        display: block;
        width: 100%;
        height: auto;
        font-size: 14px;
        padding: 0px;
        margin: 0px;
        line-height: 18px;
        top: 50%;
        left: -16px;
        transform: translate(0%,-50%);
        opacity: 0;
        visibility: hidden;
        transition: all 0.45s cubic-bezier(1.0, 0.5, 0.8, 1.0);
        p {
          font-size: 16px;
          line-height: 20px;
          padding: 0px;
          margin: 0px;
          padding-bottom: 16px;
          span {
            font-size: 10px;
          }
          &.copyright {
            line-height: 14px;
          }
        }
        a {
          color: #363636;
          text-decoration: none;
        }
      }
      img {
        &.logo {
          max-height: 60%;  
          max-width: 60%; 
          width: auto;
          height: auto;
          position: absolute;  
          top: 0;  
          bottom: 0;  
          left: 0;  
          right: 0;  
          margin: auto;
          z-index: -1;
          transition: all 0.45s cubic-bezier(1.0, 0.5, 0.8, 1.0);
          opacity: 1;
          visibility: visible;
        }
      }
      .logo-bg-holder {
        position: absolute;
        display: block;
        width: 100%;
        height: 100%;
        top: 0;
        right: 0;
        bottom: 0;
        left: 0;
        z-index: -1;
        .logo-bg {
          position: absolute;
          display: block;
          width: 100%;
          height: 100%;
          -moz-border-radius: 50%;
          -webkit-border-radius: 50%;
          border-radius: 50%;
          top: 50%; left: 50%;
          box-shadow: 0 0 36px rgba(0,0,0,0.15), 0 0 36px rgba(0,0,0,0.05);
          transition: all 0.45s cubic-bezier(1.0, 0.5, 0.8, 1.0);
          &.work-oval-big {
            width: 400px;
            height: 360px;
            background: #a5d6a7;
            transform: translate( -50%, -50% );
            z-index: -3;
            opacity: 0;
            visibility: hidden;
          }
          &.work-oval-small {
            width: 300px;
            height: 340px;
            background: #a5d6a7;
            transform: translate( -50%, -50% );
            z-index: -2;
            opacity: 0;
            visibility: hidden;
          } 
          &.work-circle {
            width: 260px;
            height: 260px;
            background: #a5d6a7;
            transform: translate( -50%, -50% );
            z-index: -1;
            opacity: 0;
            visibility: hidden;
          }
        }
      }
      &:hover {
        .content {
          left: 0px;
          opacity: 1;
          visibility: visible;
        }
        img {
          &.logo {
            opacity: 0;
            visibility: hidden;
          }
        }
        .logo-bg-holder {
          .logo-bg {
            &.work-oval-big {
              transform: scale(1) translate( -50%, -50% );
              opacity: 0.25;
              visibility: visible;
            }
            &.work-oval-small {
              transform: scale(1) translate( -50%, -50% );
              opacity: 0.45;
              visibility: visible;
            }
            &.work-circle {
              transform: scale(1) translate( -50%, -50% );
              opacity: 1;
              visibility: visible;
            }
          }
        }
      }
    }
  }
  @-webkit-keyframes rotating /* Safari and Chrome */ {
    from {
      -webkit-transform: translate( -50%, -50% ) rotate(0deg);
      -o-transform: translate( -50%, -50% ) rotate(0deg);
      transform: translate( -50%, -50% ) rotate(0deg);
    }
    to {
      -webkit-transform: translate( -50%, -50% ) rotate(360deg);
      -o-transform: translate( -50%, -50% ) rotate(360deg);
      transform: translate( -50%, -50% ) rotate(360deg);
    }
  }
  @keyframes rotating {
    from {
      -ms-transform: translate( -50%, -50% ) rotate(0deg);
      -moz-transform: translate( -50%, -50% ) rotate(0deg);
      -webkit-transform: translate( -50%, -50% ) rotate(0deg);
      -o-transform: translate( -50%, -50% ) rotate(0deg);
      transform: translate( -50%, -50% ) rotate(0deg);
    }
    to {
      -ms-transform: translate( -50%, -50% ) rotate(360deg);
      -moz-transform: translate( -50%, -50% ) rotate(360deg);
      -webkit-transform: translate( -50%, -50% ) rotate(360deg);
      -o-transform: translate( -50%, -50% ) rotate(360deg);
      transform: translate( -50%, -50% ) rotate(360deg);
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
      -webkit-transform: translate( -50%, -50% ) rotate(0deg);
      -o-transform: translate( -50%, -50% ) rotate(0deg);
      transform: translate( -50%, -50% ) rotate(0deg);
    }
    to {
      -webkit-transform: translate( -50%, -50% ) rotate(-360deg);
      -o-transform: translate( -50%, -50% ) rotate(-360deg);
      transform: translate( -50%, -50% ) rotate(-360deg);
    }
  }
  @keyframes rotating-inverse {
    from {
      -ms-transform: translate( -50%, -50% ) rotate(0deg);
      -moz-transform: translate( -50%, -50% ) rotate(0deg);
      -webkit-transform: translate( -50%, -50% ) rotate(0deg);
      -o-transform: translate( -50%, -50% ) rotate(0deg);
      transform: translate( -50%, -50% ) rotate(0deg);
    }
    to {
      -ms-transform: translate( -50%, -50% ) rotate(-360deg);
      -moz-transform: translate( -50%, -50% ) rotate(-360deg);
      -webkit-transform: translate( -50%, -50% ) rotate(-360deg);
      -o-transform: translate( -50%, -50% ) rotate(-360deg);
      transform: translate( -50%, -50% ) rotate(-360deg);
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