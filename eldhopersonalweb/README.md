# wwww
/* Preload images */
body:after {
  display: none;
}

.lightboxOverlay {
  position: absolute;
  top: 0;
  left: 0;
  z-index: 9999;
  background-color: black;
  filter: progid:DXImageTransform.Microsoft.Alpha(Opacity=80);
  opacity: 0.8;
  display: none;
}

.lightbox {
  position: absolute;
  left: 0;
  width: 100%;
  z-index: 10000;
  text-align: center;
  line-height: 0;
  font-weight: normal;
}

.lightbox .lb-image {
  display: block;
  height: auto;
  max-width: inherit;
  -webkit-border-radius: 3px;
  -moz-border-radius: 3px;
  -ms-border-radius: 3px;
  -o-border-radius: 3px;
  border-radius: 3px;
}

.lightbox a img {
  border: none;
}

.lb-outerContainer {
  position: relative;
  background-color: white;
  *zoom: 1;
  width: 250px;
  height: 250px;
  margin: 0 auto;
  -webkit-border-radius: 4px;
  -moz-border-radius: 4px;
  -ms-border-radius: 4px;
  -o-border-radius: 4px;
  border-radius: 4px;
}

.lb-outerContainer:after {
  content: "";
  display: table;
  clear: both;
}

.lb-container {
  padding: 4px;
}

.lb-loader {
  position: absolute;
  top: 43%;
  left: 0;
  height: 25%;
  width: 100%;
  text-align: center;
  line-height: 0;
}

.lb-cancel {
  display: block;
  width: 32px;
  height: 32px;
  margin: 0 auto;
  background: url(../images/loading.gif) no-repeat;
}

.lb-nav {
  position: absolute;
  top: 0;
  left: 0;
  height: 100%;
  width: 100%;
  z-index: 10;
}

.lb-container > .nav {
  left: 0;
}

.lb-nav a {
  outline: none;
  background-image: url('data:image/gif;base64,R0lGODlhAQABAPAAAP///wAAACH5BAEAAAAALAAAAAABAAEAAAICRAEAOw==');
}

.lb-prev, .lb-next {
  height: 100%;
  cursor: pointer;
  display: block;
}

.lb-nav a.lb-prev {
    width: 5em;
    float: left;
    background:url(../images/img-sprite.png) 30px 48% no-repeat;
    filter: progid:DXImageTransform.Microsoft.Alpha(Opacity=0);
    opacity: 0;
    -webkit-transition: opacity 0.6s;
    -moz-transition: opacity 0.6s;
    -o-transition: opacity 0.6s;
    transition: opacity 0.6s;
}

.lb-nav a.lb-prev:hover {
  filter: progid:DXImageTransform.Microsoft.Alpha(Opacity=100);
  opacity: 1;
}

.lb-nav a.lb-next {
    width: 5em;
    right: 0;
    float: right;
    background: url(../images/img-sprite.png) -23px 48% no-repeat;
    filter: progid:DXImageTransform.Microsoft.Alpha(Opacity=0);
    opacity: 0;
    -webkit-transition: opacity 0.6s;
    -moz-transition: opacity 0.6s;
    -o-transition: opacity 0.6s;
    transition: opacity 0.6s;
}
.lb-nav a.lb-next:hover {
  filter: progid:DXImageTransform.Microsoft.Alpha(Opacity=100);
  opacity: 1;
}

.lb-dataContainer {
  margin: 0 auto;
  padding-top: 5px;
  *zoom: 1;
  width: 100%;
  -moz-border-radius-bottomleft: 4px;
  -webkit-border-bottom-left-radius: 4px;
  border-bottom-left-radius: 4px;
  -moz-border-radius-bottomright: 4px;
  -webkit-border-bottom-right-radius: 4px;
  border-bottom-right-radius: 4px;
}

.lb-dataContainer:after {
  content: "";
  display: table;
  clear: both;
}

.lb-data {
  padding: 0 4px;
  color: #ccc;
}

.lb-data .lb-details {
    width: 90%;
    float: left;
    text-align: left;
    line-height: 1.1em;
    margin-top: 2em;
}

.lb-data .lb-caption {
    font-size: 13px;
    line-height: 1.8em;
    color: #fff;
    letter-spacing: 1px;
}

.lb-data .lb-number {
    display: block;
    clear: left;
    padding-top: 1em;
    font-size: 1em;
    color: #fff;
}

.lb-data .lb-close {
  display: block;
  float: right;
  width: 30px;
  height: 30px;
  margin-top: 1.5em;
  background: url(../images/close.png) top right no-repeat;
  text-align: right;
  outline: none;
  filter: progid:DXImageTransform.Microsoft.Alpha(Opacity=70);
  opacity: 0.7;
  -webkit-transition: opacity 0.2s;
  -moz-transition: opacity 0.2s;
  -o-transition: opacity 0.2s;
  transition: opacity 0.2s;
} 
.lb-data .lb-close:hover {
  cursor: pointer;
  filter: progid:DXImageTransform.Microsoft.Alpha(Opacity=100);
  opacity: 1;
}
@media screen and (max-width: 320px){
.lb-data .lb-details {
    width: 89%; 
    margin-top: 1em;
}
.lb-data .lb-caption {
    font-size: 12px;  
}
} 
 359  eldhopersonalweb/css/owl.carousel.css 
@@ -0,0 +1,359 @@
/*
* 	Owl Carousel Owl Demo Theme 
*	v1.24
*/
    #owl-demo .item{
        margin: 3px;
    }
    #owl-demo .item img{
        height: auto;
		    height: auto;
    margin: 0 auto;

    }

.owl-theme .owl-controls{
	margin-top: 0px;
    text-align: center;
}

/* Styling Next and Prev buttons */

.owl-theme .owl-controls .owl-buttons div{
	color: #FFF;
	display: inline-block;
	zoom: 1;
	margin: 5px;
	padding: 3px 10px;
	font-size: 12px;
	width: 13px;
	height: 17px;
}
.owl-next{
	background: url(../images/pagnate.png) no-repeat -10px 0px;
	position: absolute;
	right: 2%;
	top: 95%;
}
.owl-prev{
	background: url(../images/pagnate.png) no-repeat 0px 0px;
	position: absolute;
	right: 3%;
	top: 95%;
}
/* Clickable class fix problem with hover on touch devices */
/* Use it for non-touch hover action */
.owl-theme .owl-controls.clickable .owl-buttons div:hover{
	filter: Alpha(Opacity=100);/*IE7 fix*/
	opacity: 1;
	text-decoration: none;
}

/* Styling Pagination*/

.owl-theme .owl-controls .owl-page{
	display: inline-block;
	zoom: 1;
	*display: inline;/*IE7 life-saver */
}
.owl-theme .owl-controls .owl-page span{
	display: block;
	width: 12px;
    height: 12px;
	margin: 4px;
	filter: Alpha(Opacity=50);/*IE7 fix*/
	opacity: 0.5;
	-webkit-border-radius: 20px;
	-moz-border-radius: 20px;
	border-radius: 20px;
	background: #fff;
}

.owl-theme .owl-controls .owl-page.active span,
.owl-theme .owl-controls.clickable .owl-page:hover span{
	filter: Alpha(Opacity=100);/*IE7 fix*/
	opacity: 1;
}

/* If PaginationNumbers is true */

.owl-theme .owl-controls .owl-page span.owl-numbers{
	height: auto;
	width: auto;
	color: #FFF;
	padding: 2px 10px;
	font-size: 12px;
	-webkit-border-radius: 30px;
	-moz-border-radius: 30px;
	border-radius: 30px;
}

/* preloading images */
.owl-item.loading{
	min-height: 150px;
	background: url(AjaxLoader.gif) no-repeat center center
}
/* 
 * 	Core Owl Carousel CSS File
 *	v1.24
 */

/* clearfix */
.owl-carousel .owl-wrapper:after {
	content: ".";
	display: block;
	clear: both;
	visibility: hidden;
	line-height: 0;
	height: 0;
}
/* display none until init */
.owl-carousel{
	display: none;
	position: relative;
	width: 100%;
	-ms-touch-action: pan-y;
	margin:0em auto;
}
.owl-carousel .owl-wrapper{
	display: none;
	position: relative;
	-webkit-transform: translate3d(0px, 0px, 0px);
}
.owl-carousel .owl-wrapper-outer{
	overflow: hidden;
	position: relative;
	width: 100%;
}
.owl-carousel .owl-wrapper-outer.autoHeight{
	-webkit-transition: height 500ms ease-in-out;
	-moz-transition: height 500ms ease-in-out;
	-ms-transition: height 500ms ease-in-out;
	-o-transition: height 500ms ease-in-out;
	transition: height 500ms ease-in-out;
}

.owl-carousel .owl-item{
	float: left;
}
.owl-controls .owl-page,
.owl-controls .owl-buttons div{
	cursor: pointer;
}
.owl-controls {
	-webkit-user-select: none;
	-khtml-user-select: none;
	-moz-user-select: none;
	-ms-user-select: none;
	user-select: none;
	-webkit-tap-highlight-color: rgba(0, 0, 0, 0);
}

/* mouse grab icon */
.grabbing { 
    cursor:url(grabbing.png) 8 8, move;
}

/* fix */
.owl-carousel  .owl-wrapper,
.owl-carousel  .owl-item{
	-webkit-backface-visibility: hidden;
	-moz-backface-visibility:    hidden;
	-ms-backface-visibility:     hidden;
  -webkit-transform: translate3d(0,0,0);
  -moz-transform: translate3d(0,0,0);
  -ms-transform: translate3d(0,0,0);
}

/* CSS3 Transitions */

.owl-origin {
	-webkit-perspective: 1200px;
	-webkit-perspective-origin-x : 50%;
	-webkit-perspective-origin-y : 50%;
	-moz-perspective : 1200px;
	-moz-perspective-origin-x : 50%;
	-moz-perspective-origin-y : 50%;
	perspective : 1200px;
}
/* fade */
.owl-fade-out {
  z-index: 10;
  -webkit-animation: fadeOut .7s both ease;
  -moz-animation: fadeOut .7s both ease;
  animation: fadeOut .7s both ease;
}
.owl-fade-in {
  -webkit-animation: fadeIn .7s both ease;
  -moz-animation: fadeIn .7s both ease;
  animation: fadeIn .7s both ease;
}
/* backSlide */
.owl-backSlide-out {
  -webkit-animation: backSlideOut 1s both ease;
  -moz-animation: backSlideOut 1s both ease;
  animation: backSlideOut 1s both ease;
}
.owl-backSlide-in {
  -webkit-animation: backSlideIn 1s both ease;
  -moz-animation: backSlideIn 1s both ease;
  animation: backSlideIn 1s both ease;
}
/* goDown */
.owl-goDown-out {
  -webkit-animation: scaleToFade .7s ease both;
  -moz-animation: scaleToFade .7s ease both;
  animation: scaleToFade .7s ease both;
}
.owl-goDown-in {
  -webkit-animation: goDown .6s ease both;
  -moz-animation: goDown .6s ease both;
  animation: goDown .6s ease both;
}
/* scaleUp */
.owl-fadeUp-in {
  -webkit-animation: scaleUpFrom .5s ease both;
  -moz-animation: scaleUpFrom .5s ease both;
  animation: scaleUpFrom .5s ease both;
}

.owl-fadeUp-out {
  -webkit-animation: scaleUpTo .5s ease both;
  -moz-animation: scaleUpTo .5s ease both;
  animation: scaleUpTo .5s ease both;
}
/* Keyframes */
/*empty*/
@-webkit-keyframes empty {
  0% {opacity: 1}
}
@-moz-keyframes empty {
  0% {opacity: 1}
}
@keyframes empty {
  0% {opacity: 1}
}
@-webkit-keyframes fadeIn {
  0% { opacity:0; }
  100% { opacity:1; }
}
@-moz-keyframes fadeIn {
  0% { opacity:0; }
  100% { opacity:1; }
}
@keyframes fadeIn {
  0% { opacity:0; }
  100% { opacity:1; }
}
@-webkit-keyframes fadeOut {
  0% { opacity:1; }
  100% { opacity:0; }
}
@-moz-keyframes fadeOut {
  0% { opacity:1; }
  100% { opacity:0; }
}
@keyframes fadeOut {
  0% { opacity:1; }
  100% { opacity:0; }
}
@-webkit-keyframes backSlideOut {
  25% { opacity: .5; -webkit-transform: translateZ(-500px); }
  75% { opacity: .5; -webkit-transform: translateZ(-500px) translateX(-200%); }
  100% { opacity: .5; -webkit-transform: translateZ(-500px) translateX(-200%); }
}
@-moz-keyframes backSlideOut {
  25% { opacity: .5; -moz-transform: translateZ(-500px); }
  75% { opacity: .5; -moz-transform: translateZ(-500px) translateX(-200%); }
  100% { opacity: .5; -moz-transform: translateZ(-500px) translateX(-200%); }
}
@keyframes backSlideOut {
  25% { opacity: .5; transform: translateZ(-500px); }
  75% { opacity: .5; transform: translateZ(-500px) translateX(-200%); }
  100% { opacity: .5; transform: translateZ(-500px) translateX(-200%); }
}
@-webkit-keyframes backSlideIn {
  0%, 25% { opacity: .5; -webkit-transform: translateZ(-500px) translateX(200%); }
  75% { opacity: .5; -webkit-transform: translateZ(-500px); }
  100% { opacity: 1; -webkit-transform: translateZ(0) translateX(0); }
}
@-moz-keyframes backSlideIn {
  0%, 25% { opacity: .5; -moz-transform: translateZ(-500px) translateX(200%); }
  75% { opacity: .5; -moz-transform: translateZ(-500px); }
  100% { opacity: 1; -moz-transform: translateZ(0) translateX(0); }
}
@keyframes backSlideIn {
  0%, 25% { opacity: .5; transform: translateZ(-500px) translateX(200%); }
  75% { opacity: .5; transform: translateZ(-500px); }
  100% { opacity: 1; transform: translateZ(0) translateX(0); }
}
@-webkit-keyframes scaleToFade {
  to { opacity: 0; -webkit-transform: scale(.8); }
}
@-moz-keyframes scaleToFade {
  to { opacity: 0; -moz-transform: scale(.8); }
}
@keyframes scaleToFade {
  to { opacity: 0; transform: scale(.8); }
}
@-webkit-keyframes goDown {
  from { -webkit-transform: translateY(-100%); }
}
@-moz-keyframes goDown {
  from { -moz-transform: translateY(-100%); }
}
@keyframes goDown {
  from { transform: translateY(-100%); }
}

@-webkit-keyframes scaleUpFrom {
  from { opacity: 0; -webkit-transform: scale(1.5); }
}
@-moz-keyframes scaleUpFrom {
  from { opacity: 0; -moz-transform: scale(1.5); }
}
@keyframes scaleUpFrom {
  from { opacity: 0; transform: scale(1.5); }
}

@-webkit-keyframes scaleUpTo {
  to { opacity: 0; -webkit-transform: scale(1.5); }
}
@-moz-keyframes scaleUpTo {
  to { opacity: 0; -moz-transform: scale(1.5); }
}
@keyframes scaleUpTo {
  to { opacity: 0; transform: scale(1.5); }
}
/*----responsive-mediaquries-----*/
@media (max-width:768px){
	.owl-carousel {
		width: 100%;
	}
}
@media (max-width:640px){
}
@media (max-width:480px){
	.owl-theme .owl-controls .owl-page span {
		display: block;
		width: 12px;
		height: 12px;
	}
}
@media (max-width:320px){
	.owl-carousel {
		width: 90%;
	}
	.owl-prev {
		top: 100%;
	}
	.owl-next {
		right: 1%;
		top: 100%;
	}
	.owl-theme .owl-controls .owl-page span {
		width: 12px;
		height: 12px;
		margin: 5px 5px;
	}
}
 1,152  eldhopersonalweb/css/style.css 
Large diffs are not rendered by default.

 BIN +654 Bytes eldhopersonalweb/images/arr.png 
Binary file not shown.
 BIN +57.8 KB eldhopersonalweb/images/b1.jpg 
Binary file not shown.
 BIN +108 KB eldhopersonalweb/images/blog.jpg 
Binary file not shown.
 BIN +280 Bytes eldhopersonalweb/images/close.png 
Binary file not shown.
 BIN +77.9 KB eldhopersonalweb/images/g1.jpg 
Binary file not shown.
 BIN +66.8 KB eldhopersonalweb/images/g2.jpg 
Binary file not shown.
 BIN +34.2 KB eldhopersonalweb/images/g3.jpg 
Binary file not shown.
 BIN +38.2 KB eldhopersonalweb/images/g4.jpg 
Binary file not shown.
 BIN +25.6 KB eldhopersonalweb/images/g5.jpg 
Binary file not shown.
 BIN +21.1 KB eldhopersonalweb/images/g6.jpg 
Binary file not shown.
 BIN +3.72 KB eldhopersonalweb/images/img-sprite.png 
Binary file not shown.
 BIN +37.4 KB eldhopersonalweb/images/img.jpg 
Binary file not shown.
 BIN +491 KB eldhopersonalweb/images/img1.png 
Binary file not shown.
 BIN +2.74 KB eldhopersonalweb/images/layer.png 
Binary file not shown.
 BIN +8.28 KB eldhopersonalweb/images/loading.gif 
Binary file not shown.
 BIN +211 KB eldhopersonalweb/images/test.jpg 
Binary file not shown.
 BIN +37.1 KB eldhopersonalweb/images/test1.jpg 
Binary file not shown.
 483  eldhopersonalweb/index.html 
Large diffs are not rendered by default.

 523  eldhopersonalweb/js/SmoothScroll.min.js 
Large diffs are not rendered by default.

 3,894  eldhopersonalweb/js/bootstrap.js 
Large diffs are not rendered by default.

 140  eldhopersonalweb/js/easing.js 
@@ -0,0 +1,140 @@
/*
 * jQuery EasIng v1.1.2 - http://gsgd.co.uk/sandbox/jquery.easIng.php
 *
 * Uses the built In easIng capabilities added In jQuery 1.1
 * to offer multiple easIng options
 *
 * Copyright (c) 2007 George Smith
 * Licensed under the MIT License:
 *   http://www.opensource.org/licenses/mit-license.php
 */

// t: current time, b: begInnIng value, c: change In value, d: duration

jQuery.extend( jQuery.easing,
{
	easeInQuad: function (x, t, b, c, d) {
		return c*(t/=d)*t + b;
	},
	easeOutQuad: function (x, t, b, c, d) {
		return -c *(t/=d)*(t-2) + b;
	},
	easeInOutQuad: function (x, t, b, c, d) {
		if ((t/=d/2) < 1) return c/2*t*t + b;
		return -c/2 * ((--t)*(t-2) - 1) + b;
	},
	easeInCubic: function (x, t, b, c, d) {
		return c*(t/=d)*t*t + b;
	},
	easeOutCubic: function (x, t, b, c, d) {
		return c*((t=t/d-1)*t*t + 1) + b;
	},
	easeInOutCubic: function (x, t, b, c, d) {
		if ((t/=d/2) < 1) return c/2*t*t*t + b;
		return c/2*((t-=2)*t*t + 2) + b;
	},
	easeInQuart: function (x, t, b, c, d) {
		return c*(t/=d)*t*t*t + b;
	},
	easeOutQuart: function (x, t, b, c, d) {
		return -c * ((t=t/d-1)*t*t*t - 1) + b;
	},
	easeInOutQuart: function (x, t, b, c, d) {
		if ((t/=d/2) < 1) return c/2*t*t*t*t + b;
		return -c/2 * ((t-=2)*t*t*t - 2) + b;
	},
	easeInQuint: function (x, t, b, c, d) {
		return c*(t/=d)*t*t*t*t + b;
	},
	easeOutQuint: function (x, t, b, c, d) {
		return c*((t=t/d-1)*t*t*t*t + 1) + b;
	},
	easeInOutQuint: function (x, t, b, c, d) {
		if ((t/=d/2) < 1) return c/2*t*t*t*t*t + b;
		return c/2*((t-=2)*t*t*t*t + 2) + b;
	},
	easeInSine: function (x, t, b, c, d) {
		return -c * Math.cos(t/d * (Math.PI/2)) + c + b;
	},
	easeOutSine: function (x, t, b, c, d) {
		return c * Math.sin(t/d * (Math.PI/2)) + b;
	},
	easeInOutSine: function (x, t, b, c, d) {
		return -c/2 * (Math.cos(Math.PI*t/d) - 1) + b;
	},
	easeInExpo: function (x, t, b, c, d) {
		return (t==0) ? b : c * Math.pow(2, 10 * (t/d - 1)) + b;
	},
	easeOutExpo: function (x, t, b, c, d) {
		return (t==d) ? b+c : c * (-Math.pow(2, -10 * t/d) + 1) + b;
	},
	easeInOutExpo: function (x, t, b, c, d) {
		if (t==0) return b;
		if (t==d) return b+c;
		if ((t/=d/2) < 1) return c/2 * Math.pow(2, 10 * (t - 1)) + b;
		return c/2 * (-Math.pow(2, -10 * --t) + 2) + b;
	},
	easeInCirc: function (x, t, b, c, d) {
		return -c * (Math.sqrt(1 - (t/=d)*t) - 1) + b;
	},
	easeOutCirc: function (x, t, b, c, d) {
		return c * Math.sqrt(1 - (t=t/d-1)*t) + b;
	},
	easeInOutCirc: function (x, t, b, c, d) {
		if ((t/=d/2) < 1) return -c/2 * (Math.sqrt(1 - t*t) - 1) + b;
		return c/2 * (Math.sqrt(1 - (t-=2)*t) + 1) + b;
	},
	easeInElastic: function (x, t, b, c, d) {
		var s=1.70158;var p=0;var a=c;
		if (t==0) return b;  if ((t/=d)==1) return b+c;  if (!p) p=d*.3;
		if (a < Math.abs(c)) { a=c; var s=p/4; }
		else var s = p/(2*Math.PI) * Math.asin (c/a);
		return -(a*Math.pow(2,10*(t-=1)) * Math.sin( (t*d-s)*(2*Math.PI)/p )) + b;
	},
	easeOutElastic: function (x, t, b, c, d) {
		var s=1.70158;var p=0;var a=c;
		if (t==0) return b;  if ((t/=d)==1) return b+c;  if (!p) p=d*.3;
		if (a < Math.abs(c)) { a=c; var s=p/4; }
		else var s = p/(2*Math.PI) * Math.asin (c/a);
		return a*Math.pow(2,-10*t) * Math.sin( (t*d-s)*(2*Math.PI)/p ) + c + b;
	},
	easeInOutElastic: function (x, t, b, c, d) {
		var s=1.70158;var p=0;var a=c;
		if (t==0) return b;  if ((t/=d/2)==2) return b+c;  if (!p) p=d*(.3*1.5);
		if (a < Math.abs(c)) { a=c; var s=p/4; }
		else var s = p/(2*Math.PI) * Math.asin (c/a);
		if (t < 1) return -.5*(a*Math.pow(2,10*(t-=1)) * Math.sin( (t*d-s)*(2*Math.PI)/p )) + b;
		return a*Math.pow(2,-10*(t-=1)) * Math.sin( (t*d-s)*(2*Math.PI)/p )*.5 + c + b;
	},
	easeInBack: function (x, t, b, c, d, s) {
		if (s == undefined) s = 1.70158;
		return c*(t/=d)*t*((s+1)*t - s) + b;
	},
	easeOutBack: function (x, t, b, c, d, s) {
		if (s == undefined) s = 1.70158;
		return c*((t=t/d-1)*t*((s+1)*t + s) + 1) + b;
	},
	easeInOutBack: function (x, t, b, c, d, s) {
		if (s == undefined) s = 1.70158; 
		if ((t/=d/2) < 1) return c/2*(t*t*(((s*=(1.525))+1)*t - s)) + b;
		return c/2*((t-=2)*t*(((s*=(1.525))+1)*t + s) + 2) + b;
	},
	easeInBounce: function (x, t, b, c, d) {
		return c - jQuery.easing.easeOutBounce (x, d-t, 0, c, d) + b;
	},
	easeOutBounce: function (x, t, b, c, d) {
		if ((t/=d) < (1/2.75)) {
			return c*(7.5625*t*t) + b;
		} else if (t < (2/2.75)) {
			return c*(7.5625*(t-=(1.5/2.75))*t + .75) + b;
		} else if (t < (2.5/2.75)) {
			return c*(7.5625*(t-=(2.25/2.75))*t + .9375) + b;
		} else {
			return c*(7.5625*(t-=(2.625/2.75))*t + .984375) + b;
		}
	},
	easeInOutBounce: function (x, t, b, c, d) {
		if (t < d/2) return jQuery.easing.easeInBounce (x, t*2, 0, c, d) * .5 + b;
		return jQuery.easing.easeOutBounce (x, t*2-d, 0, c, d) * .5 + c*.5 + b;
	}
});
 4  eldhopersonalweb/js/jquery-2.1.4.min.js 
Large diffs are not rendered by default.

 38  eldhopersonalweb/js/lightbox-plus-jquery.min.js 
Large diffs are not rendered by default.

 5  eldhopersonalweb/js/move-top.js 
 1,470  eldhopersonalweb/js/owl.carousel.js 
Large diffs are not rendered by default.

 55  eldhopersonalweb/w3layouts-License.txt 
@@ -0,0 +1,55 @@
/*
A Design by W3Layouts
Author: W3layouts
Author URL: http://w3layouts.com
License: Creative Commons Attribution 3.0 Unported
License URL: http://creativecommons.org/licenses/by/3.0/
*/
----------------------------------
NOTE : FREQUENTLY ASKED QUESTIONS 
----------------------------------

1. What is W3layouts?

	W3layouts is an initiative of AgileITs to provide free web designs which are cross device supported.

2. Is W3layouts Templates Really Free?

	Yes, all our templates free to use for both commercial and non-commercial, but you have provide a back link to w3layouts.com which is already included in footer design by w3layouts.com don’t edit or remove it.

3. I want to Help W3layouts, How can I?

	You can help w3layouts By
	1. Donate Some $’s, Any Amount your wish
	2. Contribute Design inventory like stock photos, Icons or PSD designs with full rights to w3layouts

4. I want to remove w3layouts.com back link from footer?

	We have two plans for that per template and unlimited.
	Donate us $10 per template. If you want templates for multiple domains or bulk templates please contact support@w3layouts.com

5. Will these templates work on iPhone, Android platforms, Tabs like kindle and Ipads?

	Yes, w3layouts templates work with all Smartphones and Tablets. To, support all the devices we are providing bootstrap Responisve designs WEB Template.

6. What is Web Template?

	WEB template is a responsive design which can be used for desktop users. Users visiting website from desktop browsers can view WEB template


7. Do I need a separate version for Smartphones and Tablets?

	No, WEB Template is compatible in all web browsers, Smartphones and Tablets. 

8. Do I need any database?

	No, it is not necessary.

9. Do you provide WordPress Themes?

	Yes, we are working on it. Check WPMthemes.com

10. Under which license you are providing these templates?

	W3layouts templates are under Creative Commons Attribution 3.0 unported

 BIN +96.3 KB eldhopersonalweb/webfonts/fa-brands-400.eot 
Binary file not shown.
 1,008  eldhopersonalweb/webfonts/fa-brands-400.svg 
Large diffs are not rendered by default.

 BIN +96.1 KB eldhopersonalweb/webfonts/fa-brands-400.ttf 
Binary file not shown.
 BIN +62.2 KB eldhopersonalweb/webfonts/fa-brands-400.woff 
Binary file not shown.
 BIN +53.2 KB eldhopersonalweb/webfonts/fa-brands-400.woff2 
Binary file not shown.
 BIN +30.4 KB eldhopersonalweb/webfonts/fa-regular-400.eot 
Binary file not shown.
 366  eldhopersonalweb/webfonts/fa-regular-400.svg 
Large diffs are not rendered by default.

 BIN +30.2 KB eldhopersonalweb/webfonts/fa-regular-400.ttf 
Binary file not shown.
 BIN +14.4 KB eldhopersonalweb/webfonts/fa-regular-400.woff 
Binary file not shown.
 BIN +12 KB eldhopersonalweb/webfonts/fa-regular-400.woff2 
Binary file not shown.
 BIN +104 KB eldhopersonalweb/webfonts/fa-solid-900.eot 
Binary file not shown.
 1,518  eldhopersonalweb/webfonts/fa-solid-900.svg 
Large diffs are not rendered by default.

 BIN +103 KB eldhopersonalweb/webfonts/fa-solid-900.ttf 
Binary file not shown.
 BIN +49.3 KB eldhopersonalweb/webfonts/fa-solid-900.woff 
Binary file not shown.
 BIN +39.2 KB eldhopersonalweb/webfonts/fa-solid-900.woff2 
Binary file not shown.
0 comments on commit 2215ba7
@eldho51248
 
 
Leave a comment
No file chosen
Attach files by dragging & dropping, selecting or pasting them.
 You’re receiving notifications because you’re watching this repository.
© 2021 GitHub, Inc.
Terms
Privacy
Security
Status
Docs
Contact GitHub
Pricing
API
Training
Blog
About
