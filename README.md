<!DOCTYPE html>
<html>
<head><meta charset="utf-8" />

<title>plot</title>

<script src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.1.10/require.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/2.0.3/jquery.min.js"></script>



<style type="text/css">
    /*!
*
* Twitter Bootstrap
*
*/
/*!
 * Bootstrap v3.3.7 (http://getbootstrap.com)
 * Copyright 2011-2016 Twitter, Inc.
 * Licensed under MIT (https://github.com/twbs/bootstrap/blob/master/LICENSE)
 */
/*! normalize.css v3.0.3 | MIT License | github.com/necolas/normalize.css */
html {
  font-family: sans-serif;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
}
body {
  margin: 0;
}
article,
aside,
details,
figcaption,
figure,
footer,
header,
hgroup,
main,
menu,
nav,
section,
summary {
  display: block;
}
audio,
canvas,
progress,
video {
  display: inline-block;
  vertical-align: baseline;
}
audio:not([controls]) {
  display: none;
  height: 0;
}
[hidden],
template {
  display: none;
}
a {
  background-color: transparent;
}
a:active,
a:hover {
  outline: 0;
}
abbr[title] {
  border-bottom: 1px dotted;
}
b,
strong {
  font-weight: bold;
}
dfn {
  font-style: italic;
}
h1 {
  font-size: 2em;
  margin: 0.67em 0;
}
mark {
  background: #ff0;
  color: #000;
}
small {
  font-size: 80%;
}
sub,
sup {
  font-size: 75%;
  line-height: 0;
  position: relative;
  vertical-align: baseline;
}
sup {
  top: -0.5em;
}
sub {
  bottom: -0.25em;
}
img {
  border: 0;
}
svg:not(:root) {
  overflow: hidden;
}
figure {
  margin: 1em 40px;
}
hr {
  box-sizing: content-box;
  height: 0;
}
pre {
  overflow: auto;
}
code,
kbd,
pre,
samp {
  font-family: monospace, monospace;
  font-size: 1em;
}
button,
input,
optgroup,
select,
textarea {
  color: inherit;
  font: inherit;
  margin: 0;
}
button {
  overflow: visible;
}
button,
select {
  text-transform: none;
}
button,
html input[type="button"],
input[type="reset"],
input[type="submit"] {
  -webkit-appearance: button;
  cursor: pointer;
}
button[disabled],
html input[disabled] {
  cursor: default;
}
button::-moz-focus-inner,
input::-moz-focus-inner {
  border: 0;
  padding: 0;
}
input {
  line-height: normal;
}
input[type="checkbox"],
input[type="radio"] {
  box-sizing: border-box;
  padding: 0;
}
input[type="number"]::-webkit-inner-spin-button,
input[type="number"]::-webkit-outer-spin-button {
  height: auto;
}
input[type="search"] {
  -webkit-appearance: textfield;
  box-sizing: content-box;
}
input[type="search"]::-webkit-search-cancel-button,
input[type="search"]::-webkit-search-decoration {
  -webkit-appearance: none;
}
fieldset {
  border: 1px solid #c0c0c0;
  margin: 0 2px;
  padding: 0.35em 0.625em 0.75em;
}
legend {
  border: 0;
  padding: 0;
}
textarea {
  overflow: auto;
}
optgroup {
  font-weight: bold;
}
table {
  border-collapse: collapse;
  border-spacing: 0;
}
td,
th {
  padding: 0;
}
/*! Source: https://github.com/h5bp/html5-boilerplate/blob/master/src/css/main.css */
@media print {
  *,
  *:before,
  *:after {
    background: transparent !important;
    box-shadow: none !important;
    text-shadow: none !important;
  }
  a,
  a:visited {
    text-decoration: underline;
  }
  a[href]:after {
    content: " (" attr(href) ")";
  }
  abbr[title]:after {
    content: " (" attr(title) ")";
  }
  a[href^="#"]:after,
  a[href^="javascript:"]:after {
    content: "";
  }
  pre,
  blockquote {
    border: 1px solid #999;
    page-break-inside: avoid;
  }
  thead {
    display: table-header-group;
  }
  tr,
  img {
    page-break-inside: avoid;
  }
  img {
    max-width: 100% !important;
  }
  p,
  h2,
  h3 {
    orphans: 3;
    widows: 3;
  }
  h2,
  h3 {
    page-break-after: avoid;
  }
  .navbar {
    display: none;
  }
  .btn > .caret,
  .dropup > .btn > .caret {
    border-top-color: #000 !important;
  }
  .label {
    border: 1px solid #000;
  }
  .table {
    border-collapse: collapse !important;
  }
  .table td,
  .table th {
    background-color: #fff !important;
  }
  .table-bordered th,
  .table-bordered td {
    border: 1px solid #ddd !important;
  }
}
@font-face {
  font-family: 'Glyphicons Halflings';
  src: url('../components/bootstrap/fonts/glyphicons-halflings-regular.eot');
  src: url('../components/bootstrap/fonts/glyphicons-halflings-regular.eot?#iefix') format('embedded-opentype'), url('../components/bootstrap/fonts/glyphicons-halflings-regular.woff2') format('woff2'), url('../components/bootstrap/fonts/glyphicons-halflings-regular.woff') format('woff'), url('../components/bootstrap/fonts/glyphicons-halflings-regular.ttf') format('truetype'), url('../components/bootstrap/fonts/glyphicons-halflings-regular.svg#glyphicons_halflingsregular') format('svg');
}
.glyphicon {
  position: relative;
  top: 1px;
  display: inline-block;
  font-family: 'Glyphicons Halflings';
  font-style: normal;
  font-weight: normal;
  line-height: 1;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
.glyphicon-asterisk:before {
  content: "\002a";
}
.glyphicon-plus:before {
  content: "\002b";
}
.glyphicon-euro:before,
.glyphicon-eur:before {
  content: "\20ac";
}
.glyphicon-minus:before {
  content: "\2212";
}
.glyphicon-cloud:before {
  content: "\2601";
}
.glyphicon-envelope:before {
  content: "\2709";
}
.glyphicon-pencil:before {
  content: "\270f";
}
.glyphicon-glass:before {
  content: "\e001";
}
.glyphicon-music:before {
  content: "\e002";
}
.glyphicon-search:before {
  content: "\e003";
}
.glyphicon-heart:before {
  content: "\e005";
}
.glyphicon-star:before {
  content: "\e006";
}
.glyphicon-star-empty:before {
  content: "\e007";
}
.glyphicon-user:before {
  content: "\e008";
}
.glyphicon-film:before {
  content: "\e009";
}
.glyphicon-th-large:before {
  content: "\e010";
}
.glyphicon-th:before {
  content: "\e011";
}
.glyphicon-th-list:before {
  content: "\e012";
}
.glyphicon-ok:before {
  content: "\e013";
}
.glyphicon-remove:before {
  content: "\e014";
}
.glyphicon-zoom-in:before {
  content: "\e015";
}
.glyphicon-zoom-out:before {
  content: "\e016";
}
.glyphicon-off:before {
  content: "\e017";
}
.glyphicon-signal:before {
  content: "\e018";
}
.glyphicon-cog:before {
  content: "\e019";
}
.glyphicon-trash:before {
  content: "\e020";
}
.glyphicon-home:before {
  content: "\e021";
}
.glyphicon-file:before {
  content: "\e022";
}
.glyphicon-time:before {
  content: "\e023";
}
.glyphicon-road:before {
  content: "\e024";
}
.glyphicon-download-alt:before {
  content: "\e025";
}
.glyphicon-download:before {
  content: "\e026";
}
.glyphicon-upload:before {
  content: "\e027";
}
.glyphicon-inbox:before {
  content: "\e028";
}
.glyphicon-play-circle:before {
  content: "\e029";
}
.glyphicon-repeat:before {
  content: "\e030";
}
.glyphicon-refresh:before {
  content: "\e031";
}
.glyphicon-list-alt:before {
  content: "\e032";
}
.glyphicon-lock:before {
  content: "\e033";
}
.glyphicon-flag:before {
  content: "\e034";
}
.glyphicon-headphones:before {
  content: "\e035";
}
.glyphicon-volume-off:before {
  content: "\e036";
}
.glyphicon-volume-down:before {
  content: "\e037";
}
.glyphicon-volume-up:before {
  content: "\e038";
}
.glyphicon-qrcode:before {
  content: "\e039";
}
.glyphicon-barcode:before {
  content: "\e040";
}
.glyphicon-tag:before {
  content: "\e041";
}
.glyphicon-tags:before {
  content: "\e042";
}
.glyphicon-book:before {
  content: "\e043";
}
.glyphicon-bookmark:before {
  content: "\e044";
}
.glyphicon-print:before {
  content: "\e045";
}
.glyphicon-camera:before {
  content: "\e046";
}
.glyphicon-font:before {
  content: "\e047";
}
.glyphicon-bold:before {
  content: "\e048";
}
.glyphicon-italic:before {
  content: "\e049";
}
.glyphicon-text-height:before {
  content: "\e050";
}
.glyphicon-text-width:before {
  content: "\e051";
}
.glyphicon-align-left:before {
  content: "\e052";
}
.glyphicon-align-center:before {
  content: "\e053";
}
.glyphicon-align-right:before {
  content: "\e054";
}
.glyphicon-align-justify:before {
  content: "\e055";
}
.glyphicon-list:before {
  content: "\e056";
}
.glyphicon-indent-left:before {
  content: "\e057";
}
.glyphicon-indent-right:before {
  content: "\e058";
}
.glyphicon-facetime-video:before {
  content: "\e059";
}
.glyphicon-picture:before {
  content: "\e060";
}
.glyphicon-map-marker:before {
  content: "\e062";
}
.glyphicon-adjust:before {
  content: "\e063";
}
.glyphicon-tint:before {
  content: "\e064";
}
.glyphicon-edit:before {
  content: "\e065";
}
.glyphicon-share:before {
  content: "\e066";
}
.glyphicon-check:before {
  content: "\e067";
}
.glyphicon-move:before {
  content: "\e068";
}
.glyphicon-step-backward:before {
  content: "\e069";
}
.glyphicon-fast-backward:before {
  content: "\e070";
}
.glyphicon-backward:before {
  content: "\e071";
}
.glyphicon-play:before {
  content: "\e072";
}
.glyphicon-pause:before {
  content: "\e073";
}
.glyphicon-stop:before {
  content: "\e074";
}
.glyphicon-forward:before {
  content: "\e075";
}
.glyphicon-fast-forward:before {
  content: "\e076";
}
.glyphicon-step-forward:before {
  content: "\e077";
}
.glyphicon-eject:before {
  content: "\e078";
}
.glyphicon-chevron-left:before {
  content: "\e079";
}
.glyphicon-chevron-right:before {
  content: "\e080";
}
.glyphicon-plus-sign:before {
  content: "\e081";
}
.glyphicon-minus-sign:before {
  content: "\e082";
}
.glyphicon-remove-sign:before {
  content: "\e083";
}
.glyphicon-ok-sign:before {
  content: "\e084";
}
.glyphicon-question-sign:before {
  content: "\e085";
}
.glyphicon-info-sign:before {
  content: "\e086";
}
.glyphicon-screenshot:before {
  content: "\e087";
}
.glyphicon-remove-circle:before {
  content: "\e088";
}
.glyphicon-ok-circle:before {
  content: "\e089";
}
.glyphicon-ban-circle:before {
  content: "\e090";
}
.glyphicon-arrow-left:before {
  content: "\e091";
}
.glyphicon-arrow-right:before {
  content: "\e092";
}
.glyphicon-arrow-up:before {
  content: "\e093";
}
.glyphicon-arrow-down:before {
  content: "\e094";
}
.glyphicon-share-alt:before {
  content: "\e095";
}
.glyphicon-resize-full:before {
  content: "\e096";
}
.glyphicon-resize-small:before {
  content: "\e097";
}
.glyphicon-exclamation-sign:before {
  content: "\e101";
}
.glyphicon-gift:before {
  content: "\e102";
}
.glyphicon-leaf:before {
  content: "\e103";
}
.glyphicon-fire:before {
  content: "\e104";
}
.glyphicon-eye-open:before {
  content: "\e105";
}
.glyphicon-eye-close:before {
  content: "\e106";
}
.glyphicon-warning-sign:before {
  content: "\e107";
}
.glyphicon-plane:before {
  content: "\e108";
}
.glyphicon-calendar:before {
  content: "\e109";
}
.glyphicon-random:before {
  content: "\e110";
}
.glyphicon-comment:before {
  content: "\e111";
}
.glyphicon-magnet:before {
  content: "\e112";
}
.glyphicon-chevron-up:before {
  content: "\e113";
}
.glyphicon-chevron-down:before {
  content: "\e114";
}
.glyphicon-retweet:before {
  content: "\e115";
}
.glyphicon-shopping-cart:before {
  content: "\e116";
}
.glyphicon-folder-close:before {
  content: "\e117";
}
.glyphicon-folder-open:before {
  content: "\e118";
}
.glyphicon-resize-vertical:before {
  content: "\e119";
}
.glyphicon-resize-horizontal:before {
  content: "\e120";
}
.glyphicon-hdd:before {
  content: "\e121";
}
.glyphicon-bullhorn:before {
  content: "\e122";
}
.glyphicon-bell:before {
  content: "\e123";
}
.glyphicon-certificate:before {
  content: "\e124";
}
.glyphicon-thumbs-up:before {
  content: "\e125";
}
.glyphicon-thumbs-down:before {
  content: "\e126";
}
.glyphicon-hand-right:before {
  content: "\e127";
}
.glyphicon-hand-left:before {
  content: "\e128";
}
.glyphicon-hand-up:before {
  content: "\e129";
}
.glyphicon-hand-down:before {
  content: "\e130";
}
.glyphicon-circle-arrow-right:before {
  content: "\e131";
}
.glyphicon-circle-arrow-left:before {
  content: "\e132";
}
.glyphicon-circle-arrow-up:before {
  content: "\e133";
}
.glyphicon-circle-arrow-down:before {
  content: "\e134";
}
.glyphicon-globe:before {
  content: "\e135";
}
.glyphicon-wrench:before {
  content: "\e136";
}
.glyphicon-tasks:before {
  content: "\e137";
}
.glyphicon-filter:before {
  content: "\e138";
}
.glyphicon-briefcase:before {
  content: "\e139";
}
.glyphicon-fullscreen:before {
  content: "\e140";
}
.glyphicon-dashboard:before {
  content: "\e141";
}
.glyphicon-paperclip:before {
  content: "\e142";
}
.glyphicon-heart-empty:before {
  content: "\e143";
}
.glyphicon-link:before {
  content: "\e144";
}
.glyphicon-phone:before {
  content: "\e145";
}
.glyphicon-pushpin:before {
  content: "\e146";
}
.glyphicon-usd:before {
  content: "\e148";
}
.glyphicon-gbp:before {
  content: "\e149";
}
.glyphicon-sort:before {
  content: "\e150";
}
.glyphicon-sort-by-alphabet:before {
  content: "\e151";
}
.glyphicon-sort-by-alphabet-alt:before {
  content: "\e152";
}
.glyphicon-sort-by-order:before {
  content: "\e153";
}
.glyphicon-sort-by-order-alt:before {
  content: "\e154";
}
.glyphicon-sort-by-attributes:before {
  content: "\e155";
}
.glyphicon-sort-by-attributes-alt:before {
  content: "\e156";
}
.glyphicon-unchecked:before {
  content: "\e157";
}
.glyphicon-expand:before {
  content: "\e158";
}
.glyphicon-collapse-down:before {
  content: "\e159";
}
.glyphicon-collapse-up:before {
  content: "\e160";
}
.glyphicon-log-in:before {
  content: "\e161";
}
.glyphicon-flash:before {
  content: "\e162";
}
.glyphicon-log-out:before {
  content: "\e163";
}
.glyphicon-new-window:before {
  content: "\e164";
}
.glyphicon-record:before {
  content: "\e165";
}
.glyphicon-save:before {
  content: "\e166";
}
.glyphicon-open:before {
  content: "\e167";
}
.glyphicon-saved:before {
  content: "\e168";
}
.glyphicon-import:before {
  content: "\e169";
}
.glyphicon-export:before {
  content: "\e170";
}
.glyphicon-send:before {
  content: "\e171";
}
.glyphicon-floppy-disk:before {
  content: "\e172";
}
.glyphicon-floppy-saved:before {
  content: "\e173";
}
.glyphicon-floppy-remove:before {
  content: "\e174";
}
.glyphicon-floppy-save:before {
  content: "\e175";
}
.glyphicon-floppy-open:before {
  content: "\e176";
}
.glyphicon-credit-card:before {
  content: "\e177";
}
.glyphicon-transfer:before {
  content: "\e178";
}
.glyphicon-cutlery:before {
  content: "\e179";
}
.glyphicon-header:before {
  content: "\e180";
}
.glyphicon-compressed:before {
  content: "\e181";
}
.glyphicon-earphone:before {
  content: "\e182";
}
.glyphicon-phone-alt:before {
  content: "\e183";
}
.glyphicon-tower:before {
  content: "\e184";
}
.glyphicon-stats:before {
  content: "\e185";
}
.glyphicon-sd-video:before {
  content: "\e186";
}
.glyphicon-hd-video:before {
  content: "\e187";
}
.glyphicon-subtitles:before {
  content: "\e188";
}
.glyphicon-sound-stereo:before {
  content: "\e189";
}
.glyphicon-sound-dolby:before {
  content: "\e190";
}
.glyphicon-sound-5-1:before {
  content: "\e191";
}
.glyphicon-sound-6-1:before {
  content: "\e192";
}
.glyphicon-sound-7-1:before {
  content: "\e193";
}
.glyphicon-copyright-mark:before {
  content: "\e194";
}
.glyphicon-registration-mark:before {
  content: "\e195";
}
.glyphicon-cloud-download:before {
  content: "\e197";
}
.glyphicon-cloud-upload:before {
  content: "\e198";
}
.glyphicon-tree-conifer:before {
  content: "\e199";
}
.glyphicon-tree-deciduous:before {
  content: "\e200";
}
.glyphicon-cd:before {
  content: "\e201";
}
.glyphicon-save-file:before {
  content: "\e202";
}
.glyphicon-open-file:before {
  content: "\e203";
}
.glyphicon-level-up:before {
  content: "\e204";
}
.glyphicon-copy:before {
  content: "\e205";
}
.glyphicon-paste:before {
  content: "\e206";
}
.glyphicon-alert:before {
  content: "\e209";
}
.glyphicon-equalizer:before {
  content: "\e210";
}
.glyphicon-king:before {
  content: "\e211";
}
.glyphicon-queen:before {
  content: "\e212";
}
.glyphicon-pawn:before {
  content: "\e213";
}
.glyphicon-bishop:before {
  content: "\e214";
}
.glyphicon-knight:before {
  content: "\e215";
}
.glyphicon-baby-formula:before {
  content: "\e216";
}
.glyphicon-tent:before {
  content: "\26fa";
}
.glyphicon-blackboard:before {
  content: "\e218";
}
.glyphicon-bed:before {
  content: "\e219";
}
.glyphicon-apple:before {
  content: "\f8ff";
}
.glyphicon-erase:before {
  content: "\e221";
}
.glyphicon-hourglass:before {
  content: "\231b";
}
.glyphicon-lamp:before {
  content: "\e223";
}
.glyphicon-duplicate:before {
  content: "\e224";
}
.glyphicon-piggy-bank:before {
  content: "\e225";
}
.glyphicon-scissors:before {
  content: "\e226";
}
.glyphicon-bitcoin:before {
  content: "\e227";
}
.glyphicon-btc:before {
  content: "\e227";
}
.glyphicon-xbt:before {
  content: "\e227";
}
.glyphicon-yen:before {
  content: "\00a5";
}
.glyphicon-jpy:before {
  content: "\00a5";
}
.glyphicon-ruble:before {
  content: "\20bd";
}
.glyphicon-rub:before {
  content: "\20bd";
}
.glyphicon-scale:before {
  content: "\e230";
}
.glyphicon-ice-lolly:before {
  content: "\e231";
}
.glyphicon-ice-lolly-tasted:before {
  content: "\e232";
}
.glyphicon-education:before {
  content: "\e233";
}
.glyphicon-option-horizontal:before {
  content: "\e234";
}
.glyphicon-option-vertical:before {
  content: "\e235";
}
.glyphicon-menu-hamburger:before {
  content: "\e236";
}
.glyphicon-modal-window:before {
  content: "\e237";
}
.glyphicon-oil:before {
  content: "\e238";
}
.glyphicon-grain:before {
  content: "\e239";
}
.glyphicon-sunglasses:before {
  content: "\e240";
}
.glyphicon-text-size:before {
  content: "\e241";
}
.glyphicon-text-color:before {
  content: "\e242";
}
.glyphicon-text-background:before {
  content: "\e243";
}
.glyphicon-object-align-top:before {
  content: "\e244";
}
.glyphicon-object-align-bottom:before {
  content: "\e245";
}
.glyphicon-object-align-horizontal:before {
  content: "\e246";
}
.glyphicon-object-align-left:before {
  content: "\e247";
}
.glyphicon-object-align-vertical:before {
  content: "\e248";
}
.glyphicon-object-align-right:before {
  content: "\e249";
}
.glyphicon-triangle-right:before {
  content: "\e250";
}
.glyphicon-triangle-left:before {
  content: "\e251";
}
.glyphicon-triangle-bottom:before {
  content: "\e252";
}
.glyphicon-triangle-top:before {
  content: "\e253";
}
.glyphicon-console:before {
  content: "\e254";
}
.glyphicon-superscript:before {
  content: "\e255";
}
.glyphicon-subscript:before {
  content: "\e256";
}
.glyphicon-menu-left:before {
  content: "\e257";
}
.glyphicon-menu-right:before {
  content: "\e258";
}
.glyphicon-menu-down:before {
  content: "\e259";
}
.glyphicon-menu-up:before {
  content: "\e260";
}
* {
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box;
}
*:before,
*:after {
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box;
}
html {
  font-size: 10px;
  -webkit-tap-highlight-color: rgba(0, 0, 0, 0);
}
body {
  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
  font-size: 13px;
  line-height: 1.42857143;
  color: #000;
  background-color: #fff;
}
input,
button,
select,
textarea {
  font-family: inherit;
  font-size: inherit;
  line-height: inherit;
}
a {
  color: #337ab7;
  text-decoration: none;
}
a:hover,
a:focus {
  color: #23527c;
  text-decoration: underline;
}
a:focus {
  outline: 5px auto -webkit-focus-ring-color;
  outline-offset: -2px;
}
figure {
  margin: 0;
}
img {
  vertical-align: middle;
}
.img-responsive,
.thumbnail > img,
.thumbnail a > img,
.carousel-inner > .item > img,
.carousel-inner > .item > a > img {
  display: block;
  max-width: 100%;
  height: auto;
}
.img-rounded {
  border-radius: 3px;
}
.img-thumbnail {
  padding: 4px;
  line-height: 1.42857143;
  background-color: #fff;
  border: 1px solid #ddd;
  border-radius: 2px;
  -webkit-transition: all 0.2s ease-in-out;
  -o-transition: all 0.2s ease-in-out;
  transition: all 0.2s ease-in-out;
  display: inline-block;
  max-width: 100%;
  height: auto;
}
.img-circle {
  border-radius: 50%;
}
hr {
  margin-top: 18px;
  margin-bottom: 18px;
  border: 0;
  border-top: 1px solid #eeeeee;
}
.sr-only {
  position: absolute;
  width: 1px;
  height: 1px;
  margin: -1px;
  padding: 0;
  overflow: hidden;
  clip: rect(0, 0, 0, 0);
  border: 0;
}
.sr-only-focusable:active,
.sr-only-focusable:focus {
  position: static;
  width: auto;
  height: auto;
  margin: 0;
  overflow: visible;
  clip: auto;
}
[role="button"] {
  cursor: pointer;
}
h1,
h2,
h3,
h4,
h5,
h6,
.h1,
.h2,
.h3,
.h4,
.h5,
.h6 {
  font-family: inherit;
  font-weight: 500;
  line-height: 1.1;
  color: inherit;
}
h1 small,
h2 small,
h3 small,
h4 small,
h5 small,
h6 small,
.h1 small,
.h2 small,
.h3 small,
.h4 small,
.h5 small,
.h6 small,
h1 .small,
h2 .small,
h3 .small,
h4 .small,
h5 .small,
h6 .small,
.h1 .small,
.h2 .small,
.h3 .small,
.h4 .small,
.h5 .small,
.h6 .small {
  font-weight: normal;
  line-height: 1;
  color: #777777;
}
h1,
.h1,
h2,
.h2,
h3,
.h3 {
  margin-top: 18px;
  margin-bottom: 9px;
}
h1 small,
.h1 small,
h2 small,
.h2 small,
h3 small,
.h3 small,
h1 .small,
.h1 .small,
h2 .small,
.h2 .small,
h3 .small,
.h3 .small {
  font-size: 65%;
}
h4,
.h4,
h5,
.h5,
h6,
.h6 {
  margin-top: 9px;
  margin-bottom: 9px;
}
h4 small,
.h4 small,
h5 small,
.h5 small,
h6 small,
.h6 small,
h4 .small,
.h4 .small,
h5 .small,
.h5 .small,
h6 .small,
.h6 .small {
  font-size: 75%;
}
h1,
.h1 {
  font-size: 33px;
}
h2,
.h2 {
  font-size: 27px;
}
h3,
.h3 {
  font-size: 23px;
}
h4,
.h4 {
  font-size: 17px;
}
h5,
.h5 {
  font-size: 13px;
}
h6,
.h6 {
  font-size: 12px;
}
p {
  margin: 0 0 9px;
}
.lead {
  margin-bottom: 18px;
  font-size: 14px;
  font-weight: 300;
  line-height: 1.4;
}
@media (min-width: 768px) {
  .lead {
    font-size: 19.5px;
  }
}
small,
.small {
  font-size: 92%;
}
mark,
.mark {
  background-color: #fcf8e3;
  padding: .2em;
}
.text-left {
  text-align: left;
}
.text-right {
  text-align: right;
}
.text-center {
  text-align: center;
}
.text-justify {
  text-align: justify;
}
.text-nowrap {
  white-space: nowrap;
}
.text-lowercase {
  text-transform: lowercase;
}
.text-uppercase {
  text-transform: uppercase;
}
.text-capitalize {
  text-transform: capitalize;
}
.text-muted {
  color: #777777;
}
.text-primary {
  color: #337ab7;
}
a.text-primary:hover,
a.text-primary:focus {
  color: #286090;
}
.text-success {
  color: #3c763d;
}
a.text-success:hover,
a.text-success:focus {
  color: #2b542c;
}
.text-info {
  color: #31708f;
}
a.text-info:hover,
a.text-info:focus {
  color: #245269;
}
.text-warning {
  color: #8a6d3b;
}
a.text-warning:hover,
a.text-warning:focus {
  color: #66512c;
}
.text-danger {
  color: #a94442;
}
a.text-danger:hover,
a.text-danger:focus {
  color: #843534;
}
.bg-primary {
  color: #fff;
  background-color: #337ab7;
}
a.bg-primary:hover,
a.bg-primary:focus {
  background-color: #286090;
}
.bg-success {
  background-color: #dff0d8;
}
a.bg-success:hover,
a.bg-success:focus {
  background-color: #c1e2b3;
}
.bg-info {
  background-color: #d9edf7;
}
a.bg-info:hover,
a.bg-info:focus {
  background-color: #afd9ee;
}
.bg-warning {
  background-color: #fcf8e3;
}
a.bg-warning:hover,
a.bg-warning:focus {
  background-color: #f7ecb5;
}
.bg-danger {
  background-color: #f2dede;
}
a.bg-danger:hover,
a.bg-danger:focus {
  background-color: #e4b9b9;
}
.page-header {
  padding-bottom: 8px;
  margin: 36px 0 18px;
  border-bottom: 1px solid #eeeeee;
}
ul,
ol {
  margin-top: 0;
  margin-bottom: 9px;
}
ul ul,
ol ul,
ul ol,
ol ol {
  margin-bottom: 0;
}
.list-unstyled {
  padding-left: 0;
  list-style: none;
}
.list-inline {
  padding-left: 0;
  list-style: none;
  margin-left: -5px;
}
.list-inline > li {
  display: inline-block;
  padding-left: 5px;
  padding-right: 5px;
}
dl {
  margin-top: 0;
  margin-bottom: 18px;
}
dt,
dd {
  line-height: 1.42857143;
}
dt {
  font-weight: bold;
}
dd {
  margin-left: 0;
}
@media (min-width: 541px) {
  .dl-horizontal dt {
    float: left;
    width: 160px;
    clear: left;
    text-align: right;
    overflow: hidden;
    text-overflow: ellipsis;
    white-space: nowrap;
  }
  .dl-horizontal dd {
    margin-left: 180px;
  }
}
abbr[title],
abbr[data-original-title] {
  cursor: help;
  border-bottom: 1px dotted #777777;
}
.initialism {
  font-size: 90%;
  text-transform: uppercase;
}
blockquote {
  padding: 9px 18px;
  margin: 0 0 18px;
  font-size: inherit;
  border-left: 5px solid #eeeeee;
}
blockquote p:last-child,
blockquote ul:last-child,
blockquote ol:last-child {
  margin-bottom: 0;
}
blockquote footer,
blockquote small,
blockquote .small {
  display: block;
  font-size: 80%;
  line-height: 1.42857143;
  color: #777777;
}
blockquote footer:before,
blockquote small:before,
blockquote .small:before {
  content: '\2014 \00A0';
}
.blockquote-reverse,
blockquote.pull-right {
  padding-right: 15px;
  padding-left: 0;
  border-right: 5px solid #eeeeee;
  border-left: 0;
  text-align: right;
}
.blockquote-reverse footer:before,
blockquote.pull-right footer:before,
.blockquote-reverse small:before,
blockquote.pull-right small:before,
.blockquote-reverse .small:before,
blockquote.pull-right .small:before {
  content: '';
}
.blockquote-reverse footer:after,
blockquote.pull-right footer:after,
.blockquote-reverse small:after,
blockquote.pull-right small:after,
.blockquote-reverse .small:after,
blockquote.pull-right .small:after {
  content: '\00A0 \2014';
}
address {
  margin-bottom: 18px;
  font-style: normal;
  line-height: 1.42857143;
}
code,
kbd,
pre,
samp {
  font-family: monospace;
}
code {
  padding: 2px 4px;
  font-size: 90%;
  color: #c7254e;
  background-color: #f9f2f4;
  border-radius: 2px;
}
kbd {
  padding: 2px 4px;
  font-size: 90%;
  color: #888;
  background-color: transparent;
  border-radius: 1px;
  box-shadow: inset 0 -1px 0 rgba(0, 0, 0, 0.25);
}
kbd kbd {
  padding: 0;
  font-size: 100%;
  font-weight: bold;
  box-shadow: none;
}
pre {
  display: block;
  padding: 8.5px;
  margin: 0 0 9px;
  font-size: 12px;
  line-height: 1.42857143;
  word-break: break-all;
  word-wrap: break-word;
  color: #333333;
  background-color: #f5f5f5;
  border: 1px solid #ccc;
  border-radius: 2px;
}
pre code {
  padding: 0;
  font-size: inherit;
  color: inherit;
  white-space: pre-wrap;
  background-color: transparent;
  border-radius: 0;
}
.pre-scrollable {
  max-height: 340px;
  overflow-y: scroll;
}
.container {
  margin-right: auto;
  margin-left: auto;
  padding-left: 0px;
  padding-right: 0px;
}
@media (min-width: 768px) {
  .container {
    width: 768px;
  }
}
@media (min-width: 992px) {
  .container {
    width: 940px;
  }
}
@media (min-width: 1200px) {
  .container {
    width: 1140px;
  }
}
.container-fluid {
  margin-right: auto;
  margin-left: auto;
  padding-left: 0px;
  padding-right: 0px;
}
.row {
  margin-left: 0px;
  margin-right: 0px;
}
.col-xs-1, .col-sm-1, .col-md-1, .col-lg-1, .col-xs-2, .col-sm-2, .col-md-2, .col-lg-2, .col-xs-3, .col-sm-3, .col-md-3, .col-lg-3, .col-xs-4, .col-sm-4, .col-md-4, .col-lg-4, .col-xs-5, .col-sm-5, .col-md-5, .col-lg-5, .col-xs-6, .col-sm-6, .col-md-6, .col-lg-6, .col-xs-7, .col-sm-7, .col-md-7, .col-lg-7, .col-xs-8, .col-sm-8, .col-md-8, .col-lg-8, .col-xs-9, .col-sm-9, .col-md-9, .col-lg-9, .col-xs-10, .col-sm-10, .col-md-10, .col-lg-10, .col-xs-11, .col-sm-11, .col-md-11, .col-lg-11, .col-xs-12, .col-sm-12, .col-md-12, .col-lg-12 {
  position: relative;
  min-height: 1px;
  padding-left: 0px;
  padding-right: 0px;
}
.col-xs-1, .col-xs-2, .col-xs-3, .col-xs-4, .col-xs-5, .col-xs-6, .col-xs-7, .col-xs-8, .col-xs-9, .col-xs-10, .col-xs-11, .col-xs-12 {
  float: left;
}
.col-xs-12 {
  width: 100%;
}
.col-xs-11 {
  width: 91.66666667%;
}
.col-xs-10 {
  width: 83.33333333%;
}
.col-xs-9 {
  width: 75%;
}
.col-xs-8 {
  width: 66.66666667%;
}
.col-xs-7 {
  width: 58.33333333%;
}
.col-xs-6 {
  width: 50%;
}
.col-xs-5 {
  width: 41.66666667%;
}
.col-xs-4 {
  width: 33.33333333%;
}
.col-xs-3 {
  width: 25%;
}
.col-xs-2 {
  width: 16.66666667%;
}
.col-xs-1 {
  width: 8.33333333%;
}
.col-xs-pull-12 {
  right: 100%;
}
.col-xs-pull-11 {
  right: 91.66666667%;
}
.col-xs-pull-10 {
  right: 83.33333333%;
}
.col-xs-pull-9 {
  right: 75%;
}
.col-xs-pull-8 {
  right: 66.66666667%;
}
.col-xs-pull-7 {
  right: 58.33333333%;
}
.col-xs-pull-6 {
  right: 50%;
}
.col-xs-pull-5 {
  right: 41.66666667%;
}
.col-xs-pull-4 {
  right: 33.33333333%;
}
.col-xs-pull-3 {
  right: 25%;
}
.col-xs-pull-2 {
  right: 16.66666667%;
}
.col-xs-pull-1 {
  right: 8.33333333%;
}
.col-xs-pull-0 {
  right: auto;
}
.col-xs-push-12 {
  left: 100%;
}
.col-xs-push-11 {
  left: 91.66666667%;
}
.col-xs-push-10 {
  left: 83.33333333%;
}
.col-xs-push-9 {
  left: 75%;
}
.col-xs-push-8 {
  left: 66.66666667%;
}
.col-xs-push-7 {
  left: 58.33333333%;
}
.col-xs-push-6 {
  left: 50%;
}
.col-xs-push-5 {
  left: 41.66666667%;
}
.col-xs-push-4 {
  left: 33.33333333%;
}
.col-xs-push-3 {
  left: 25%;
}
.col-xs-push-2 {
  left: 16.66666667%;
}
.col-xs-push-1 {
  left: 8.33333333%;
}
.col-xs-push-0 {
  left: auto;
}
.col-xs-offset-12 {
  margin-left: 100%;
}
.col-xs-offset-11 {
  margin-left: 91.66666667%;
}
.col-xs-offset-10 {
  margin-left: 83.33333333%;
}
.col-xs-offset-9 {
  margin-left: 75%;
}
.col-xs-offset-8 {
  margin-left: 66.66666667%;
}
.col-xs-offset-7 {
  margin-left: 58.33333333%;
}
.col-xs-offset-6 {
  margin-left: 50%;
}
.col-xs-offset-5 {
  margin-left: 41.66666667%;
}
.col-xs-offset-4 {
  margin-left: 33.33333333%;
}
.col-xs-offset-3 {
  margin-left: 25%;
}
.col-xs-offset-2 {
  margin-left: 16.66666667%;
}
.col-xs-offset-1 {
  margin-left: 8.33333333%;
}
.col-xs-offset-0 {
  margin-left: 0%;
}
@media (min-width: 768px) {
  .col-sm-1, .col-sm-2, .col-sm-3, .col-sm-4, .col-sm-5, .col-sm-6, .col-sm-7, .col-sm-8, .col-sm-9, .col-sm-10, .col-sm-11, .col-sm-12 {
    float: left;
  }
  .col-sm-12 {
    width: 100%;
  }
  .col-sm-11 {
    width: 91.66666667%;
  }
  .col-sm-10 {
    width: 83.33333333%;
  }
  .col-sm-9 {
    width: 75%;
  }
  .col-sm-8 {
    width: 66.66666667%;
  }
  .col-sm-7 {
    width: 58.33333333%;
  }
  .col-sm-6 {
    width: 50%;
  }
  .col-sm-5 {
    width: 41.66666667%;
  }
  .col-sm-4 {
    width: 33.33333333%;
  }
  .col-sm-3 {
    width: 25%;
  }
  .col-sm-2 {
    width: 16.66666667%;
  }
  .col-sm-1 {
    width: 8.33333333%;
  }
  .col-sm-pull-12 {
    right: 100%;
  }
  .col-sm-pull-11 {
    right: 91.66666667%;
  }
  .col-sm-pull-10 {
    right: 83.33333333%;
  }
  .col-sm-pull-9 {
    right: 75%;
  }
  .col-sm-pull-8 {
    right: 66.66666667%;
  }
  .col-sm-pull-7 {
    right: 58.33333333%;
  }
  .col-sm-pull-6 {
    right: 50%;
  }
  .col-sm-pull-5 {
    right: 41.66666667%;
  }
  .col-sm-pull-4 {
    right: 33.33333333%;
  }
  .col-sm-pull-3 {
    right: 25%;
  }
  .col-sm-pull-2 {
    right: 16.66666667%;
  }
  .col-sm-pull-1 {
    right: 8.33333333%;
  }
  .col-sm-pull-0 {
    right: auto;
  }
  .col-sm-push-12 {
    left: 100%;
  }
  .col-sm-push-11 {
    left: 91.66666667%;
  }
  .col-sm-push-10 {
    left: 83.33333333%;
  }
  .col-sm-push-9 {
    left: 75%;
  }
  .col-sm-push-8 {
    left: 66.66666667%;
  }
  .col-sm-push-7 {
    left: 58.33333333%;
  }
  .col-sm-push-6 {
    left: 50%;
  }
  .col-sm-push-5 {
    left: 41.66666667%;
  }
  .col-sm-push-4 {
    left: 33.33333333%;
  }
  .col-sm-push-3 {
    left: 25%;
  }
  .col-sm-push-2 {
    left: 16.66666667%;
  }
  .col-sm-push-1 {
    left: 8.33333333%;
  }
  .col-sm-push-0 {
    left: auto;
  }
  .col-sm-offset-12 {
    margin-left: 100%;
  }
  .col-sm-offset-11 {
    margin-left: 91.66666667%;
  }
  .col-sm-offset-10 {
    margin-left: 83.33333333%;
  }
  .col-sm-offset-9 {
    margin-left: 75%;
  }
  .col-sm-offset-8 {
    margin-left: 66.66666667%;
  }
  .col-sm-offset-7 {
    margin-left: 58.33333333%;
  }
  .col-sm-offset-6 {
    margin-left: 50%;
  }
  .col-sm-offset-5 {
    margin-left: 41.66666667%;
  }
  .col-sm-offset-4 {
    margin-left: 33.33333333%;
  }
  .col-sm-offset-3 {
    margin-left: 25%;
  }
  .col-sm-offset-2 {
    margin-left: 16.66666667%;
  }
  .col-sm-offset-1 {
    margin-left: 8.33333333%;
  }
  .col-sm-offset-0 {
    margin-left: 0%;
  }
}
@media (min-width: 992px) {
  .col-md-1, .col-md-2, .col-md-3, .col-md-4, .col-md-5, .col-md-6, .col-md-7, .col-md-8, .col-md-9, .col-md-10, .col-md-11, .col-md-12 {
    float: left;
  }
  .col-md-12 {
    width: 100%;
  }
  .col-md-11 {
    width: 91.66666667%;
  }
  .col-md-10 {
    width: 83.33333333%;
  }
  .col-md-9 {
    width: 75%;
  }
  .col-md-8 {
    width: 66.66666667%;
  }
  .col-md-7 {
    width: 58.33333333%;
  }
  .col-md-6 {
    width: 50%;
  }
  .col-md-5 {
    width: 41.66666667%;
  }
  .col-md-4 {
    width: 33.33333333%;
  }
  .col-md-3 {
    width: 25%;
  }
  .col-md-2 {
    width: 16.66666667%;
  }
  .col-md-1 {
    width: 8.33333333%;
  }
  .col-md-pull-12 {
    right: 100%;
  }
  .col-md-pull-11 {
    right: 91.66666667%;
  }
  .col-md-pull-10 {
    right: 83.33333333%;
  }
  .col-md-pull-9 {
    right: 75%;
  }
  .col-md-pull-8 {
    right: 66.66666667%;
  }
  .col-md-pull-7 {
    right: 58.33333333%;
  }
  .col-md-pull-6 {
    right: 50%;
  }
  .col-md-pull-5 {
    right: 41.66666667%;
  }
  .col-md-pull-4 {
    right: 33.33333333%;
  }
  .col-md-pull-3 {
    right: 25%;
  }
  .col-md-pull-2 {
    right: 16.66666667%;
  }
  .col-md-pull-1 {
    right: 8.33333333%;
  }
  .col-md-pull-0 {
    right: auto;
  }
  .col-md-push-12 {
    left: 100%;
  }
  .col-md-push-11 {
    left: 91.66666667%;
  }
  .col-md-push-10 {
    left: 83.33333333%;
  }
  .col-md-push-9 {
    left: 75%;
  }
  .col-md-push-8 {
    left: 66.66666667%;
  }
  .col-md-push-7 {
    left: 58.33333333%;
  }
  .col-md-push-6 {
    left: 50%;
  }
  .col-md-push-5 {
    left: 41.66666667%;
  }
  .col-md-push-4 {
    left: 33.33333333%;
  }
  .col-md-push-3 {
    left: 25%;
  }
  .col-md-push-2 {
    left: 16.66666667%;
  }
  .col-md-push-1 {
    left: 8.33333333%;
  }
  .col-md-push-0 {
    left: auto;
  }
  .col-md-offset-12 {
    margin-left: 100%;
  }
  .col-md-offset-11 {
    margin-left: 91.66666667%;
  }
  .col-md-offset-10 {
    margin-left: 83.33333333%;
  }
  .col-md-offset-9 {
    margin-left: 75%;
  }
  .col-md-offset-8 {
    margin-left: 66.66666667%;
  }
  .col-md-offset-7 {
    margin-left: 58.33333333%;
  }
  .col-md-offset-6 {
    margin-left: 50%;
  }
  .col-md-offset-5 {
    margin-left: 41.66666667%;
  }
  .col-md-offset-4 {
    margin-left: 33.33333333%;
  }
  .col-md-offset-3 {
    margin-left: 25%;
  }
  .col-md-offset-2 {
    margin-left: 16.66666667%;
  }
  .col-md-offset-1 {
    margin-left: 8.33333333%;
  }
  .col-md-offset-0 {
    margin-left: 0%;
  }
}
@media (min-width: 1200px) {
  .col-lg-1, .col-lg-2, .col-lg-3, .col-lg-4, .col-lg-5, .col-lg-6, .col-lg-7, .col-lg-8, .col-lg-9, .col-lg-10, .col-lg-11, .col-lg-12 {
    float: left;
  }
  .col-lg-12 {
    width: 100%;
  }
  .col-lg-11 {
    width: 91.66666667%;
  }
  .col-lg-10 {
    width: 83.33333333%;
  }
  .col-lg-9 {
    width: 75%;
  }
  .col-lg-8 {
    width: 66.66666667%;
  }
  .col-lg-7 {
    width: 58.33333333%;
  }
  .col-lg-6 {
    width: 50%;
  }
  .col-lg-5 {
    width: 41.66666667%;
  }
  .col-lg-4 {
    width: 33.33333333%;
  }
  .col-lg-3 {
    width: 25%;
  }
  .col-lg-2 {
    width: 16.66666667%;
  }
  .col-lg-1 {
    width: 8.33333333%;
  }
  .col-lg-pull-12 {
    right: 100%;
  }
  .col-lg-pull-11 {
    right: 91.66666667%;
  }
  .col-lg-pull-10 {
    right: 83.33333333%;
  }
  .col-lg-pull-9 {
    right: 75%;
  }
  .col-lg-pull-8 {
    right: 66.66666667%;
  }
  .col-lg-pull-7 {
    right: 58.33333333%;
  }
  .col-lg-pull-6 {
    right: 50%;
  }
  .col-lg-pull-5 {
    right: 41.66666667%;
  }
  .col-lg-pull-4 {
    right: 33.33333333%;
  }
  .col-lg-pull-3 {
    right: 25%;
  }
  .col-lg-pull-2 {
    right: 16.66666667%;
  }
  .col-lg-pull-1 {
    right: 8.33333333%;
  }
  .col-lg-pull-0 {
    right: auto;
  }
  .col-lg-push-12 {
    left: 100%;
  }
  .col-lg-push-11 {
    left: 91.66666667%;
  }
  .col-lg-push-10 {
    left: 83.33333333%;
  }
  .col-lg-push-9 {
    left: 75%;
  }
  .col-lg-push-8 {
    left: 66.66666667%;
  }
  .col-lg-push-7 {
    left: 58.33333333%;
  }
  .col-lg-push-6 {
    left: 50%;
  }
  .col-lg-push-5 {
    left: 41.66666667%;
  }
  .col-lg-push-4 {
    left: 33.33333333%;
  }
  .col-lg-push-3 {
    left: 25%;
  }
  .col-lg-push-2 {
    left: 16.66666667%;
  }
  .col-lg-push-1 {
    left: 8.33333333%;
  }
  .col-lg-push-0 {
    left: auto;
  }
  .col-lg-offset-12 {
    margin-left: 100%;
  }
  .col-lg-offset-11 {
    margin-left: 91.66666667%;
  }
  .col-lg-offset-10 {
    margin-left: 83.33333333%;
  }
  .col-lg-offset-9 {
    margin-left: 75%;
  }
  .col-lg-offset-8 {
    margin-left: 66.66666667%;
  }
  .col-lg-offset-7 {
    margin-left: 58.33333333%;
  }
  .col-lg-offset-6 {
    margin-left: 50%;
  }
  .col-lg-offset-5 {
    margin-left: 41.66666667%;
  }
  .col-lg-offset-4 {
    margin-left: 33.33333333%;
  }
  .col-lg-offset-3 {
    margin-left: 25%;
  }
  .col-lg-offset-2 {
    margin-left: 16.66666667%;
  }
  .col-lg-offset-1 {
    margin-left: 8.33333333%;
  }
  .col-lg-offset-0 {
    margin-left: 0%;
  }
}
table {
  background-color: transparent;
}
caption {
  padding-top: 8px;
  padding-bottom: 8px;
  color: #777777;
  text-align: left;
}
th {
  text-align: left;
}
.table {
  width: 100%;
  max-width: 100%;
  margin-bottom: 18px;
}
.table > thead > tr > th,
.table > tbody > tr > th,
.table > tfoot > tr > th,
.table > thead > tr > td,
.table > tbody > tr > td,
.table > tfoot > tr > td {
  padding: 8px;
  line-height: 1.42857143;
  vertical-align: top;
  border-top: 1px solid #ddd;
}
.table > thead > tr > th {
  vertical-align: bottom;
  border-bottom: 2px solid #ddd;
}
.table > caption + thead > tr:first-child > th,
.table > colgroup + thead > tr:first-child > th,
.table > thead:first-child > tr:first-child > th,
.table > caption + thead > tr:first-child > td,
.table > colgroup + thead > tr:first-child > td,
.table > thead:first-child > tr:first-child > td {
  border-top: 0;
}
.table > tbody + tbody {
  border-top: 2px solid #ddd;
}
.table .table {
  background-color: #fff;
}
.table-condensed > thead > tr > th,
.table-condensed > tbody > tr > th,
.table-condensed > tfoot > tr > th,
.table-condensed > thead > tr > td,
.table-condensed > tbody > tr > td,
.table-condensed > tfoot > tr > td {
  padding: 5px;
}
.table-bordered {
  border: 1px solid #ddd;
}
.table-bordered > thead > tr > th,
.table-bordered > tbody > tr > th,
.table-bordered > tfoot > tr > th,
.table-bordered > thead > tr > td,
.table-bordered > tbody > tr > td,
.table-bordered > tfoot > tr > td {
  border: 1px solid #ddd;
}
.table-bordered > thead > tr > th,
.table-bordered > thead > tr > td {
  border-bottom-width: 2px;
}
.table-striped > tbody > tr:nth-of-type(odd) {
  background-color: #f9f9f9;
}
.table-hover > tbody > tr:hover {
  background-color: #f5f5f5;
}
table col[class*="col-"] {
  position: static;
  float: none;
  display: table-column;
}
table td[class*="col-"],
table th[class*="col-"] {
  position: static;
  float: none;
  display: table-cell;
}
.table > thead > tr > td.active,
.table > tbody > tr > td.active,
.table > tfoot > tr > td.active,
.table > thead > tr > th.active,
.table > tbody > tr > th.active,
.table > tfoot > tr > th.active,
.table > thead > tr.active > td,
.table > tbody > tr.active > td,
.table > tfoot > tr.active > td,
.table > thead > tr.active > th,
.table > tbody > tr.active > th,
.table > tfoot > tr.active > th {
  background-color: #f5f5f5;
}
.table-hover > tbody > tr > td.active:hover,
.table-hover > tbody > tr > th.active:hover,
.table-hover > tbody > tr.active:hover > td,
.table-hover > tbody > tr:hover > .active,
.table-hover > tbody > tr.active:hover > th {
  background-color: #e8e8e8;
}
.table > thead > tr > td.success,
.table > tbody > tr > td.success,
.table > tfoot > tr > td.success,
.table > thead > tr > th.success,
.table > tbody > tr > th.success,
.table > tfoot > tr > th.success,
.table > thead > tr.success > td,
.table > tbody > tr.success > td,
.table > tfoot > tr.success > td,
.table > thead > tr.success > th,
.table > tbody > tr.success > th,
.table > tfoot > tr.success > th {
  background-color: #dff0d8;
}
.table-hover > tbody > tr > td.success:hover,
.table-hover > tbody > tr > th.success:hover,
.table-hover > tbody > tr.success:hover > td,
.table-hover > tbody > tr:hover > .success,
.table-hover > tbody > tr.success:hover > th {
  background-color: #d0e9c6;
}
.table > thead > tr > td.info,
.table > tbody > tr > td.info,
.table > tfoot > tr > td.info,
.table > thead > tr > th.info,
.table > tbody > tr > th.info,
.table > tfoot > tr > th.info,
.table > thead > tr.info > td,
.table > tbody > tr.info > td,
.table > tfoot > tr.info > td,
.table > thead > tr.info > th,
.table > tbody > tr.info > th,
.table > tfoot > tr.info > th {
  background-color: #d9edf7;
}
.table-hover > tbody > tr > td.info:hover,
.table-hover > tbody > tr > th.info:hover,
.table-hover > tbody > tr.info:hover > td,
.table-hover > tbody > tr:hover > .info,
.table-hover > tbody > tr.info:hover > th {
  background-color: #c4e3f3;
}
.table > thead > tr > td.warning,
.table > tbody > tr > td.warning,
.table > tfoot > tr > td.warning,
.table > thead > tr > th.warning,
.table > tbody > tr > th.warning,
.table > tfoot > tr > th.warning,
.table > thead > tr.warning > td,
.table > tbody > tr.warning > td,
.table > tfoot > tr.warning > td,
.table > thead > tr.warning > th,
.table > tbody > tr.warning > th,
.table > tfoot > tr.warning > th {
  background-color: #fcf8e3;
}
.table-hover > tbody > tr > td.warning:hover,
.table-hover > tbody > tr > th.warning:hover,
.table-hover > tbody > tr.warning:hover > td,
.table-hover > tbody > tr:hover > .warning,
.table-hover > tbody > tr.warning:hover > th {
  background-color: #faf2cc;
}
.table > thead > tr > td.danger,
.table > tbody > tr > td.danger,
.table > tfoot > tr > td.danger,
.table > thead > tr > th.danger,
.table > tbody > tr > th.danger,
.table > tfoot > tr > th.danger,
.table > thead > tr.danger > td,
.table > tbody > tr.danger > td,
.table > tfoot > tr.danger > td,
.table > thead > tr.danger > th,
.table > tbody > tr.danger > th,
.table > tfoot > tr.danger > th {
  background-color: #f2dede;
}
.table-hover > tbody > tr > td.danger:hover,
.table-hover > tbody > tr > th.danger:hover,
.table-hover > tbody > tr.danger:hover > td,
.table-hover > tbody > tr:hover > .danger,
.table-hover > tbody > tr.danger:hover > th {
  background-color: #ebcccc;
}
.table-responsive {
  overflow-x: auto;
  min-height: 0.01%;
}
@media screen and (max-width: 767px) {
  .table-responsive {
    width: 100%;
    margin-bottom: 13.5px;
    overflow-y: hidden;
    -ms-overflow-style: -ms-autohiding-scrollbar;
    border: 1px solid #ddd;
  }
  .table-responsive > .table {
    margin-bottom: 0;
  }
  .table-responsive > .table > thead > tr > th,
  .table-responsive > .table > tbody > tr > th,
  .table-responsive > .table > tfoot > tr > th,
  .table-responsive > .table > thead > tr > td,
  .table-responsive > .table > tbody > tr > td,
  .table-responsive > .table > tfoot > tr > td {
    white-space: nowrap;
  }
  .table-responsive > .table-bordered {
    border: 0;
  }
  .table-responsive > .table-bordered > thead > tr > th:first-child,
  .table-responsive > .table-bordered > tbody > tr > th:first-child,
  .table-responsive > .table-bordered > tfoot > tr > th:first-child,
  .table-responsive > .table-bordered > thead > tr > td:first-child,
  .table-responsive > .table-bordered > tbody > tr > td:first-child,
  .table-responsive > .table-bordered > tfoot > tr > td:first-child {
    border-left: 0;
  }
  .table-responsive > .table-bordered > thead > tr > th:last-child,
  .table-responsive > .table-bordered > tbody > tr > th:last-child,
  .table-responsive > .table-bordered > tfoot > tr > th:last-child,
  .table-responsive > .table-bordered > thead > tr > td:last-child,
  .table-responsive > .table-bordered > tbody > tr > td:last-child,
  .table-responsive > .table-bordered > tfoot > tr > td:last-child {
    border-right: 0;
  }
  .table-responsive > .table-bordered > tbody > tr:last-child > th,
  .table-responsive > .table-bordered > tfoot > tr:last-child > th,
  .table-responsive > .table-bordered > tbody > tr:last-child > td,
  .table-responsive > .table-bordered > tfoot > tr:last-child > td {
    border-bottom: 0;
  }
}
fieldset {
  padding: 0;
  margin: 0;
  border: 0;
  min-width: 0;
}
legend {
  display: block;
  width: 100%;
  padding: 0;
  margin-bottom: 18px;
  font-size: 19.5px;
  line-height: inherit;
  color: #333333;
  border: 0;
  border-bottom: 1px solid #e5e5e5;
}
label {
  display: inline-block;
  max-width: 100%;
  margin-bottom: 5px;
  font-weight: bold;
}
input[type="search"] {
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box;
}
input[type="radio"],
input[type="checkbox"] {
  margin: 4px 0 0;
  margin-top: 1px \9;
  line-height: normal;
}
input[type="file"] {
  display: block;
}
input[type="range"] {
  display: block;
  width: 100%;
}
select[multiple],
select[size] {
  height: auto;
}
input[type="file"]:focus,
input[type="radio"]:focus,
input[type="checkbox"]:focus {
  outline: 5px auto -webkit-focus-ring-color;
  outline-offset: -2px;
}
output {
  display: block;
  padding-top: 7px;
  font-size: 13px;
  line-height: 1.42857143;
  color: #555555;
}
.form-control {
  display: block;
  width: 100%;
  height: 32px;
  padding: 6px 12px;
  font-size: 13px;
  line-height: 1.42857143;
  color: #555555;
  background-color: #fff;
  background-image: none;
  border: 1px solid #ccc;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  -webkit-transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  -o-transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
}
.form-control:focus {
  border-color: #66afe9;
  outline: 0;
  -webkit-box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, 0.6);
  box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, 0.6);
}
.form-control::-moz-placeholder {
  color: #999;
  opacity: 1;
}
.form-control:-ms-input-placeholder {
  color: #999;
}
.form-control::-webkit-input-placeholder {
  color: #999;
}
.form-control::-ms-expand {
  border: 0;
  background-color: transparent;
}
.form-control[disabled],
.form-control[readonly],
fieldset[disabled] .form-control {
  background-color: #eeeeee;
  opacity: 1;
}
.form-control[disabled],
fieldset[disabled] .form-control {
  cursor: not-allowed;
}
textarea.form-control {
  height: auto;
}
input[type="search"] {
  -webkit-appearance: none;
}
@media screen and (-webkit-min-device-pixel-ratio: 0) {
  input[type="date"].form-control,
  input[type="time"].form-control,
  input[type="datetime-local"].form-control,
  input[type="month"].form-control {
    line-height: 32px;
  }
  input[type="date"].input-sm,
  input[type="time"].input-sm,
  input[type="datetime-local"].input-sm,
  input[type="month"].input-sm,
  .input-group-sm input[type="date"],
  .input-group-sm input[type="time"],
  .input-group-sm input[type="datetime-local"],
  .input-group-sm input[type="month"] {
    line-height: 30px;
  }
  input[type="date"].input-lg,
  input[type="time"].input-lg,
  input[type="datetime-local"].input-lg,
  input[type="month"].input-lg,
  .input-group-lg input[type="date"],
  .input-group-lg input[type="time"],
  .input-group-lg input[type="datetime-local"],
  .input-group-lg input[type="month"] {
    line-height: 45px;
  }
}
.form-group {
  margin-bottom: 15px;
}
.radio,
.checkbox {
  position: relative;
  display: block;
  margin-top: 10px;
  margin-bottom: 10px;
}
.radio label,
.checkbox label {
  min-height: 18px;
  padding-left: 20px;
  margin-bottom: 0;
  font-weight: normal;
  cursor: pointer;
}
.radio input[type="radio"],
.radio-inline input[type="radio"],
.checkbox input[type="checkbox"],
.checkbox-inline input[type="checkbox"] {
  position: absolute;
  margin-left: -20px;
  margin-top: 4px \9;
}
.radio + .radio,
.checkbox + .checkbox {
  margin-top: -5px;
}
.radio-inline,
.checkbox-inline {
  position: relative;
  display: inline-block;
  padding-left: 20px;
  margin-bottom: 0;
  vertical-align: middle;
  font-weight: normal;
  cursor: pointer;
}
.radio-inline + .radio-inline,
.checkbox-inline + .checkbox-inline {
  margin-top: 0;
  margin-left: 10px;
}
input[type="radio"][disabled],
input[type="checkbox"][disabled],
input[type="radio"].disabled,
input[type="checkbox"].disabled,
fieldset[disabled] input[type="radio"],
fieldset[disabled] input[type="checkbox"] {
  cursor: not-allowed;
}
.radio-inline.disabled,
.checkbox-inline.disabled,
fieldset[disabled] .radio-inline,
fieldset[disabled] .checkbox-inline {
  cursor: not-allowed;
}
.radio.disabled label,
.checkbox.disabled label,
fieldset[disabled] .radio label,
fieldset[disabled] .checkbox label {
  cursor: not-allowed;
}
.form-control-static {
  padding-top: 7px;
  padding-bottom: 7px;
  margin-bottom: 0;
  min-height: 31px;
}
.form-control-static.input-lg,
.form-control-static.input-sm {
  padding-left: 0;
  padding-right: 0;
}
.input-sm {
  height: 30px;
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
}
select.input-sm {
  height: 30px;
  line-height: 30px;
}
textarea.input-sm,
select[multiple].input-sm {
  height: auto;
}
.form-group-sm .form-control {
  height: 30px;
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
}
.form-group-sm select.form-control {
  height: 30px;
  line-height: 30px;
}
.form-group-sm textarea.form-control,
.form-group-sm select[multiple].form-control {
  height: auto;
}
.form-group-sm .form-control-static {
  height: 30px;
  min-height: 30px;
  padding: 6px 10px;
  font-size: 12px;
  line-height: 1.5;
}
.input-lg {
  height: 45px;
  padding: 10px 16px;
  font-size: 17px;
  line-height: 1.3333333;
  border-radius: 3px;
}
select.input-lg {
  height: 45px;
  line-height: 45px;
}
textarea.input-lg,
select[multiple].input-lg {
  height: auto;
}
.form-group-lg .form-control {
  height: 45px;
  padding: 10px 16px;
  font-size: 17px;
  line-height: 1.3333333;
  border-radius: 3px;
}
.form-group-lg select.form-control {
  height: 45px;
  line-height: 45px;
}
.form-group-lg textarea.form-control,
.form-group-lg select[multiple].form-control {
  height: auto;
}
.form-group-lg .form-control-static {
  height: 45px;
  min-height: 35px;
  padding: 11px 16px;
  font-size: 17px;
  line-height: 1.3333333;
}
.has-feedback {
  position: relative;
}
.has-feedback .form-control {
  padding-right: 40px;
}
.form-control-feedback {
  position: absolute;
  top: 0;
  right: 0;
  z-index: 2;
  display: block;
  width: 32px;
  height: 32px;
  line-height: 32px;
  text-align: center;
  pointer-events: none;
}
.input-lg + .form-control-feedback,
.input-group-lg + .form-control-feedback,
.form-group-lg .form-control + .form-control-feedback {
  width: 45px;
  height: 45px;
  line-height: 45px;
}
.input-sm + .form-control-feedback,
.input-group-sm + .form-control-feedback,
.form-group-sm .form-control + .form-control-feedback {
  width: 30px;
  height: 30px;
  line-height: 30px;
}
.has-success .help-block,
.has-success .control-label,
.has-success .radio,
.has-success .checkbox,
.has-success .radio-inline,
.has-success .checkbox-inline,
.has-success.radio label,
.has-success.checkbox label,
.has-success.radio-inline label,
.has-success.checkbox-inline label {
  color: #3c763d;
}
.has-success .form-control {
  border-color: #3c763d;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
}
.has-success .form-control:focus {
  border-color: #2b542c;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #67b168;
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #67b168;
}
.has-success .input-group-addon {
  color: #3c763d;
  border-color: #3c763d;
  background-color: #dff0d8;
}
.has-success .form-control-feedback {
  color: #3c763d;
}
.has-warning .help-block,
.has-warning .control-label,
.has-warning .radio,
.has-warning .checkbox,
.has-warning .radio-inline,
.has-warning .checkbox-inline,
.has-warning.radio label,
.has-warning.checkbox label,
.has-warning.radio-inline label,
.has-warning.checkbox-inline label {
  color: #8a6d3b;
}
.has-warning .form-control {
  border-color: #8a6d3b;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
}
.has-warning .form-control:focus {
  border-color: #66512c;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #c0a16b;
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #c0a16b;
}
.has-warning .input-group-addon {
  color: #8a6d3b;
  border-color: #8a6d3b;
  background-color: #fcf8e3;
}
.has-warning .form-control-feedback {
  color: #8a6d3b;
}
.has-error .help-block,
.has-error .control-label,
.has-error .radio,
.has-error .checkbox,
.has-error .radio-inline,
.has-error .checkbox-inline,
.has-error.radio label,
.has-error.checkbox label,
.has-error.radio-inline label,
.has-error.checkbox-inline label {
  color: #a94442;
}
.has-error .form-control {
  border-color: #a94442;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
}
.has-error .form-control:focus {
  border-color: #843534;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #ce8483;
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #ce8483;
}
.has-error .input-group-addon {
  color: #a94442;
  border-color: #a94442;
  background-color: #f2dede;
}
.has-error .form-control-feedback {
  color: #a94442;
}
.has-feedback label ~ .form-control-feedback {
  top: 23px;
}
.has-feedback label.sr-only ~ .form-control-feedback {
  top: 0;
}
.help-block {
  display: block;
  margin-top: 5px;
  margin-bottom: 10px;
  color: #404040;
}
@media (min-width: 768px) {
  .form-inline .form-group {
    display: inline-block;
    margin-bottom: 0;
    vertical-align: middle;
  }
  .form-inline .form-control {
    display: inline-block;
    width: auto;
    vertical-align: middle;
  }
  .form-inline .form-control-static {
    display: inline-block;
  }
  .form-inline .input-group {
    display: inline-table;
    vertical-align: middle;
  }
  .form-inline .input-group .input-group-addon,
  .form-inline .input-group .input-group-btn,
  .form-inline .input-group .form-control {
    width: auto;
  }
  .form-inline .input-group > .form-control {
    width: 100%;
  }
  .form-inline .control-label {
    margin-bottom: 0;
    vertical-align: middle;
  }
  .form-inline .radio,
  .form-inline .checkbox {
    display: inline-block;
    margin-top: 0;
    margin-bottom: 0;
    vertical-align: middle;
  }
  .form-inline .radio label,
  .form-inline .checkbox label {
    padding-left: 0;
  }
  .form-inline .radio input[type="radio"],
  .form-inline .checkbox input[type="checkbox"] {
    position: relative;
    margin-left: 0;
  }
  .form-inline .has-feedback .form-control-feedback {
    top: 0;
  }
}
.form-horizontal .radio,
.form-horizontal .checkbox,
.form-horizontal .radio-inline,
.form-horizontal .checkbox-inline {
  margin-top: 0;
  margin-bottom: 0;
  padding-top: 7px;
}
.form-horizontal .radio,
.form-horizontal .checkbox {
  min-height: 25px;
}
.form-horizontal .form-group {
  margin-left: 0px;
  margin-right: 0px;
}
@media (min-width: 768px) {
  .form-horizontal .control-label {
    text-align: right;
    margin-bottom: 0;
    padding-top: 7px;
  }
}
.form-horizontal .has-feedback .form-control-feedback {
  right: 0px;
}
@media (min-width: 768px) {
  .form-horizontal .form-group-lg .control-label {
    padding-top: 11px;
    font-size: 17px;
  }
}
@media (min-width: 768px) {
  .form-horizontal .form-group-sm .control-label {
    padding-top: 6px;
    font-size: 12px;
  }
}
.btn {
  display: inline-block;
  margin-bottom: 0;
  font-weight: normal;
  text-align: center;
  vertical-align: middle;
  touch-action: manipulation;
  cursor: pointer;
  background-image: none;
  border: 1px solid transparent;
  white-space: nowrap;
  padding: 6px 12px;
  font-size: 13px;
  line-height: 1.42857143;
  border-radius: 2px;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}
.btn:focus,
.btn:active:focus,
.btn.active:focus,
.btn.focus,
.btn:active.focus,
.btn.active.focus {
  outline: 5px auto -webkit-focus-ring-color;
  outline-offset: -2px;
}
.btn:hover,
.btn:focus,
.btn.focus {
  color: #333;
  text-decoration: none;
}
.btn:active,
.btn.active {
  outline: 0;
  background-image: none;
  -webkit-box-shadow: inset 0 3px 5px rgba(0, 0, 0, 0.125);
  box-shadow: inset 0 3px 5px rgba(0, 0, 0, 0.125);
}
.btn.disabled,
.btn[disabled],
fieldset[disabled] .btn {
  cursor: not-allowed;
  opacity: 0.65;
  filter: alpha(opacity=65);
  -webkit-box-shadow: none;
  box-shadow: none;
}
a.btn.disabled,
fieldset[disabled] a.btn {
  pointer-events: none;
}
.btn-default {
  color: #333;
  background-color: #fff;
  border-color: #ccc;
}
.btn-default:focus,
.btn-default.focus {
  color: #333;
  background-color: #e6e6e6;
  border-color: #8c8c8c;
}
.btn-default:hover {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
.btn-default:active,
.btn-default.active,
.open > .dropdown-toggle.btn-default {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
.btn-default:active:hover,
.btn-default.active:hover,
.open > .dropdown-toggle.btn-default:hover,
.btn-default:active:focus,
.btn-default.active:focus,
.open > .dropdown-toggle.btn-default:focus,
.btn-default:active.focus,
.btn-default.active.focus,
.open > .dropdown-toggle.btn-default.focus {
  color: #333;
  background-color: #d4d4d4;
  border-color: #8c8c8c;
}
.btn-default:active,
.btn-default.active,
.open > .dropdown-toggle.btn-default {
  background-image: none;
}
.btn-default.disabled:hover,
.btn-default[disabled]:hover,
fieldset[disabled] .btn-default:hover,
.btn-default.disabled:focus,
.btn-default[disabled]:focus,
fieldset[disabled] .btn-default:focus,
.btn-default.disabled.focus,
.btn-default[disabled].focus,
fieldset[disabled] .btn-default.focus {
  background-color: #fff;
  border-color: #ccc;
}
.btn-default .badge {
  color: #fff;
  background-color: #333;
}
.btn-primary {
  color: #fff;
  background-color: #337ab7;
  border-color: #2e6da4;
}
.btn-primary:focus,
.btn-primary.focus {
  color: #fff;
  background-color: #286090;
  border-color: #122b40;
}
.btn-primary:hover {
  color: #fff;
  background-color: #286090;
  border-color: #204d74;
}
.btn-primary:active,
.btn-primary.active,
.open > .dropdown-toggle.btn-primary {
  color: #fff;
  background-color: #286090;
  border-color: #204d74;
}
.btn-primary:active:hover,
.btn-primary.active:hover,
.open > .dropdown-toggle.btn-primary:hover,
.btn-primary:active:focus,
.btn-primary.active:focus,
.open > .dropdown-toggle.btn-primary:focus,
.btn-primary:active.focus,
.btn-primary.active.focus,
.open > .dropdown-toggle.btn-primary.focus {
  color: #fff;
  background-color: #204d74;
  border-color: #122b40;
}
.btn-primary:active,
.btn-primary.active,
.open > .dropdown-toggle.btn-primary {
  background-image: none;
}
.btn-primary.disabled:hover,
.btn-primary[disabled]:hover,
fieldset[disabled] .btn-primary:hover,
.btn-primary.disabled:focus,
.btn-primary[disabled]:focus,
fieldset[disabled] .btn-primary:focus,
.btn-primary.disabled.focus,
.btn-primary[disabled].focus,
fieldset[disabled] .btn-primary.focus {
  background-color: #337ab7;
  border-color: #2e6da4;
}
.btn-primary .badge {
  color: #337ab7;
  background-color: #fff;
}
.btn-success {
  color: #fff;
  background-color: #5cb85c;
  border-color: #4cae4c;
}
.btn-success:focus,
.btn-success.focus {
  color: #fff;
  background-color: #449d44;
  border-color: #255625;
}
.btn-success:hover {
  color: #fff;
  background-color: #449d44;
  border-color: #398439;
}
.btn-success:active,
.btn-success.active,
.open > .dropdown-toggle.btn-success {
  color: #fff;
  background-color: #449d44;
  border-color: #398439;
}
.btn-success:active:hover,
.btn-success.active:hover,
.open > .dropdown-toggle.btn-success:hover,
.btn-success:active:focus,
.btn-success.active:focus,
.open > .dropdown-toggle.btn-success:focus,
.btn-success:active.focus,
.btn-success.active.focus,
.open > .dropdown-toggle.btn-success.focus {
  color: #fff;
  background-color: #398439;
  border-color: #255625;
}
.btn-success:active,
.btn-success.active,
.open > .dropdown-toggle.btn-success {
  background-image: none;
}
.btn-success.disabled:hover,
.btn-success[disabled]:hover,
fieldset[disabled] .btn-success:hover,
.btn-success.disabled:focus,
.btn-success[disabled]:focus,
fieldset[disabled] .btn-success:focus,
.btn-success.disabled.focus,
.btn-success[disabled].focus,
fieldset[disabled] .btn-success.focus {
  background-color: #5cb85c;
  border-color: #4cae4c;
}
.btn-success .badge {
  color: #5cb85c;
  background-color: #fff;
}
.btn-info {
  color: #fff;
  background-color: #5bc0de;
  border-color: #46b8da;
}
.btn-info:focus,
.btn-info.focus {
  color: #fff;
  background-color: #31b0d5;
  border-color: #1b6d85;
}
.btn-info:hover {
  color: #fff;
  background-color: #31b0d5;
  border-color: #269abc;
}
.btn-info:active,
.btn-info.active,
.open > .dropdown-toggle.btn-info {
  color: #fff;
  background-color: #31b0d5;
  border-color: #269abc;
}
.btn-info:active:hover,
.btn-info.active:hover,
.open > .dropdown-toggle.btn-info:hover,
.btn-info:active:focus,
.btn-info.active:focus,
.open > .dropdown-toggle.btn-info:focus,
.btn-info:active.focus,
.btn-info.active.focus,
.open > .dropdown-toggle.btn-info.focus {
  color: #fff;
  background-color: #269abc;
  border-color: #1b6d85;
}
.btn-info:active,
.btn-info.active,
.open > .dropdown-toggle.btn-info {
  background-image: none;
}
.btn-info.disabled:hover,
.btn-info[disabled]:hover,
fieldset[disabled] .btn-info:hover,
.btn-info.disabled:focus,
.btn-info[disabled]:focus,
fieldset[disabled] .btn-info:focus,
.btn-info.disabled.focus,
.btn-info[disabled].focus,
fieldset[disabled] .btn-info.focus {
  background-color: #5bc0de;
  border-color: #46b8da;
}
.btn-info .badge {
  color: #5bc0de;
  background-color: #fff;
}
.btn-warning {
  color: #fff;
  background-color: #f0ad4e;
  border-color: #eea236;
}
.btn-warning:focus,
.btn-warning.focus {
  color: #fff;
  background-color: #ec971f;
  border-color: #985f0d;
}
.btn-warning:hover {
  color: #fff;
  background-color: #ec971f;
  border-color: #d58512;
}
.btn-warning:active,
.btn-warning.active,
.open > .dropdown-toggle.btn-warning {
  color: #fff;
  background-color: #ec971f;
  border-color: #d58512;
}
.btn-warning:active:hover,
.btn-warning.active:hover,
.open > .dropdown-toggle.btn-warning:hover,
.btn-warning:active:focus,
.btn-warning.active:focus,
.open > .dropdown-toggle.btn-warning:focus,
.btn-warning:active.focus,
.btn-warning.active.focus,
.open > .dropdown-toggle.btn-warning.focus {
  color: #fff;
  background-color: #d58512;
  border-color: #985f0d;
}
.btn-warning:active,
.btn-warning.active,
.open > .dropdown-toggle.btn-warning {
  background-image: none;
}
.btn-warning.disabled:hover,
.btn-warning[disabled]:hover,
fieldset[disabled] .btn-warning:hover,
.btn-warning.disabled:focus,
.btn-warning[disabled]:focus,
fieldset[disabled] .btn-warning:focus,
.btn-warning.disabled.focus,
.btn-warning[disabled].focus,
fieldset[disabled] .btn-warning.focus {
  background-color: #f0ad4e;
  border-color: #eea236;
}
.btn-warning .badge {
  color: #f0ad4e;
  background-color: #fff;
}
.btn-danger {
  color: #fff;
  background-color: #d9534f;
  border-color: #d43f3a;
}
.btn-danger:focus,
.btn-danger.focus {
  color: #fff;
  background-color: #c9302c;
  border-color: #761c19;
}
.btn-danger:hover {
  color: #fff;
  background-color: #c9302c;
  border-color: #ac2925;
}
.btn-danger:active,
.btn-danger.active,
.open > .dropdown-toggle.btn-danger {
  color: #fff;
  background-color: #c9302c;
  border-color: #ac2925;
}
.btn-danger:active:hover,
.btn-danger.active:hover,
.open > .dropdown-toggle.btn-danger:hover,
.btn-danger:active:focus,
.btn-danger.active:focus,
.open > .dropdown-toggle.btn-danger:focus,
.btn-danger:active.focus,
.btn-danger.active.focus,
.open > .dropdown-toggle.btn-danger.focus {
  color: #fff;
  background-color: #ac2925;
  border-color: #761c19;
}
.btn-danger:active,
.btn-danger.active,
.open > .dropdown-toggle.btn-danger {
  background-image: none;
}
.btn-danger.disabled:hover,
.btn-danger[disabled]:hover,
fieldset[disabled] .btn-danger:hover,
.btn-danger.disabled:focus,
.btn-danger[disabled]:focus,
fieldset[disabled] .btn-danger:focus,
.btn-danger.disabled.focus,
.btn-danger[disabled].focus,
fieldset[disabled] .btn-danger.focus {
  background-color: #d9534f;
  border-color: #d43f3a;
}
.btn-danger .badge {
  color: #d9534f;
  background-color: #fff;
}
.btn-link {
  color: #337ab7;
  font-weight: normal;
  border-radius: 0;
}
.btn-link,
.btn-link:active,
.btn-link.active,
.btn-link[disabled],
fieldset[disabled] .btn-link {
  background-color: transparent;
  -webkit-box-shadow: none;
  box-shadow: none;
}
.btn-link,
.btn-link:hover,
.btn-link:focus,
.btn-link:active {
  border-color: transparent;
}
.btn-link:hover,
.btn-link:focus {
  color: #23527c;
  text-decoration: underline;
  background-color: transparent;
}
.btn-link[disabled]:hover,
fieldset[disabled] .btn-link:hover,
.btn-link[disabled]:focus,
fieldset[disabled] .btn-link:focus {
  color: #777777;
  text-decoration: none;
}
.btn-lg,
.btn-group-lg > .btn {
  padding: 10px 16px;
  font-size: 17px;
  line-height: 1.3333333;
  border-radius: 3px;
}
.btn-sm,
.btn-group-sm > .btn {
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
}
.btn-xs,
.btn-group-xs > .btn {
  padding: 1px 5px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
}
.btn-block {
  display: block;
  width: 100%;
}
.btn-block + .btn-block {
  margin-top: 5px;
}
input[type="submit"].btn-block,
input[type="reset"].btn-block,
input[type="button"].btn-block {
  width: 100%;
}
.fade {
  opacity: 0;
  -webkit-transition: opacity 0.15s linear;
  -o-transition: opacity 0.15s linear;
  transition: opacity 0.15s linear;
}
.fade.in {
  opacity: 1;
}
.collapse {
  display: none;
}
.collapse.in {
  display: block;
}
tr.collapse.in {
  display: table-row;
}
tbody.collapse.in {
  display: table-row-group;
}
.collapsing {
  position: relative;
  height: 0;
  overflow: hidden;
  -webkit-transition-property: height, visibility;
  transition-property: height, visibility;
  -webkit-transition-duration: 0.35s;
  transition-duration: 0.35s;
  -webkit-transition-timing-function: ease;
  transition-timing-function: ease;
}
.caret {
  display: inline-block;
  width: 0;
  height: 0;
  margin-left: 2px;
  vertical-align: middle;
  border-top: 4px dashed;
  border-top: 4px solid \9;
  border-right: 4px solid transparent;
  border-left: 4px solid transparent;
}
.dropup,
.dropdown {
  position: relative;
}
.dropdown-toggle:focus {
  outline: 0;
}
.dropdown-menu {
  position: absolute;
  top: 100%;
  left: 0;
  z-index: 1000;
  display: none;
  float: left;
  min-width: 160px;
  padding: 5px 0;
  margin: 2px 0 0;
  list-style: none;
  font-size: 13px;
  text-align: left;
  background-color: #fff;
  border: 1px solid #ccc;
  border: 1px solid rgba(0, 0, 0, 0.15);
  border-radius: 2px;
  -webkit-box-shadow: 0 6px 12px rgba(0, 0, 0, 0.175);
  box-shadow: 0 6px 12px rgba(0, 0, 0, 0.175);
  background-clip: padding-box;
}
.dropdown-menu.pull-right {
  right: 0;
  left: auto;
}
.dropdown-menu .divider {
  height: 1px;
  margin: 8px 0;
  overflow: hidden;
  background-color: #e5e5e5;
}
.dropdown-menu > li > a {
  display: block;
  padding: 3px 20px;
  clear: both;
  font-weight: normal;
  line-height: 1.42857143;
  color: #333333;
  white-space: nowrap;
}
.dropdown-menu > li > a:hover,
.dropdown-menu > li > a:focus {
  text-decoration: none;
  color: #262626;
  background-color: #f5f5f5;
}
.dropdown-menu > .active > a,
.dropdown-menu > .active > a:hover,
.dropdown-menu > .active > a:focus {
  color: #fff;
  text-decoration: none;
  outline: 0;
  background-color: #337ab7;
}
.dropdown-menu > .disabled > a,
.dropdown-menu > .disabled > a:hover,
.dropdown-menu > .disabled > a:focus {
  color: #777777;
}
.dropdown-menu > .disabled > a:hover,
.dropdown-menu > .disabled > a:focus {
  text-decoration: none;
  background-color: transparent;
  background-image: none;
  filter: progid:DXImageTransform.Microsoft.gradient(enabled = false);
  cursor: not-allowed;
}
.open > .dropdown-menu {
  display: block;
}
.open > a {
  outline: 0;
}
.dropdown-menu-right {
  left: auto;
  right: 0;
}
.dropdown-menu-left {
  left: 0;
  right: auto;
}
.dropdown-header {
  display: block;
  padding: 3px 20px;
  font-size: 12px;
  line-height: 1.42857143;
  color: #777777;
  white-space: nowrap;
}
.dropdown-backdrop {
  position: fixed;
  left: 0;
  right: 0;
  bottom: 0;
  top: 0;
  z-index: 990;
}
.pull-right > .dropdown-menu {
  right: 0;
  left: auto;
}
.dropup .caret,
.navbar-fixed-bottom .dropdown .caret {
  border-top: 0;
  border-bottom: 4px dashed;
  border-bottom: 4px solid \9;
  content: "";
}
.dropup .dropdown-menu,
.navbar-fixed-bottom .dropdown .dropdown-menu {
  top: auto;
  bottom: 100%;
  margin-bottom: 2px;
}
@media (min-width: 541px) {
  .navbar-right .dropdown-menu {
    left: auto;
    right: 0;
  }
  .navbar-right .dropdown-menu-left {
    left: 0;
    right: auto;
  }
}
.btn-group,
.btn-group-vertical {
  position: relative;
  display: inline-block;
  vertical-align: middle;
}
.btn-group > .btn,
.btn-group-vertical > .btn {
  position: relative;
  float: left;
}
.btn-group > .btn:hover,
.btn-group-vertical > .btn:hover,
.btn-group > .btn:focus,
.btn-group-vertical > .btn:focus,
.btn-group > .btn:active,
.btn-group-vertical > .btn:active,
.btn-group > .btn.active,
.btn-group-vertical > .btn.active {
  z-index: 2;
}
.btn-group .btn + .btn,
.btn-group .btn + .btn-group,
.btn-group .btn-group + .btn,
.btn-group .btn-group + .btn-group {
  margin-left: -1px;
}
.btn-toolbar {
  margin-left: -5px;
}
.btn-toolbar .btn,
.btn-toolbar .btn-group,
.btn-toolbar .input-group {
  float: left;
}
.btn-toolbar > .btn,
.btn-toolbar > .btn-group,
.btn-toolbar > .input-group {
  margin-left: 5px;
}
.btn-group > .btn:not(:first-child):not(:last-child):not(.dropdown-toggle) {
  border-radius: 0;
}
.btn-group > .btn:first-child {
  margin-left: 0;
}
.btn-group > .btn:first-child:not(:last-child):not(.dropdown-toggle) {
  border-bottom-right-radius: 0;
  border-top-right-radius: 0;
}
.btn-group > .btn:last-child:not(:first-child),
.btn-group > .dropdown-toggle:not(:first-child) {
  border-bottom-left-radius: 0;
  border-top-left-radius: 0;
}
.btn-group > .btn-group {
  float: left;
}
.btn-group > .btn-group:not(:first-child):not(:last-child) > .btn {
  border-radius: 0;
}
.btn-group > .btn-group:first-child:not(:last-child) > .btn:last-child,
.btn-group > .btn-group:first-child:not(:last-child) > .dropdown-toggle {
  border-bottom-right-radius: 0;
  border-top-right-radius: 0;
}
.btn-group > .btn-group:last-child:not(:first-child) > .btn:first-child {
  border-bottom-left-radius: 0;
  border-top-left-radius: 0;
}
.btn-group .dropdown-toggle:active,
.btn-group.open .dropdown-toggle {
  outline: 0;
}
.btn-group > .btn + .dropdown-toggle {
  padding-left: 8px;
  padding-right: 8px;
}
.btn-group > .btn-lg + .dropdown-toggle {
  padding-left: 12px;
  padding-right: 12px;
}
.btn-group.open .dropdown-toggle {
  -webkit-box-shadow: inset 0 3px 5px rgba(0, 0, 0, 0.125);
  box-shadow: inset 0 3px 5px rgba(0, 0, 0, 0.125);
}
.btn-group.open .dropdown-toggle.btn-link {
  -webkit-box-shadow: none;
  box-shadow: none;
}
.btn .caret {
  margin-left: 0;
}
.btn-lg .caret {
  border-width: 5px 5px 0;
  border-bottom-width: 0;
}
.dropup .btn-lg .caret {
  border-width: 0 5px 5px;
}
.btn-group-vertical > .btn,
.btn-group-vertical > .btn-group,
.btn-group-vertical > .btn-group > .btn {
  display: block;
  float: none;
  width: 100%;
  max-width: 100%;
}
.btn-group-vertical > .btn-group > .btn {
  float: none;
}
.btn-group-vertical > .btn + .btn,
.btn-group-vertical > .btn + .btn-group,
.btn-group-vertical > .btn-group + .btn,
.btn-group-vertical > .btn-group + .btn-group {
  margin-top: -1px;
  margin-left: 0;
}
.btn-group-vertical > .btn:not(:first-child):not(:last-child) {
  border-radius: 0;
}
.btn-group-vertical > .btn:first-child:not(:last-child) {
  border-top-right-radius: 2px;
  border-top-left-radius: 2px;
  border-bottom-right-radius: 0;
  border-bottom-left-radius: 0;
}
.btn-group-vertical > .btn:last-child:not(:first-child) {
  border-top-right-radius: 0;
  border-top-left-radius: 0;
  border-bottom-right-radius: 2px;
  border-bottom-left-radius: 2px;
}
.btn-group-vertical > .btn-group:not(:first-child):not(:last-child) > .btn {
  border-radius: 0;
}
.btn-group-vertical > .btn-group:first-child:not(:last-child) > .btn:last-child,
.btn-group-vertical > .btn-group:first-child:not(:last-child) > .dropdown-toggle {
  border-bottom-right-radius: 0;
  border-bottom-left-radius: 0;
}
.btn-group-vertical > .btn-group:last-child:not(:first-child) > .btn:first-child {
  border-top-right-radius: 0;
  border-top-left-radius: 0;
}
.btn-group-justified {
  display: table;
  width: 100%;
  table-layout: fixed;
  border-collapse: separate;
}
.btn-group-justified > .btn,
.btn-group-justified > .btn-group {
  float: none;
  display: table-cell;
  width: 1%;
}
.btn-group-justified > .btn-group .btn {
  width: 100%;
}
.btn-group-justified > .btn-group .dropdown-menu {
  left: auto;
}
[data-toggle="buttons"] > .btn input[type="radio"],
[data-toggle="buttons"] > .btn-group > .btn input[type="radio"],
[data-toggle="buttons"] > .btn input[type="checkbox"],
[data-toggle="buttons"] > .btn-group > .btn input[type="checkbox"] {
  position: absolute;
  clip: rect(0, 0, 0, 0);
  pointer-events: none;
}
.input-group {
  position: relative;
  display: table;
  border-collapse: separate;
}
.input-group[class*="col-"] {
  float: none;
  padding-left: 0;
  padding-right: 0;
}
.input-group .form-control {
  position: relative;
  z-index: 2;
  float: left;
  width: 100%;
  margin-bottom: 0;
}
.input-group .form-control:focus {
  z-index: 3;
}
.input-group-lg > .form-control,
.input-group-lg > .input-group-addon,
.input-group-lg > .input-group-btn > .btn {
  height: 45px;
  padding: 10px 16px;
  font-size: 17px;
  line-height: 1.3333333;
  border-radius: 3px;
}
select.input-group-lg > .form-control,
select.input-group-lg > .input-group-addon,
select.input-group-lg > .input-group-btn > .btn {
  height: 45px;
  line-height: 45px;
}
textarea.input-group-lg > .form-control,
textarea.input-group-lg > .input-group-addon,
textarea.input-group-lg > .input-group-btn > .btn,
select[multiple].input-group-lg > .form-control,
select[multiple].input-group-lg > .input-group-addon,
select[multiple].input-group-lg > .input-group-btn > .btn {
  height: auto;
}
.input-group-sm > .form-control,
.input-group-sm > .input-group-addon,
.input-group-sm > .input-group-btn > .btn {
  height: 30px;
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
}
select.input-group-sm > .form-control,
select.input-group-sm > .input-group-addon,
select.input-group-sm > .input-group-btn > .btn {
  height: 30px;
  line-height: 30px;
}
textarea.input-group-sm > .form-control,
textarea.input-group-sm > .input-group-addon,
textarea.input-group-sm > .input-group-btn > .btn,
select[multiple].input-group-sm > .form-control,
select[multiple].input-group-sm > .input-group-addon,
select[multiple].input-group-sm > .input-group-btn > .btn {
  height: auto;
}
.input-group-addon,
.input-group-btn,
.input-group .form-control {
  display: table-cell;
}
.input-group-addon:not(:first-child):not(:last-child),
.input-group-btn:not(:first-child):not(:last-child),
.input-group .form-control:not(:first-child):not(:last-child) {
  border-radius: 0;
}
.input-group-addon,
.input-group-btn {
  width: 1%;
  white-space: nowrap;
  vertical-align: middle;
}
.input-group-addon {
  padding: 6px 12px;
  font-size: 13px;
  font-weight: normal;
  line-height: 1;
  color: #555555;
  text-align: center;
  background-color: #eeeeee;
  border: 1px solid #ccc;
  border-radius: 2px;
}
.input-group-addon.input-sm {
  padding: 5px 10px;
  font-size: 12px;
  border-radius: 1px;
}
.input-group-addon.input-lg {
  padding: 10px 16px;
  font-size: 17px;
  border-radius: 3px;
}
.input-group-addon input[type="radio"],
.input-group-addon input[type="checkbox"] {
  margin-top: 0;
}
.input-group .form-control:first-child,
.input-group-addon:first-child,
.input-group-btn:first-child > .btn,
.input-group-btn:first-child > .btn-group > .btn,
.input-group-btn:first-child > .dropdown-toggle,
.input-group-btn:last-child > .btn:not(:last-child):not(.dropdown-toggle),
.input-group-btn:last-child > .btn-group:not(:last-child) > .btn {
  border-bottom-right-radius: 0;
  border-top-right-radius: 0;
}
.input-group-addon:first-child {
  border-right: 0;
}
.input-group .form-control:last-child,
.input-group-addon:last-child,
.input-group-btn:last-child > .btn,
.input-group-btn:last-child > .btn-group > .btn,
.input-group-btn:last-child > .dropdown-toggle,
.input-group-btn:first-child > .btn:not(:first-child),
.input-group-btn:first-child > .btn-group:not(:first-child) > .btn {
  border-bottom-left-radius: 0;
  border-top-left-radius: 0;
}
.input-group-addon:last-child {
  border-left: 0;
}
.input-group-btn {
  position: relative;
  font-size: 0;
  white-space: nowrap;
}
.input-group-btn > .btn {
  position: relative;
}
.input-group-btn > .btn + .btn {
  margin-left: -1px;
}
.input-group-btn > .btn:hover,
.input-group-btn > .btn:focus,
.input-group-btn > .btn:active {
  z-index: 2;
}
.input-group-btn:first-child > .btn,
.input-group-btn:first-child > .btn-group {
  margin-right: -1px;
}
.input-group-btn:last-child > .btn,
.input-group-btn:last-child > .btn-group {
  z-index: 2;
  margin-left: -1px;
}
.nav {
  margin-bottom: 0;
  padding-left: 0;
  list-style: none;
}
.nav > li {
  position: relative;
  display: block;
}
.nav > li > a {
  position: relative;
  display: block;
  padding: 10px 15px;
}
.nav > li > a:hover,
.nav > li > a:focus {
  text-decoration: none;
  background-color: #eeeeee;
}
.nav > li.disabled > a {
  color: #777777;
}
.nav > li.disabled > a:hover,
.nav > li.disabled > a:focus {
  color: #777777;
  text-decoration: none;
  background-color: transparent;
  cursor: not-allowed;
}
.nav .open > a,
.nav .open > a:hover,
.nav .open > a:focus {
  background-color: #eeeeee;
  border-color: #337ab7;
}
.nav .nav-divider {
  height: 1px;
  margin: 8px 0;
  overflow: hidden;
  background-color: #e5e5e5;
}
.nav > li > a > img {
  max-width: none;
}
.nav-tabs {
  border-bottom: 1px solid #ddd;
}
.nav-tabs > li {
  float: left;
  margin-bottom: -1px;
}
.nav-tabs > li > a {
  margin-right: 2px;
  line-height: 1.42857143;
  border: 1px solid transparent;
  border-radius: 2px 2px 0 0;
}
.nav-tabs > li > a:hover {
  border-color: #eeeeee #eeeeee #ddd;
}
.nav-tabs > li.active > a,
.nav-tabs > li.active > a:hover,
.nav-tabs > li.active > a:focus {
  color: #555555;
  background-color: #fff;
  border: 1px solid #ddd;
  border-bottom-color: transparent;
  cursor: default;
}
.nav-tabs.nav-justified {
  width: 100%;
  border-bottom: 0;
}
.nav-tabs.nav-justified > li {
  float: none;
}
.nav-tabs.nav-justified > li > a {
  text-align: center;
  margin-bottom: 5px;
}
.nav-tabs.nav-justified > .dropdown .dropdown-menu {
  top: auto;
  left: auto;
}
@media (min-width: 768px) {
  .nav-tabs.nav-justified > li {
    display: table-cell;
    width: 1%;
  }
  .nav-tabs.nav-justified > li > a {
    margin-bottom: 0;
  }
}
.nav-tabs.nav-justified > li > a {
  margin-right: 0;
  border-radius: 2px;
}
.nav-tabs.nav-justified > .active > a,
.nav-tabs.nav-justified > .active > a:hover,
.nav-tabs.nav-justified > .active > a:focus {
  border: 1px solid #ddd;
}
@media (min-width: 768px) {
  .nav-tabs.nav-justified > li > a {
    border-bottom: 1px solid #ddd;
    border-radius: 2px 2px 0 0;
  }
  .nav-tabs.nav-justified > .active > a,
  .nav-tabs.nav-justified > .active > a:hover,
  .nav-tabs.nav-justified > .active > a:focus {
    border-bottom-color: #fff;
  }
}
.nav-pills > li {
  float: left;
}
.nav-pills > li > a {
  border-radius: 2px;
}
.nav-pills > li + li {
  margin-left: 2px;
}
.nav-pills > li.active > a,
.nav-pills > li.active > a:hover,
.nav-pills > li.active > a:focus {
  color: #fff;
  background-color: #337ab7;
}
.nav-stacked > li {
  float: none;
}
.nav-stacked > li + li {
  margin-top: 2px;
  margin-left: 0;
}
.nav-justified {
  width: 100%;
}
.nav-justified > li {
  float: none;
}
.nav-justified > li > a {
  text-align: center;
  margin-bottom: 5px;
}
.nav-justified > .dropdown .dropdown-menu {
  top: auto;
  left: auto;
}
@media (min-width: 768px) {
  .nav-justified > li {
    display: table-cell;
    width: 1%;
  }
  .nav-justified > li > a {
    margin-bottom: 0;
  }
}
.nav-tabs-justified {
  border-bottom: 0;
}
.nav-tabs-justified > li > a {
  margin-right: 0;
  border-radius: 2px;
}
.nav-tabs-justified > .active > a,
.nav-tabs-justified > .active > a:hover,
.nav-tabs-justified > .active > a:focus {
  border: 1px solid #ddd;
}
@media (min-width: 768px) {
  .nav-tabs-justified > li > a {
    border-bottom: 1px solid #ddd;
    border-radius: 2px 2px 0 0;
  }
  .nav-tabs-justified > .active > a,
  .nav-tabs-justified > .active > a:hover,
  .nav-tabs-justified > .active > a:focus {
    border-bottom-color: #fff;
  }
}
.tab-content > .tab-pane {
  display: none;
}
.tab-content > .active {
  display: block;
}
.nav-tabs .dropdown-menu {
  margin-top: -1px;
  border-top-right-radius: 0;
  border-top-left-radius: 0;
}
.navbar {
  position: relative;
  min-height: 30px;
  margin-bottom: 18px;
  border: 1px solid transparent;
}
@media (min-width: 541px) {
  .navbar {
    border-radius: 2px;
  }
}
@media (min-width: 541px) {
  .navbar-header {
    float: left;
  }
}
.navbar-collapse {
  overflow-x: visible;
  padding-right: 0px;
  padding-left: 0px;
  border-top: 1px solid transparent;
  box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.1);
  -webkit-overflow-scrolling: touch;
}
.navbar-collapse.in {
  overflow-y: auto;
}
@media (min-width: 541px) {
  .navbar-collapse {
    width: auto;
    border-top: 0;
    box-shadow: none;
  }
  .navbar-collapse.collapse {
    display: block !important;
    height: auto !important;
    padding-bottom: 0;
    overflow: visible !important;
  }
  .navbar-collapse.in {
    overflow-y: visible;
  }
  .navbar-fixed-top .navbar-collapse,
  .navbar-static-top .navbar-collapse,
  .navbar-fixed-bottom .navbar-collapse {
    padding-left: 0;
    padding-right: 0;
  }
}
.navbar-fixed-top .navbar-collapse,
.navbar-fixed-bottom .navbar-collapse {
  max-height: 340px;
}
@media (max-device-width: 540px) and (orientation: landscape) {
  .navbar-fixed-top .navbar-collapse,
  .navbar-fixed-bottom .navbar-collapse {
    max-height: 200px;
  }
}
.container > .navbar-header,
.container-fluid > .navbar-header,
.container > .navbar-collapse,
.container-fluid > .navbar-collapse {
  margin-right: 0px;
  margin-left: 0px;
}
@media (min-width: 541px) {
  .container > .navbar-header,
  .container-fluid > .navbar-header,
  .container > .navbar-collapse,
  .container-fluid > .navbar-collapse {
    margin-right: 0;
    margin-left: 0;
  }
}
.navbar-static-top {
  z-index: 1000;
  border-width: 0 0 1px;
}
@media (min-width: 541px) {
  .navbar-static-top {
    border-radius: 0;
  }
}
.navbar-fixed-top,
.navbar-fixed-bottom {
  position: fixed;
  right: 0;
  left: 0;
  z-index: 1030;
}
@media (min-width: 541px) {
  .navbar-fixed-top,
  .navbar-fixed-bottom {
    border-radius: 0;
  }
}
.navbar-fixed-top {
  top: 0;
  border-width: 0 0 1px;
}
.navbar-fixed-bottom {
  bottom: 0;
  margin-bottom: 0;
  border-width: 1px 0 0;
}
.navbar-brand {
  float: left;
  padding: 6px 0px;
  font-size: 17px;
  line-height: 18px;
  height: 30px;
}
.navbar-brand:hover,
.navbar-brand:focus {
  text-decoration: none;
}
.navbar-brand > img {
  display: block;
}
@media (min-width: 541px) {
  .navbar > .container .navbar-brand,
  .navbar > .container-fluid .navbar-brand {
    margin-left: 0px;
  }
}
.navbar-toggle {
  position: relative;
  float: right;
  margin-right: 0px;
  padding: 9px 10px;
  margin-top: -2px;
  margin-bottom: -2px;
  background-color: transparent;
  background-image: none;
  border: 1px solid transparent;
  border-radius: 2px;
}
.navbar-toggle:focus {
  outline: 0;
}
.navbar-toggle .icon-bar {
  display: block;
  width: 22px;
  height: 2px;
  border-radius: 1px;
}
.navbar-toggle .icon-bar + .icon-bar {
  margin-top: 4px;
}
@media (min-width: 541px) {
  .navbar-toggle {
    display: none;
  }
}
.navbar-nav {
  margin: 3px 0px;
}
.navbar-nav > li > a {
  padding-top: 10px;
  padding-bottom: 10px;
  line-height: 18px;
}
@media (max-width: 540px) {
  .navbar-nav .open .dropdown-menu {
    position: static;
    float: none;
    width: auto;
    margin-top: 0;
    background-color: transparent;
    border: 0;
    box-shadow: none;
  }
  .navbar-nav .open .dropdown-menu > li > a,
  .navbar-nav .open .dropdown-menu .dropdown-header {
    padding: 5px 15px 5px 25px;
  }
  .navbar-nav .open .dropdown-menu > li > a {
    line-height: 18px;
  }
  .navbar-nav .open .dropdown-menu > li > a:hover,
  .navbar-nav .open .dropdown-menu > li > a:focus {
    background-image: none;
  }
}
@media (min-width: 541px) {
  .navbar-nav {
    float: left;
    margin: 0;
  }
  .navbar-nav > li {
    float: left;
  }
  .navbar-nav > li > a {
    padding-top: 6px;
    padding-bottom: 6px;
  }
}
.navbar-form {
  margin-left: 0px;
  margin-right: 0px;
  padding: 10px 0px;
  border-top: 1px solid transparent;
  border-bottom: 1px solid transparent;
  -webkit-box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.1), 0 1px 0 rgba(255, 255, 255, 0.1);
  box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.1), 0 1px 0 rgba(255, 255, 255, 0.1);
  margin-top: -1px;
  margin-bottom: -1px;
}
@media (min-width: 768px) {
  .navbar-form .form-group {
    display: inline-block;
    margin-bottom: 0;
    vertical-align: middle;
  }
  .navbar-form .form-control {
    display: inline-block;
    width: auto;
    vertical-align: middle;
  }
  .navbar-form .form-control-static {
    display: inline-block;
  }
  .navbar-form .input-group {
    display: inline-table;
    vertical-align: middle;
  }
  .navbar-form .input-group .input-group-addon,
  .navbar-form .input-group .input-group-btn,
  .navbar-form .input-group .form-control {
    width: auto;
  }
  .navbar-form .input-group > .form-control {
    width: 100%;
  }
  .navbar-form .control-label {
    margin-bottom: 0;
    vertical-align: middle;
  }
  .navbar-form .radio,
  .navbar-form .checkbox {
    display: inline-block;
    margin-top: 0;
    margin-bottom: 0;
    vertical-align: middle;
  }
  .navbar-form .radio label,
  .navbar-form .checkbox label {
    padding-left: 0;
  }
  .navbar-form .radio input[type="radio"],
  .navbar-form .checkbox input[type="checkbox"] {
    position: relative;
    margin-left: 0;
  }
  .navbar-form .has-feedback .form-control-feedback {
    top: 0;
  }
}
@media (max-width: 540px) {
  .navbar-form .form-group {
    margin-bottom: 5px;
  }
  .navbar-form .form-group:last-child {
    margin-bottom: 0;
  }
}
@media (min-width: 541px) {
  .navbar-form {
    width: auto;
    border: 0;
    margin-left: 0;
    margin-right: 0;
    padding-top: 0;
    padding-bottom: 0;
    -webkit-box-shadow: none;
    box-shadow: none;
  }
}
.navbar-nav > li > .dropdown-menu {
  margin-top: 0;
  border-top-right-radius: 0;
  border-top-left-radius: 0;
}
.navbar-fixed-bottom .navbar-nav > li > .dropdown-menu {
  margin-bottom: 0;
  border-top-right-radius: 2px;
  border-top-left-radius: 2px;
  border-bottom-right-radius: 0;
  border-bottom-left-radius: 0;
}
.navbar-btn {
  margin-top: -1px;
  margin-bottom: -1px;
}
.navbar-btn.btn-sm {
  margin-top: 0px;
  margin-bottom: 0px;
}
.navbar-btn.btn-xs {
  margin-top: 4px;
  margin-bottom: 4px;
}
.navbar-text {
  margin-top: 6px;
  margin-bottom: 6px;
}
@media (min-width: 541px) {
  .navbar-text {
    float: left;
    margin-left: 0px;
    margin-right: 0px;
  }
}
@media (min-width: 541px) {
  .navbar-left {
    float: left !important;
    float: left;
  }
  .navbar-right {
    float: right !important;
    float: right;
    margin-right: 0px;
  }
  .navbar-right ~ .navbar-right {
    margin-right: 0;
  }
}
.navbar-default {
  background-color: #f8f8f8;
  border-color: #e7e7e7;
}
.navbar-default .navbar-brand {
  color: #777;
}
.navbar-default .navbar-brand:hover,
.navbar-default .navbar-brand:focus {
  color: #5e5e5e;
  background-color: transparent;
}
.navbar-default .navbar-text {
  color: #777;
}
.navbar-default .navbar-nav > li > a {
  color: #777;
}
.navbar-default .navbar-nav > li > a:hover,
.navbar-default .navbar-nav > li > a:focus {
  color: #333;
  background-color: transparent;
}
.navbar-default .navbar-nav > .active > a,
.navbar-default .navbar-nav > .active > a:hover,
.navbar-default .navbar-nav > .active > a:focus {
  color: #555;
  background-color: #e7e7e7;
}
.navbar-default .navbar-nav > .disabled > a,
.navbar-default .navbar-nav > .disabled > a:hover,
.navbar-default .navbar-nav > .disabled > a:focus {
  color: #ccc;
  background-color: transparent;
}
.navbar-default .navbar-toggle {
  border-color: #ddd;
}
.navbar-default .navbar-toggle:hover,
.navbar-default .navbar-toggle:focus {
  background-color: #ddd;
}
.navbar-default .navbar-toggle .icon-bar {
  background-color: #888;
}
.navbar-default .navbar-collapse,
.navbar-default .navbar-form {
  border-color: #e7e7e7;
}
.navbar-default .navbar-nav > .open > a,
.navbar-default .navbar-nav > .open > a:hover,
.navbar-default .navbar-nav > .open > a:focus {
  background-color: #e7e7e7;
  color: #555;
}
@media (max-width: 540px) {
  .navbar-default .navbar-nav .open .dropdown-menu > li > a {
    color: #777;
  }
  .navbar-default .navbar-nav .open .dropdown-menu > li > a:hover,
  .navbar-default .navbar-nav .open .dropdown-menu > li > a:focus {
    color: #333;
    background-color: transparent;
  }
  .navbar-default .navbar-nav .open .dropdown-menu > .active > a,
  .navbar-default .navbar-nav .open .dropdown-menu > .active > a:hover,
  .navbar-default .navbar-nav .open .dropdown-menu > .active > a:focus {
    color: #555;
    background-color: #e7e7e7;
  }
  .navbar-default .navbar-nav .open .dropdown-menu > .disabled > a,
  .navbar-default .navbar-nav .open .dropdown-menu > .disabled > a:hover,
  .navbar-default .navbar-nav .open .dropdown-menu > .disabled > a:focus {
    color: #ccc;
    background-color: transparent;
  }
}
.navbar-default .navbar-link {
  color: #777;
}
.navbar-default .navbar-link:hover {
  color: #333;
}
.navbar-default .btn-link {
  color: #777;
}
.navbar-default .btn-link:hover,
.navbar-default .btn-link:focus {
  color: #333;
}
.navbar-default .btn-link[disabled]:hover,
fieldset[disabled] .navbar-default .btn-link:hover,
.navbar-default .btn-link[disabled]:focus,
fieldset[disabled] .navbar-default .btn-link:focus {
  color: #ccc;
}
.navbar-inverse {
  background-color: #222;
  border-color: #080808;
}
.navbar-inverse .navbar-brand {
  color: #9d9d9d;
}
.navbar-inverse .navbar-brand:hover,
.navbar-inverse .navbar-brand:focus {
  color: #fff;
  background-color: transparent;
}
.navbar-inverse .navbar-text {
  color: #9d9d9d;
}
.navbar-inverse .navbar-nav > li > a {
  color: #9d9d9d;
}
.navbar-inverse .navbar-nav > li > a:hover,
.navbar-inverse .navbar-nav > li > a:focus {
  color: #fff;
  background-color: transparent;
}
.navbar-inverse .navbar-nav > .active > a,
.navbar-inverse .navbar-nav > .active > a:hover,
.navbar-inverse .navbar-nav > .active > a:focus {
  color: #fff;
  background-color: #080808;
}
.navbar-inverse .navbar-nav > .disabled > a,
.navbar-inverse .navbar-nav > .disabled > a:hover,
.navbar-inverse .navbar-nav > .disabled > a:focus {
  color: #444;
  background-color: transparent;
}
.navbar-inverse .navbar-toggle {
  border-color: #333;
}
.navbar-inverse .navbar-toggle:hover,
.navbar-inverse .navbar-toggle:focus {
  background-color: #333;
}
.navbar-inverse .navbar-toggle .icon-bar {
  background-color: #fff;
}
.navbar-inverse .navbar-collapse,
.navbar-inverse .navbar-form {
  border-color: #101010;
}
.navbar-inverse .navbar-nav > .open > a,
.navbar-inverse .navbar-nav > .open > a:hover,
.navbar-inverse .navbar-nav > .open > a:focus {
  background-color: #080808;
  color: #fff;
}
@media (max-width: 540px) {
  .navbar-inverse .navbar-nav .open .dropdown-menu > .dropdown-header {
    border-color: #080808;
  }
  .navbar-inverse .navbar-nav .open .dropdown-menu .divider {
    background-color: #080808;
  }
  .navbar-inverse .navbar-nav .open .dropdown-menu > li > a {
    color: #9d9d9d;
  }
  .navbar-inverse .navbar-nav .open .dropdown-menu > li > a:hover,
  .navbar-inverse .navbar-nav .open .dropdown-menu > li > a:focus {
    color: #fff;
    background-color: transparent;
  }
  .navbar-inverse .navbar-nav .open .dropdown-menu > .active > a,
  .navbar-inverse .navbar-nav .open .dropdown-menu > .active > a:hover,
  .navbar-inverse .navbar-nav .open .dropdown-menu > .active > a:focus {
    color: #fff;
    background-color: #080808;
  }
  .navbar-inverse .navbar-nav .open .dropdown-menu > .disabled > a,
  .navbar-inverse .navbar-nav .open .dropdown-menu > .disabled > a:hover,
  .navbar-inverse .navbar-nav .open .dropdown-menu > .disabled > a:focus {
    color: #444;
    background-color: transparent;
  }
}
.navbar-inverse .navbar-link {
  color: #9d9d9d;
}
.navbar-inverse .navbar-link:hover {
  color: #fff;
}
.navbar-inverse .btn-link {
  color: #9d9d9d;
}
.navbar-inverse .btn-link:hover,
.navbar-inverse .btn-link:focus {
  color: #fff;
}
.navbar-inverse .btn-link[disabled]:hover,
fieldset[disabled] .navbar-inverse .btn-link:hover,
.navbar-inverse .btn-link[disabled]:focus,
fieldset[disabled] .navbar-inverse .btn-link:focus {
  color: #444;
}
.breadcrumb {
  padding: 8px 15px;
  margin-bottom: 18px;
  list-style: none;
  background-color: #f5f5f5;
  border-radius: 2px;
}
.breadcrumb > li {
  display: inline-block;
}
.breadcrumb > li + li:before {
  content: "/\00a0";
  padding: 0 5px;
  color: #5e5e5e;
}
.breadcrumb > .active {
  color: #777777;
}
.pagination {
  display: inline-block;
  padding-left: 0;
  margin: 18px 0;
  border-radius: 2px;
}
.pagination > li {
  display: inline;
}
.pagination > li > a,
.pagination > li > span {
  position: relative;
  float: left;
  padding: 6px 12px;
  line-height: 1.42857143;
  text-decoration: none;
  color: #337ab7;
  background-color: #fff;
  border: 1px solid #ddd;
  margin-left: -1px;
}
.pagination > li:first-child > a,
.pagination > li:first-child > span {
  margin-left: 0;
  border-bottom-left-radius: 2px;
  border-top-left-radius: 2px;
}
.pagination > li:last-child > a,
.pagination > li:last-child > span {
  border-bottom-right-radius: 2px;
  border-top-right-radius: 2px;
}
.pagination > li > a:hover,
.pagination > li > span:hover,
.pagination > li > a:focus,
.pagination > li > span:focus {
  z-index: 2;
  color: #23527c;
  background-color: #eeeeee;
  border-color: #ddd;
}
.pagination > .active > a,
.pagination > .active > span,
.pagination > .active > a:hover,
.pagination > .active > span:hover,
.pagination > .active > a:focus,
.pagination > .active > span:focus {
  z-index: 3;
  color: #fff;
  background-color: #337ab7;
  border-color: #337ab7;
  cursor: default;
}
.pagination > .disabled > span,
.pagination > .disabled > span:hover,
.pagination > .disabled > span:focus,
.pagination > .disabled > a,
.pagination > .disabled > a:hover,
.pagination > .disabled > a:focus {
  color: #777777;
  background-color: #fff;
  border-color: #ddd;
  cursor: not-allowed;
}
.pagination-lg > li > a,
.pagination-lg > li > span {
  padding: 10px 16px;
  font-size: 17px;
  line-height: 1.3333333;
}
.pagination-lg > li:first-child > a,
.pagination-lg > li:first-child > span {
  border-bottom-left-radius: 3px;
  border-top-left-radius: 3px;
}
.pagination-lg > li:last-child > a,
.pagination-lg > li:last-child > span {
  border-bottom-right-radius: 3px;
  border-top-right-radius: 3px;
}
.pagination-sm > li > a,
.pagination-sm > li > span {
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
}
.pagination-sm > li:first-child > a,
.pagination-sm > li:first-child > span {
  border-bottom-left-radius: 1px;
  border-top-left-radius: 1px;
}
.pagination-sm > li:last-child > a,
.pagination-sm > li:last-child > span {
  border-bottom-right-radius: 1px;
  border-top-right-radius: 1px;
}
.pager {
  padding-left: 0;
  margin: 18px 0;
  list-style: none;
  text-align: center;
}
.pager li {
  display: inline;
}
.pager li > a,
.pager li > span {
  display: inline-block;
  padding: 5px 14px;
  background-color: #fff;
  border: 1px solid #ddd;
  border-radius: 15px;
}
.pager li > a:hover,
.pager li > a:focus {
  text-decoration: none;
  background-color: #eeeeee;
}
.pager .next > a,
.pager .next > span {
  float: right;
}
.pager .previous > a,
.pager .previous > span {
  float: left;
}
.pager .disabled > a,
.pager .disabled > a:hover,
.pager .disabled > a:focus,
.pager .disabled > span {
  color: #777777;
  background-color: #fff;
  cursor: not-allowed;
}
.label {
  display: inline;
  padding: .2em .6em .3em;
  font-size: 75%;
  font-weight: bold;
  line-height: 1;
  color: #fff;
  text-align: center;
  white-space: nowrap;
  vertical-align: baseline;
  border-radius: .25em;
}
a.label:hover,
a.label:focus {
  color: #fff;
  text-decoration: none;
  cursor: pointer;
}
.label:empty {
  display: none;
}
.btn .label {
  position: relative;
  top: -1px;
}
.label-default {
  background-color: #777777;
}
.label-default[href]:hover,
.label-default[href]:focus {
  background-color: #5e5e5e;
}
.label-primary {
  background-color: #337ab7;
}
.label-primary[href]:hover,
.label-primary[href]:focus {
  background-color: #286090;
}
.label-success {
  background-color: #5cb85c;
}
.label-success[href]:hover,
.label-success[href]:focus {
  background-color: #449d44;
}
.label-info {
  background-color: #5bc0de;
}
.label-info[href]:hover,
.label-info[href]:focus {
  background-color: #31b0d5;
}
.label-warning {
  background-color: #f0ad4e;
}
.label-warning[href]:hover,
.label-warning[href]:focus {
  background-color: #ec971f;
}
.label-danger {
  background-color: #d9534f;
}
.label-danger[href]:hover,
.label-danger[href]:focus {
  background-color: #c9302c;
}
.badge {
  display: inline-block;
  min-width: 10px;
  padding: 3px 7px;
  font-size: 12px;
  font-weight: bold;
  color: #fff;
  line-height: 1;
  vertical-align: middle;
  white-space: nowrap;
  text-align: center;
  background-color: #777777;
  border-radius: 10px;
}
.badge:empty {
  display: none;
}
.btn .badge {
  position: relative;
  top: -1px;
}
.btn-xs .badge,
.btn-group-xs > .btn .badge {
  top: 0;
  padding: 1px 5px;
}
a.badge:hover,
a.badge:focus {
  color: #fff;
  text-decoration: none;
  cursor: pointer;
}
.list-group-item.active > .badge,
.nav-pills > .active > a > .badge {
  color: #337ab7;
  background-color: #fff;
}
.list-group-item > .badge {
  float: right;
}
.list-group-item > .badge + .badge {
  margin-right: 5px;
}
.nav-pills > li > a > .badge {
  margin-left: 3px;
}
.jumbotron {
  padding-top: 30px;
  padding-bottom: 30px;
  margin-bottom: 30px;
  color: inherit;
  background-color: #eeeeee;
}
.jumbotron h1,
.jumbotron .h1 {
  color: inherit;
}
.jumbotron p {
  margin-bottom: 15px;
  font-size: 20px;
  font-weight: 200;
}
.jumbotron > hr {
  border-top-color: #d5d5d5;
}
.container .jumbotron,
.container-fluid .jumbotron {
  border-radius: 3px;
  padding-left: 0px;
  padding-right: 0px;
}
.jumbotron .container {
  max-width: 100%;
}
@media screen and (min-width: 768px) {
  .jumbotron {
    padding-top: 48px;
    padding-bottom: 48px;
  }
  .container .jumbotron,
  .container-fluid .jumbotron {
    padding-left: 60px;
    padding-right: 60px;
  }
  .jumbotron h1,
  .jumbotron .h1 {
    font-size: 59px;
  }
}
.thumbnail {
  display: block;
  padding: 4px;
  margin-bottom: 18px;
  line-height: 1.42857143;
  background-color: #fff;
  border: 1px solid #ddd;
  border-radius: 2px;
  -webkit-transition: border 0.2s ease-in-out;
  -o-transition: border 0.2s ease-in-out;
  transition: border 0.2s ease-in-out;
}
.thumbnail > img,
.thumbnail a > img {
  margin-left: auto;
  margin-right: auto;
}
a.thumbnail:hover,
a.thumbnail:focus,
a.thumbnail.active {
  border-color: #337ab7;
}
.thumbnail .caption {
  padding: 9px;
  color: #000;
}
.alert {
  padding: 15px;
  margin-bottom: 18px;
  border: 1px solid transparent;
  border-radius: 2px;
}
.alert h4 {
  margin-top: 0;
  color: inherit;
}
.alert .alert-link {
  font-weight: bold;
}
.alert > p,
.alert > ul {
  margin-bottom: 0;
}
.alert > p + p {
  margin-top: 5px;
}
.alert-dismissable,
.alert-dismissible {
  padding-right: 35px;
}
.alert-dismissable .close,
.alert-dismissible .close {
  position: relative;
  top: -2px;
  right: -21px;
  color: inherit;
}
.alert-success {
  background-color: #dff0d8;
  border-color: #d6e9c6;
  color: #3c763d;
}
.alert-success hr {
  border-top-color: #c9e2b3;
}
.alert-success .alert-link {
  color: #2b542c;
}
.alert-info {
  background-color: #d9edf7;
  border-color: #bce8f1;
  color: #31708f;
}
.alert-info hr {
  border-top-color: #a6e1ec;
}
.alert-info .alert-link {
  color: #245269;
}
.alert-warning {
  background-color: #fcf8e3;
  border-color: #faebcc;
  color: #8a6d3b;
}
.alert-warning hr {
  border-top-color: #f7e1b5;
}
.alert-warning .alert-link {
  color: #66512c;
}
.alert-danger {
  background-color: #f2dede;
  border-color: #ebccd1;
  color: #a94442;
}
.alert-danger hr {
  border-top-color: #e4b9c0;
}
.alert-danger .alert-link {
  color: #843534;
}
@-webkit-keyframes progress-bar-stripes {
  from {
    background-position: 40px 0;
  }
  to {
    background-position: 0 0;
  }
}
@keyframes progress-bar-stripes {
  from {
    background-position: 40px 0;
  }
  to {
    background-position: 0 0;
  }
}
.progress {
  overflow: hidden;
  height: 18px;
  margin-bottom: 18px;
  background-color: #f5f5f5;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 1px 2px rgba(0, 0, 0, 0.1);
  box-shadow: inset 0 1px 2px rgba(0, 0, 0, 0.1);
}
.progress-bar {
  float: left;
  width: 0%;
  height: 100%;
  font-size: 12px;
  line-height: 18px;
  color: #fff;
  text-align: center;
  background-color: #337ab7;
  -webkit-box-shadow: inset 0 -1px 0 rgba(0, 0, 0, 0.15);
  box-shadow: inset 0 -1px 0 rgba(0, 0, 0, 0.15);
  -webkit-transition: width 0.6s ease;
  -o-transition: width 0.6s ease;
  transition: width 0.6s ease;
}
.progress-striped .progress-bar,
.progress-bar-striped {
  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-size: 40px 40px;
}
.progress.active .progress-bar,
.progress-bar.active {
  -webkit-animation: progress-bar-stripes 2s linear infinite;
  -o-animation: progress-bar-stripes 2s linear infinite;
  animation: progress-bar-stripes 2s linear infinite;
}
.progress-bar-success {
  background-color: #5cb85c;
}
.progress-striped .progress-bar-success {
  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
}
.progress-bar-info {
  background-color: #5bc0de;
}
.progress-striped .progress-bar-info {
  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
}
.progress-bar-warning {
  background-color: #f0ad4e;
}
.progress-striped .progress-bar-warning {
  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
}
.progress-bar-danger {
  background-color: #d9534f;
}
.progress-striped .progress-bar-danger {
  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
}
.media {
  margin-top: 15px;
}
.media:first-child {
  margin-top: 0;
}
.media,
.media-body {
  zoom: 1;
  overflow: hidden;
}
.media-body {
  width: 10000px;
}
.media-object {
  display: block;
}
.media-object.img-thumbnail {
  max-width: none;
}
.media-right,
.media > .pull-right {
  padding-left: 10px;
}
.media-left,
.media > .pull-left {
  padding-right: 10px;
}
.media-left,
.media-right,
.media-body {
  display: table-cell;
  vertical-align: top;
}
.media-middle {
  vertical-align: middle;
}
.media-bottom {
  vertical-align: bottom;
}
.media-heading {
  margin-top: 0;
  margin-bottom: 5px;
}
.media-list {
  padding-left: 0;
  list-style: none;
}
.list-group {
  margin-bottom: 20px;
  padding-left: 0;
}
.list-group-item {
  position: relative;
  display: block;
  padding: 10px 15px;
  margin-bottom: -1px;
  background-color: #fff;
  border: 1px solid #ddd;
}
.list-group-item:first-child {
  border-top-right-radius: 2px;
  border-top-left-radius: 2px;
}
.list-group-item:last-child {
  margin-bottom: 0;
  border-bottom-right-radius: 2px;
  border-bottom-left-radius: 2px;
}
a.list-group-item,
button.list-group-item {
  color: #555;
}
a.list-group-item .list-group-item-heading,
button.list-group-item .list-group-item-heading {
  color: #333;
}
a.list-group-item:hover,
button.list-group-item:hover,
a.list-group-item:focus,
button.list-group-item:focus {
  text-decoration: none;
  color: #555;
  background-color: #f5f5f5;
}
button.list-group-item {
  width: 100%;
  text-align: left;
}
.list-group-item.disabled,
.list-group-item.disabled:hover,
.list-group-item.disabled:focus {
  background-color: #eeeeee;
  color: #777777;
  cursor: not-allowed;
}
.list-group-item.disabled .list-group-item-heading,
.list-group-item.disabled:hover .list-group-item-heading,
.list-group-item.disabled:focus .list-group-item-heading {
  color: inherit;
}
.list-group-item.disabled .list-group-item-text,
.list-group-item.disabled:hover .list-group-item-text,
.list-group-item.disabled:focus .list-group-item-text {
  color: #777777;
}
.list-group-item.active,
.list-group-item.active:hover,
.list-group-item.active:focus {
  z-index: 2;
  color: #fff;
  background-color: #337ab7;
  border-color: #337ab7;
}
.list-group-item.active .list-group-item-heading,
.list-group-item.active:hover .list-group-item-heading,
.list-group-item.active:focus .list-group-item-heading,
.list-group-item.active .list-group-item-heading > small,
.list-group-item.active:hover .list-group-item-heading > small,
.list-group-item.active:focus .list-group-item-heading > small,
.list-group-item.active .list-group-item-heading > .small,
.list-group-item.active:hover .list-group-item-heading > .small,
.list-group-item.active:focus .list-group-item-heading > .small {
  color: inherit;
}
.list-group-item.active .list-group-item-text,
.list-group-item.active:hover .list-group-item-text,
.list-group-item.active:focus .list-group-item-text {
  color: #c7ddef;
}
.list-group-item-success {
  color: #3c763d;
  background-color: #dff0d8;
}
a.list-group-item-success,
button.list-group-item-success {
  color: #3c763d;
}
a.list-group-item-success .list-group-item-heading,
button.list-group-item-success .list-group-item-heading {
  color: inherit;
}
a.list-group-item-success:hover,
button.list-group-item-success:hover,
a.list-group-item-success:focus,
button.list-group-item-success:focus {
  color: #3c763d;
  background-color: #d0e9c6;
}
a.list-group-item-success.active,
button.list-group-item-success.active,
a.list-group-item-success.active:hover,
button.list-group-item-success.active:hover,
a.list-group-item-success.active:focus,
button.list-group-item-success.active:focus {
  color: #fff;
  background-color: #3c763d;
  border-color: #3c763d;
}
.list-group-item-info {
  color: #31708f;
  background-color: #d9edf7;
}
a.list-group-item-info,
button.list-group-item-info {
  color: #31708f;
}
a.list-group-item-info .list-group-item-heading,
button.list-group-item-info .list-group-item-heading {
  color: inherit;
}
a.list-group-item-info:hover,
button.list-group-item-info:hover,
a.list-group-item-info:focus,
button.list-group-item-info:focus {
  color: #31708f;
  background-color: #c4e3f3;
}
a.list-group-item-info.active,
button.list-group-item-info.active,
a.list-group-item-info.active:hover,
button.list-group-item-info.active:hover,
a.list-group-item-info.active:focus,
button.list-group-item-info.active:focus {
  color: #fff;
  background-color: #31708f;
  border-color: #31708f;
}
.list-group-item-warning {
  color: #8a6d3b;
  background-color: #fcf8e3;
}
a.list-group-item-warning,
button.list-group-item-warning {
  color: #8a6d3b;
}
a.list-group-item-warning .list-group-item-heading,
button.list-group-item-warning .list-group-item-heading {
  color: inherit;
}
a.list-group-item-warning:hover,
button.list-group-item-warning:hover,
a.list-group-item-warning:focus,
button.list-group-item-warning:focus {
  color: #8a6d3b;
  background-color: #faf2cc;
}
a.list-group-item-warning.active,
button.list-group-item-warning.active,
a.list-group-item-warning.active:hover,
button.list-group-item-warning.active:hover,
a.list-group-item-warning.active:focus,
button.list-group-item-warning.active:focus {
  color: #fff;
  background-color: #8a6d3b;
  border-color: #8a6d3b;
}
.list-group-item-danger {
  color: #a94442;
  background-color: #f2dede;
}
a.list-group-item-danger,
button.list-group-item-danger {
  color: #a94442;
}
a.list-group-item-danger .list-group-item-heading,
button.list-group-item-danger .list-group-item-heading {
  color: inherit;
}
a.list-group-item-danger:hover,
button.list-group-item-danger:hover,
a.list-group-item-danger:focus,
button.list-group-item-danger:focus {
  color: #a94442;
  background-color: #ebcccc;
}
a.list-group-item-danger.active,
button.list-group-item-danger.active,
a.list-group-item-danger.active:hover,
button.list-group-item-danger.active:hover,
a.list-group-item-danger.active:focus,
button.list-group-item-danger.active:focus {
  color: #fff;
  background-color: #a94442;
  border-color: #a94442;
}
.list-group-item-heading {
  margin-top: 0;
  margin-bottom: 5px;
}
.list-group-item-text {
  margin-bottom: 0;
  line-height: 1.3;
}
.panel {
  margin-bottom: 18px;
  background-color: #fff;
  border: 1px solid transparent;
  border-radius: 2px;
  -webkit-box-shadow: 0 1px 1px rgba(0, 0, 0, 0.05);
  box-shadow: 0 1px 1px rgba(0, 0, 0, 0.05);
}
.panel-body {
  padding: 15px;
}
.panel-heading {
  padding: 10px 15px;
  border-bottom: 1px solid transparent;
  border-top-right-radius: 1px;
  border-top-left-radius: 1px;
}
.panel-heading > .dropdown .dropdown-toggle {
  color: inherit;
}
.panel-title {
  margin-top: 0;
  margin-bottom: 0;
  font-size: 15px;
  color: inherit;
}
.panel-title > a,
.panel-title > small,
.panel-title > .small,
.panel-title > small > a,
.panel-title > .small > a {
  color: inherit;
}
.panel-footer {
  padding: 10px 15px;
  background-color: #f5f5f5;
  border-top: 1px solid #ddd;
  border-bottom-right-radius: 1px;
  border-bottom-left-radius: 1px;
}
.panel > .list-group,
.panel > .panel-collapse > .list-group {
  margin-bottom: 0;
}
.panel > .list-group .list-group-item,
.panel > .panel-collapse > .list-group .list-group-item {
  border-width: 1px 0;
  border-radius: 0;
}
.panel > .list-group:first-child .list-group-item:first-child,
.panel > .panel-collapse > .list-group:first-child .list-group-item:first-child {
  border-top: 0;
  border-top-right-radius: 1px;
  border-top-left-radius: 1px;
}
.panel > .list-group:last-child .list-group-item:last-child,
.panel > .panel-collapse > .list-group:last-child .list-group-item:last-child {
  border-bottom: 0;
  border-bottom-right-radius: 1px;
  border-bottom-left-radius: 1px;
}
.panel > .panel-heading + .panel-collapse > .list-group .list-group-item:first-child {
  border-top-right-radius: 0;
  border-top-left-radius: 0;
}
.panel-heading + .list-group .list-group-item:first-child {
  border-top-width: 0;
}
.list-group + .panel-footer {
  border-top-width: 0;
}
.panel > .table,
.panel > .table-responsive > .table,
.panel > .panel-collapse > .table {
  margin-bottom: 0;
}
.panel > .table caption,
.panel > .table-responsive > .table caption,
.panel > .panel-collapse > .table caption {
  padding-left: 15px;
  padding-right: 15px;
}
.panel > .table:first-child,
.panel > .table-responsive:first-child > .table:first-child {
  border-top-right-radius: 1px;
  border-top-left-radius: 1px;
}
.panel > .table:first-child > thead:first-child > tr:first-child,
.panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child,
.panel > .table:first-child > tbody:first-child > tr:first-child,
.panel > .table-responsive:first-child > .table:first-child > tbody:first-child > tr:first-child {
  border-top-left-radius: 1px;
  border-top-right-radius: 1px;
}
.panel > .table:first-child > thead:first-child > tr:first-child td:first-child,
.panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child td:first-child,
.panel > .table:first-child > tbody:first-child > tr:first-child td:first-child,
.panel > .table-responsive:first-child > .table:first-child > tbody:first-child > tr:first-child td:first-child,
.panel > .table:first-child > thead:first-child > tr:first-child th:first-child,
.panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child th:first-child,
.panel > .table:first-child > tbody:first-child > tr:first-child th:first-child,
.panel > .table-responsive:first-child > .table:first-child > tbody:first-child > tr:first-child th:first-child {
  border-top-left-radius: 1px;
}
.panel > .table:first-child > thead:first-child > tr:first-child td:last-child,
.panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child td:last-child,
.panel > .table:first-child > tbody:first-child > tr:first-child td:last-child,
.panel > .table-responsive:first-child > .table:first-child > tbody:first-child > tr:first-child td:last-child,
.panel > .table:first-child > thead:first-child > tr:first-child th:last-child,
.panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child th:last-child,
.panel > .table:first-child > tbody:first-child > tr:first-child th:last-child,
.panel > .table-responsive:first-child > .table:first-child > tbody:first-child > tr:first-child th:last-child {
  border-top-right-radius: 1px;
}
.panel > .table:last-child,
.panel > .table-responsive:last-child > .table:last-child {
  border-bottom-right-radius: 1px;
  border-bottom-left-radius: 1px;
}
.panel > .table:last-child > tbody:last-child > tr:last-child,
.panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child,
.panel > .table:last-child > tfoot:last-child > tr:last-child,
.panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child {
  border-bottom-left-radius: 1px;
  border-bottom-right-radius: 1px;
}
.panel > .table:last-child > tbody:last-child > tr:last-child td:first-child,
.panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child td:first-child,
.panel > .table:last-child > tfoot:last-child > tr:last-child td:first-child,
.panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child td:first-child,
.panel > .table:last-child > tbody:last-child > tr:last-child th:first-child,
.panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child th:first-child,
.panel > .table:last-child > tfoot:last-child > tr:last-child th:first-child,
.panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child th:first-child {
  border-bottom-left-radius: 1px;
}
.panel > .table:last-child > tbody:last-child > tr:last-child td:last-child,
.panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child td:last-child,
.panel > .table:last-child > tfoot:last-child > tr:last-child td:last-child,
.panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child td:last-child,
.panel > .table:last-child > tbody:last-child > tr:last-child th:last-child,
.panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child th:last-child,
.panel > .table:last-child > tfoot:last-child > tr:last-child th:last-child,
.panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child th:last-child {
  border-bottom-right-radius: 1px;
}
.panel > .panel-body + .table,
.panel > .panel-body + .table-responsive,
.panel > .table + .panel-body,
.panel > .table-responsive + .panel-body {
  border-top: 1px solid #ddd;
}
.panel > .table > tbody:first-child > tr:first-child th,
.panel > .table > tbody:first-child > tr:first-child td {
  border-top: 0;
}
.panel > .table-bordered,
.panel > .table-responsive > .table-bordered {
  border: 0;
}
.panel > .table-bordered > thead > tr > th:first-child,
.panel > .table-responsive > .table-bordered > thead > tr > th:first-child,
.panel > .table-bordered > tbody > tr > th:first-child,
.panel > .table-responsive > .table-bordered > tbody > tr > th:first-child,
.panel > .table-bordered > tfoot > tr > th:first-child,
.panel > .table-responsive > .table-bordered > tfoot > tr > th:first-child,
.panel > .table-bordered > thead > tr > td:first-child,
.panel > .table-responsive > .table-bordered > thead > tr > td:first-child,
.panel > .table-bordered > tbody > tr > td:first-child,
.panel > .table-responsive > .table-bordered > tbody > tr > td:first-child,
.panel > .table-bordered > tfoot > tr > td:first-child,
.panel > .table-responsive > .table-bordered > tfoot > tr > td:first-child {
  border-left: 0;
}
.panel > .table-bordered > thead > tr > th:last-child,
.panel > .table-responsive > .table-bordered > thead > tr > th:last-child,
.panel > .table-bordered > tbody > tr > th:last-child,
.panel > .table-responsive > .table-bordered > tbody > tr > th:last-child,
.panel > .table-bordered > tfoot > tr > th:last-child,
.panel > .table-responsive > .table-bordered > tfoot > tr > th:last-child,
.panel > .table-bordered > thead > tr > td:last-child,
.panel > .table-responsive > .table-bordered > thead > tr > td:last-child,
.panel > .table-bordered > tbody > tr > td:last-child,
.panel > .table-responsive > .table-bordered > tbody > tr > td:last-child,
.panel > .table-bordered > tfoot > tr > td:last-child,
.panel > .table-responsive > .table-bordered > tfoot > tr > td:last-child {
  border-right: 0;
}
.panel > .table-bordered > thead > tr:first-child > td,
.panel > .table-responsive > .table-bordered > thead > tr:first-child > td,
.panel > .table-bordered > tbody > tr:first-child > td,
.panel > .table-responsive > .table-bordered > tbody > tr:first-child > td,
.panel > .table-bordered > thead > tr:first-child > th,
.panel > .table-responsive > .table-bordered > thead > tr:first-child > th,
.panel > .table-bordered > tbody > tr:first-child > th,
.panel > .table-responsive > .table-bordered > tbody > tr:first-child > th {
  border-bottom: 0;
}
.panel > .table-bordered > tbody > tr:last-child > td,
.panel > .table-responsive > .table-bordered > tbody > tr:last-child > td,
.panel > .table-bordered > tfoot > tr:last-child > td,
.panel > .table-responsive > .table-bordered > tfoot > tr:last-child > td,
.panel > .table-bordered > tbody > tr:last-child > th,
.panel > .table-responsive > .table-bordered > tbody > tr:last-child > th,
.panel > .table-bordered > tfoot > tr:last-child > th,
.panel > .table-responsive > .table-bordered > tfoot > tr:last-child > th {
  border-bottom: 0;
}
.panel > .table-responsive {
  border: 0;
  margin-bottom: 0;
}
.panel-group {
  margin-bottom: 18px;
}
.panel-group .panel {
  margin-bottom: 0;
  border-radius: 2px;
}
.panel-group .panel + .panel {
  margin-top: 5px;
}
.panel-group .panel-heading {
  border-bottom: 0;
}
.panel-group .panel-heading + .panel-collapse > .panel-body,
.panel-group .panel-heading + .panel-collapse > .list-group {
  border-top: 1px solid #ddd;
}
.panel-group .panel-footer {
  border-top: 0;
}
.panel-group .panel-footer + .panel-collapse .panel-body {
  border-bottom: 1px solid #ddd;
}
.panel-default {
  border-color: #ddd;
}
.panel-default > .panel-heading {
  color: #333333;
  background-color: #f5f5f5;
  border-color: #ddd;
}
.panel-default > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #ddd;
}
.panel-default > .panel-heading .badge {
  color: #f5f5f5;
  background-color: #333333;
}
.panel-default > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #ddd;
}
.panel-primary {
  border-color: #337ab7;
}
.panel-primary > .panel-heading {
  color: #fff;
  background-color: #337ab7;
  border-color: #337ab7;
}
.panel-primary > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #337ab7;
}
.panel-primary > .panel-heading .badge {
  color: #337ab7;
  background-color: #fff;
}
.panel-primary > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #337ab7;
}
.panel-success {
  border-color: #d6e9c6;
}
.panel-success > .panel-heading {
  color: #3c763d;
  background-color: #dff0d8;
  border-color: #d6e9c6;
}
.panel-success > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #d6e9c6;
}
.panel-success > .panel-heading .badge {
  color: #dff0d8;
  background-color: #3c763d;
}
.panel-success > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #d6e9c6;
}
.panel-info {
  border-color: #bce8f1;
}
.panel-info > .panel-heading {
  color: #31708f;
  background-color: #d9edf7;
  border-color: #bce8f1;
}
.panel-info > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #bce8f1;
}
.panel-info > .panel-heading .badge {
  color: #d9edf7;
  background-color: #31708f;
}
.panel-info > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #bce8f1;
}
.panel-warning {
  border-color: #faebcc;
}
.panel-warning > .panel-heading {
  color: #8a6d3b;
  background-color: #fcf8e3;
  border-color: #faebcc;
}
.panel-warning > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #faebcc;
}
.panel-warning > .panel-heading .badge {
  color: #fcf8e3;
  background-color: #8a6d3b;
}
.panel-warning > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #faebcc;
}
.panel-danger {
  border-color: #ebccd1;
}
.panel-danger > .panel-heading {
  color: #a94442;
  background-color: #f2dede;
  border-color: #ebccd1;
}
.panel-danger > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #ebccd1;
}
.panel-danger > .panel-heading .badge {
  color: #f2dede;
  background-color: #a94442;
}
.panel-danger > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #ebccd1;
}
.embed-responsive {
  position: relative;
  display: block;
  height: 0;
  padding: 0;
  overflow: hidden;
}
.embed-responsive .embed-responsive-item,
.embed-responsive iframe,
.embed-responsive embed,
.embed-responsive object,
.embed-responsive video {
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  height: 100%;
  width: 100%;
  border: 0;
}
.embed-responsive-16by9 {
  padding-bottom: 56.25%;
}
.embed-responsive-4by3 {
  padding-bottom: 75%;
}
.well {
  min-height: 20px;
  padding: 19px;
  margin-bottom: 20px;
  background-color: #f5f5f5;
  border: 1px solid #e3e3e3;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.05);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.05);
}
.well blockquote {
  border-color: #ddd;
  border-color: rgba(0, 0, 0, 0.15);
}
.well-lg {
  padding: 24px;
  border-radius: 3px;
}
.well-sm {
  padding: 9px;
  border-radius: 1px;
}
.close {
  float: right;
  font-size: 19.5px;
  font-weight: bold;
  line-height: 1;
  color: #000;
  text-shadow: 0 1px 0 #fff;
  opacity: 0.2;
  filter: alpha(opacity=20);
}
.close:hover,
.close:focus {
  color: #000;
  text-decoration: none;
  cursor: pointer;
  opacity: 0.5;
  filter: alpha(opacity=50);
}
button.close {
  padding: 0;
  cursor: pointer;
  background: transparent;
  border: 0;
  -webkit-appearance: none;
}
.modal-open {
  overflow: hidden;
}
.modal {
  display: none;
  overflow: hidden;
  position: fixed;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  z-index: 1050;
  -webkit-overflow-scrolling: touch;
  outline: 0;
}
.modal.fade .modal-dialog {
  -webkit-transform: translate(0, -25%);
  -ms-transform: translate(0, -25%);
  -o-transform: translate(0, -25%);
  transform: translate(0, -25%);
  -webkit-transition: -webkit-transform 0.3s ease-out;
  -moz-transition: -moz-transform 0.3s ease-out;
  -o-transition: -o-transform 0.3s ease-out;
  transition: transform 0.3s ease-out;
}
.modal.in .modal-dialog {
  -webkit-transform: translate(0, 0);
  -ms-transform: translate(0, 0);
  -o-transform: translate(0, 0);
  transform: translate(0, 0);
}
.modal-open .modal {
  overflow-x: hidden;
  overflow-y: auto;
}
.modal-dialog {
  position: relative;
  width: auto;
  margin: 10px;
}
.modal-content {
  position: relative;
  background-color: #fff;
  border: 1px solid #999;
  border: 1px solid rgba(0, 0, 0, 0.2);
  border-radius: 3px;
  -webkit-box-shadow: 0 3px 9px rgba(0, 0, 0, 0.5);
  box-shadow: 0 3px 9px rgba(0, 0, 0, 0.5);
  background-clip: padding-box;
  outline: 0;
}
.modal-backdrop {
  position: fixed;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  z-index: 1040;
  background-color: #000;
}
.modal-backdrop.fade {
  opacity: 0;
  filter: alpha(opacity=0);
}
.modal-backdrop.in {
  opacity: 0.5;
  filter: alpha(opacity=50);
}
.modal-header {
  padding: 15px;
  border-bottom: 1px solid #e5e5e5;
}
.modal-header .close {
  margin-top: -2px;
}
.modal-title {
  margin: 0;
  line-height: 1.42857143;
}
.modal-body {
  position: relative;
  padding: 15px;
}
.modal-footer {
  padding: 15px;
  text-align: right;
  border-top: 1px solid #e5e5e5;
}
.modal-footer .btn + .btn {
  margin-left: 5px;
  margin-bottom: 0;
}
.modal-footer .btn-group .btn + .btn {
  margin-left: -1px;
}
.modal-footer .btn-block + .btn-block {
  margin-left: 0;
}
.modal-scrollbar-measure {
  position: absolute;
  top: -9999px;
  width: 50px;
  height: 50px;
  overflow: scroll;
}
@media (min-width: 768px) {
  .modal-dialog {
    width: 600px;
    margin: 30px auto;
  }
  .modal-content {
    -webkit-box-shadow: 0 5px 15px rgba(0, 0, 0, 0.5);
    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.5);
  }
  .modal-sm {
    width: 300px;
  }
}
@media (min-width: 992px) {
  .modal-lg {
    width: 900px;
  }
}
.tooltip {
  position: absolute;
  z-index: 1070;
  display: block;
  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
  font-style: normal;
  font-weight: normal;
  letter-spacing: normal;
  line-break: auto;
  line-height: 1.42857143;
  text-align: left;
  text-align: start;
  text-decoration: none;
  text-shadow: none;
  text-transform: none;
  white-space: normal;
  word-break: normal;
  word-spacing: normal;
  word-wrap: normal;
  font-size: 12px;
  opacity: 0;
  filter: alpha(opacity=0);
}
.tooltip.in {
  opacity: 0.9;
  filter: alpha(opacity=90);
}
.tooltip.top {
  margin-top: -3px;
  padding: 5px 0;
}
.tooltip.right {
  margin-left: 3px;
  padding: 0 5px;
}
.tooltip.bottom {
  margin-top: 3px;
  padding: 5px 0;
}
.tooltip.left {
  margin-left: -3px;
  padding: 0 5px;
}
.tooltip-inner {
  max-width: 200px;
  padding: 3px 8px;
  color: #fff;
  text-align: center;
  background-color: #000;
  border-radius: 2px;
}
.tooltip-arrow {
  position: absolute;
  width: 0;
  height: 0;
  border-color: transparent;
  border-style: solid;
}
.tooltip.top .tooltip-arrow {
  bottom: 0;
  left: 50%;
  margin-left: -5px;
  border-width: 5px 5px 0;
  border-top-color: #000;
}
.tooltip.top-left .tooltip-arrow {
  bottom: 0;
  right: 5px;
  margin-bottom: -5px;
  border-width: 5px 5px 0;
  border-top-color: #000;
}
.tooltip.top-right .tooltip-arrow {
  bottom: 0;
  left: 5px;
  margin-bottom: -5px;
  border-width: 5px 5px 0;
  border-top-color: #000;
}
.tooltip.right .tooltip-arrow {
  top: 50%;
  left: 0;
  margin-top: -5px;
  border-width: 5px 5px 5px 0;
  border-right-color: #000;
}
.tooltip.left .tooltip-arrow {
  top: 50%;
  right: 0;
  margin-top: -5px;
  border-width: 5px 0 5px 5px;
  border-left-color: #000;
}
.tooltip.bottom .tooltip-arrow {
  top: 0;
  left: 50%;
  margin-left: -5px;
  border-width: 0 5px 5px;
  border-bottom-color: #000;
}
.tooltip.bottom-left .tooltip-arrow {
  top: 0;
  right: 5px;
  margin-top: -5px;
  border-width: 0 5px 5px;
  border-bottom-color: #000;
}
.tooltip.bottom-right .tooltip-arrow {
  top: 0;
  left: 5px;
  margin-top: -5px;
  border-width: 0 5px 5px;
  border-bottom-color: #000;
}
.popover {
  position: absolute;
  top: 0;
  left: 0;
  z-index: 1060;
  display: none;
  max-width: 276px;
  padding: 1px;
  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
  font-style: normal;
  font-weight: normal;
  letter-spacing: normal;
  line-break: auto;
  line-height: 1.42857143;
  text-align: left;
  text-align: start;
  text-decoration: none;
  text-shadow: none;
  text-transform: none;
  white-space: normal;
  word-break: normal;
  word-spacing: normal;
  word-wrap: normal;
  font-size: 13px;
  background-color: #fff;
  background-clip: padding-box;
  border: 1px solid #ccc;
  border: 1px solid rgba(0, 0, 0, 0.2);
  border-radius: 3px;
  -webkit-box-shadow: 0 5px 10px rgba(0, 0, 0, 0.2);
  box-shadow: 0 5px 10px rgba(0, 0, 0, 0.2);
}
.popover.top {
  margin-top: -10px;
}
.popover.right {
  margin-left: 10px;
}
.popover.bottom {
  margin-top: 10px;
}
.popover.left {
  margin-left: -10px;
}
.popover-title {
  margin: 0;
  padding: 8px 14px;
  font-size: 13px;
  background-color: #f7f7f7;
  border-bottom: 1px solid #ebebeb;
  border-radius: 2px 2px 0 0;
}
.popover-content {
  padding: 9px 14px;
}
.popover > .arrow,
.popover > .arrow:after {
  position: absolute;
  display: block;
  width: 0;
  height: 0;
  border-color: transparent;
  border-style: solid;
}
.popover > .arrow {
  border-width: 11px;
}
.popover > .arrow:after {
  border-width: 10px;
  content: "";
}
.popover.top > .arrow {
  left: 50%;
  margin-left: -11px;
  border-bottom-width: 0;
  border-top-color: #999999;
  border-top-color: rgba(0, 0, 0, 0.25);
  bottom: -11px;
}
.popover.top > .arrow:after {
  content: " ";
  bottom: 1px;
  margin-left: -10px;
  border-bottom-width: 0;
  border-top-color: #fff;
}
.popover.right > .arrow {
  top: 50%;
  left: -11px;
  margin-top: -11px;
  border-left-width: 0;
  border-right-color: #999999;
  border-right-color: rgba(0, 0, 0, 0.25);
}
.popover.right > .arrow:after {
  content: " ";
  left: 1px;
  bottom: -10px;
  border-left-width: 0;
  border-right-color: #fff;
}
.popover.bottom > .arrow {
  left: 50%;
  margin-left: -11px;
  border-top-width: 0;
  border-bottom-color: #999999;
  border-bottom-color: rgba(0, 0, 0, 0.25);
  top: -11px;
}
.popover.bottom > .arrow:after {
  content: " ";
  top: 1px;
  margin-left: -10px;
  border-top-width: 0;
  border-bottom-color: #fff;
}
.popover.left > .arrow {
  top: 50%;
  right: -11px;
  margin-top: -11px;
  border-right-width: 0;
  border-left-color: #999999;
  border-left-color: rgba(0, 0, 0, 0.25);
}
.popover.left > .arrow:after {
  content: " ";
  right: 1px;
  border-right-width: 0;
  border-left-color: #fff;
  bottom: -10px;
}
.carousel {
  position: relative;
}
.carousel-inner {
  position: relative;
  overflow: hidden;
  width: 100%;
}
.carousel-inner > .item {
  display: none;
  position: relative;
  -webkit-transition: 0.6s ease-in-out left;
  -o-transition: 0.6s ease-in-out left;
  transition: 0.6s ease-in-out left;
}
.carousel-inner > .item > img,
.carousel-inner > .item > a > img {
  line-height: 1;
}
@media all and (transform-3d), (-webkit-transform-3d) {
  .carousel-inner > .item {
    -webkit-transition: -webkit-transform 0.6s ease-in-out;
    -moz-transition: -moz-transform 0.6s ease-in-out;
    -o-transition: -o-transform 0.6s ease-in-out;
    transition: transform 0.6s ease-in-out;
    -webkit-backface-visibility: hidden;
    -moz-backface-visibility: hidden;
    backface-visibility: hidden;
    -webkit-perspective: 1000px;
    -moz-perspective: 1000px;
    perspective: 1000px;
  }
  .carousel-inner > .item.next,
  .carousel-inner > .item.active.right {
    -webkit-transform: translate3d(100%, 0, 0);
    transform: translate3d(100%, 0, 0);
    left: 0;
  }
  .carousel-inner > .item.prev,
  .carousel-inner > .item.active.left {
    -webkit-transform: translate3d(-100%, 0, 0);
    transform: translate3d(-100%, 0, 0);
    left: 0;
  }
  .carousel-inner > .item.next.left,
  .carousel-inner > .item.prev.right,
  .carousel-inner > .item.active {
    -webkit-transform: translate3d(0, 0, 0);
    transform: translate3d(0, 0, 0);
    left: 0;
  }
}
.carousel-inner > .active,
.carousel-inner > .next,
.carousel-inner > .prev {
  display: block;
}
.carousel-inner > .active {
  left: 0;
}
.carousel-inner > .next,
.carousel-inner > .prev {
  position: absolute;
  top: 0;
  width: 100%;
}
.carousel-inner > .next {
  left: 100%;
}
.carousel-inner > .prev {
  left: -100%;
}
.carousel-inner > .next.left,
.carousel-inner > .prev.right {
  left: 0;
}
.carousel-inner > .active.left {
  left: -100%;
}
.carousel-inner > .active.right {
  left: 100%;
}
.carousel-control {
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  width: 15%;
  opacity: 0.5;
  filter: alpha(opacity=50);
  font-size: 20px;
  color: #fff;
  text-align: center;
  text-shadow: 0 1px 2px rgba(0, 0, 0, 0.6);
  background-color: rgba(0, 0, 0, 0);
}
.carousel-control.left {
  background-image: -webkit-linear-gradient(left, rgba(0, 0, 0, 0.5) 0%, rgba(0, 0, 0, 0.0001) 100%);
  background-image: -o-linear-gradient(left, rgba(0, 0, 0, 0.5) 0%, rgba(0, 0, 0, 0.0001) 100%);
  background-image: linear-gradient(to right, rgba(0, 0, 0, 0.5) 0%, rgba(0, 0, 0, 0.0001) 100%);
  background-repeat: repeat-x;
  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#80000000', endColorstr='#00000000', GradientType=1);
}
.carousel-control.right {
  left: auto;
  right: 0;
  background-image: -webkit-linear-gradient(left, rgba(0, 0, 0, 0.0001) 0%, rgba(0, 0, 0, 0.5) 100%);
  background-image: -o-linear-gradient(left, rgba(0, 0, 0, 0.0001) 0%, rgba(0, 0, 0, 0.5) 100%);
  background-image: linear-gradient(to right, rgba(0, 0, 0, 0.0001) 0%, rgba(0, 0, 0, 0.5) 100%);
  background-repeat: repeat-x;
  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#00000000', endColorstr='#80000000', GradientType=1);
}
.carousel-control:hover,
.carousel-control:focus {
  outline: 0;
  color: #fff;
  text-decoration: none;
  opacity: 0.9;
  filter: alpha(opacity=90);
}
.carousel-control .icon-prev,
.carousel-control .icon-next,
.carousel-control .glyphicon-chevron-left,
.carousel-control .glyphicon-chevron-right {
  position: absolute;
  top: 50%;
  margin-top: -10px;
  z-index: 5;
  display: inline-block;
}
.carousel-control .icon-prev,
.carousel-control .glyphicon-chevron-left {
  left: 50%;
  margin-left: -10px;
}
.carousel-control .icon-next,
.carousel-control .glyphicon-chevron-right {
  right: 50%;
  margin-right: -10px;
}
.carousel-control .icon-prev,
.carousel-control .icon-next {
  width: 20px;
  height: 20px;
  line-height: 1;
  font-family: serif;
}
.carousel-control .icon-prev:before {
  content: '\2039';
}
.carousel-control .icon-next:before {
  content: '\203a';
}
.carousel-indicators {
  position: absolute;
  bottom: 10px;
  left: 50%;
  z-index: 15;
  width: 60%;
  margin-left: -30%;
  padding-left: 0;
  list-style: none;
  text-align: center;
}
.carousel-indicators li {
  display: inline-block;
  width: 10px;
  height: 10px;
  margin: 1px;
  text-indent: -999px;
  border: 1px solid #fff;
  border-radius: 10px;
  cursor: pointer;
  background-color: #000 \9;
  background-color: rgba(0, 0, 0, 0);
}
.carousel-indicators .active {
  margin: 0;
  width: 12px;
  height: 12px;
  background-color: #fff;
}
.carousel-caption {
  position: absolute;
  left: 15%;
  right: 15%;
  bottom: 20px;
  z-index: 10;
  padding-top: 20px;
  padding-bottom: 20px;
  color: #fff;
  text-align: center;
  text-shadow: 0 1px 2px rgba(0, 0, 0, 0.6);
}
.carousel-caption .btn {
  text-shadow: none;
}
@media screen and (min-width: 768px) {
  .carousel-control .glyphicon-chevron-left,
  .carousel-control .glyphicon-chevron-right,
  .carousel-control .icon-prev,
  .carousel-control .icon-next {
    width: 30px;
    height: 30px;
    margin-top: -10px;
    font-size: 30px;
  }
  .carousel-control .glyphicon-chevron-left,
  .carousel-control .icon-prev {
    margin-left: -10px;
  }
  .carousel-control .glyphicon-chevron-right,
  .carousel-control .icon-next {
    margin-right: -10px;
  }
  .carousel-caption {
    left: 20%;
    right: 20%;
    padding-bottom: 30px;
  }
  .carousel-indicators {
    bottom: 20px;
  }
}
.clearfix:before,
.clearfix:after,
.dl-horizontal dd:before,
.dl-horizontal dd:after,
.container:before,
.container:after,
.container-fluid:before,
.container-fluid:after,
.row:before,
.row:after,
.form-horizontal .form-group:before,
.form-horizontal .form-group:after,
.btn-toolbar:before,
.btn-toolbar:after,
.btn-group-vertical > .btn-group:before,
.btn-group-vertical > .btn-group:after,
.nav:before,
.nav:after,
.navbar:before,
.navbar:after,
.navbar-header:before,
.navbar-header:after,
.navbar-collapse:before,
.navbar-collapse:after,
.pager:before,
.pager:after,
.panel-body:before,
.panel-body:after,
.modal-header:before,
.modal-header:after,
.modal-footer:before,
.modal-footer:after,
.item_buttons:before,
.item_buttons:after {
  content: " ";
  display: table;
}
.clearfix:after,
.dl-horizontal dd:after,
.container:after,
.container-fluid:after,
.row:after,
.form-horizontal .form-group:after,
.btn-toolbar:after,
.btn-group-vertical > .btn-group:after,
.nav:after,
.navbar:after,
.navbar-header:after,
.navbar-collapse:after,
.pager:after,
.panel-body:after,
.modal-header:after,
.modal-footer:after,
.item_buttons:after {
  clear: both;
}
.center-block {
  display: block;
  margin-left: auto;
  margin-right: auto;
}
.pull-right {
  float: right !important;
}
.pull-left {
  float: left !important;
}
.hide {
  display: none !important;
}
.show {
  display: block !important;
}
.invisible {
  visibility: hidden;
}
.text-hide {
  font: 0/0 a;
  color: transparent;
  text-shadow: none;
  background-color: transparent;
  border: 0;
}
.hidden {
  display: none !important;
}
.affix {
  position: fixed;
}
@-ms-viewport {
  width: device-width;
}
.visible-xs,
.visible-sm,
.visible-md,
.visible-lg {
  display: none !important;
}
.visible-xs-block,
.visible-xs-inline,
.visible-xs-inline-block,
.visible-sm-block,
.visible-sm-inline,
.visible-sm-inline-block,
.visible-md-block,
.visible-md-inline,
.visible-md-inline-block,
.visible-lg-block,
.visible-lg-inline,
.visible-lg-inline-block {
  display: none !important;
}
@media (max-width: 767px) {
  .visible-xs {
    display: block !important;
  }
  table.visible-xs {
    display: table !important;
  }
  tr.visible-xs {
    display: table-row !important;
  }
  th.visible-xs,
  td.visible-xs {
    display: table-cell !important;
  }
}
@media (max-width: 767px) {
  .visible-xs-block {
    display: block !important;
  }
}
@media (max-width: 767px) {
  .visible-xs-inline {
    display: inline !important;
  }
}
@media (max-width: 767px) {
  .visible-xs-inline-block {
    display: inline-block !important;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  .visible-sm {
    display: block !important;
  }
  table.visible-sm {
    display: table !important;
  }
  tr.visible-sm {
    display: table-row !important;
  }
  th.visible-sm,
  td.visible-sm {
    display: table-cell !important;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  .visible-sm-block {
    display: block !important;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  .visible-sm-inline {
    display: inline !important;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  .visible-sm-inline-block {
    display: inline-block !important;
  }
}
@media (min-width: 992px) and (max-width: 1199px) {
  .visible-md {
    display: block !important;
  }
  table.visible-md {
    display: table !important;
  }
  tr.visible-md {
    display: table-row !important;
  }
  th.visible-md,
  td.visible-md {
    display: table-cell !important;
  }
}
@media (min-width: 992px) and (max-width: 1199px) {
  .visible-md-block {
    display: block !important;
  }
}
@media (min-width: 992px) and (max-width: 1199px) {
  .visible-md-inline {
    display: inline !important;
  }
}
@media (min-width: 992px) and (max-width: 1199px) {
  .visible-md-inline-block {
    display: inline-block !important;
  }
}
@media (min-width: 1200px) {
  .visible-lg {
    display: block !important;
  }
  table.visible-lg {
    display: table !important;
  }
  tr.visible-lg {
    display: table-row !important;
  }
  th.visible-lg,
  td.visible-lg {
    display: table-cell !important;
  }
}
@media (min-width: 1200px) {
  .visible-lg-block {
    display: block !important;
  }
}
@media (min-width: 1200px) {
  .visible-lg-inline {
    display: inline !important;
  }
}
@media (min-width: 1200px) {
  .visible-lg-inline-block {
    display: inline-block !important;
  }
}
@media (max-width: 767px) {
  .hidden-xs {
    display: none !important;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  .hidden-sm {
    display: none !important;
  }
}
@media (min-width: 992px) and (max-width: 1199px) {
  .hidden-md {
    display: none !important;
  }
}
@media (min-width: 1200px) {
  .hidden-lg {
    display: none !important;
  }
}
.visible-print {
  display: none !important;
}
@media print {
  .visible-print {
    display: block !important;
  }
  table.visible-print {
    display: table !important;
  }
  tr.visible-print {
    display: table-row !important;
  }
  th.visible-print,
  td.visible-print {
    display: table-cell !important;
  }
}
.visible-print-block {
  display: none !important;
}
@media print {
  .visible-print-block {
    display: block !important;
  }
}
.visible-print-inline {
  display: none !important;
}
@media print {
  .visible-print-inline {
    display: inline !important;
  }
}
.visible-print-inline-block {
  display: none !important;
}
@media print {
  .visible-print-inline-block {
    display: inline-block !important;
  }
}
@media print {
  .hidden-print {
    display: none !important;
  }
}
/*!
*
* Font Awesome
*
*/
/*!
 *  Font Awesome 4.7.0 by @davegandy - http://fontawesome.io - @fontawesome
 *  License - http://fontawesome.io/license (Font: SIL OFL 1.1, CSS: MIT License)
 */
/* FONT PATH
 * -------------------------- */
@font-face {
  font-family: 'FontAwesome';
  src: url('../components/font-awesome/fonts/fontawesome-webfont.eot?v=4.7.0');
  src: url('../components/font-awesome/fonts/fontawesome-webfont.eot?#iefix&v=4.7.0') format('embedded-opentype'), url('../components/font-awesome/fonts/fontawesome-webfont.woff2?v=4.7.0') format('woff2'), url('../components/font-awesome/fonts/fontawesome-webfont.woff?v=4.7.0') format('woff'), url('../components/font-awesome/fonts/fontawesome-webfont.ttf?v=4.7.0') format('truetype'), url('../components/font-awesome/fonts/fontawesome-webfont.svg?v=4.7.0#fontawesomeregular') format('svg');
  font-weight: normal;
  font-style: normal;
}
.fa {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
/* makes the font 33% larger relative to the icon container */
.fa-lg {
  font-size: 1.33333333em;
  line-height: 0.75em;
  vertical-align: -15%;
}
.fa-2x {
  font-size: 2em;
}
.fa-3x {
  font-size: 3em;
}
.fa-4x {
  font-size: 4em;
}
.fa-5x {
  font-size: 5em;
}
.fa-fw {
  width: 1.28571429em;
  text-align: center;
}
.fa-ul {
  padding-left: 0;
  margin-left: 2.14285714em;
  list-style-type: none;
}
.fa-ul > li {
  position: relative;
}
.fa-li {
  position: absolute;
  left: -2.14285714em;
  width: 2.14285714em;
  top: 0.14285714em;
  text-align: center;
}
.fa-li.fa-lg {
  left: -1.85714286em;
}
.fa-border {
  padding: .2em .25em .15em;
  border: solid 0.08em #eee;
  border-radius: .1em;
}
.fa-pull-left {
  float: left;
}
.fa-pull-right {
  float: right;
}
.fa.fa-pull-left {
  margin-right: .3em;
}
.fa.fa-pull-right {
  margin-left: .3em;
}
/* Deprecated as of 4.4.0 */
.pull-right {
  float: right;
}
.pull-left {
  float: left;
}
.fa.pull-left {
  margin-right: .3em;
}
.fa.pull-right {
  margin-left: .3em;
}
.fa-spin {
  -webkit-animation: fa-spin 2s infinite linear;
  animation: fa-spin 2s infinite linear;
}
.fa-pulse {
  -webkit-animation: fa-spin 1s infinite steps(8);
  animation: fa-spin 1s infinite steps(8);
}
@-webkit-keyframes fa-spin {
  0% {
    -webkit-transform: rotate(0deg);
    transform: rotate(0deg);
  }
  100% {
    -webkit-transform: rotate(359deg);
    transform: rotate(359deg);
  }
}
@keyframes fa-spin {
  0% {
    -webkit-transform: rotate(0deg);
    transform: rotate(0deg);
  }
  100% {
    -webkit-transform: rotate(359deg);
    transform: rotate(359deg);
  }
}
.fa-rotate-90 {
  -ms-filter: "progid:DXImageTransform.Microsoft.BasicImage(rotation=1)";
  -webkit-transform: rotate(90deg);
  -ms-transform: rotate(90deg);
  transform: rotate(90deg);
}
.fa-rotate-180 {
  -ms-filter: "progid:DXImageTransform.Microsoft.BasicImage(rotation=2)";
  -webkit-transform: rotate(180deg);
  -ms-transform: rotate(180deg);
  transform: rotate(180deg);
}
.fa-rotate-270 {
  -ms-filter: "progid:DXImageTransform.Microsoft.BasicImage(rotation=3)";
  -webkit-transform: rotate(270deg);
  -ms-transform: rotate(270deg);
  transform: rotate(270deg);
}
.fa-flip-horizontal {
  -ms-filter: "progid:DXImageTransform.Microsoft.BasicImage(rotation=0, mirror=1)";
  -webkit-transform: scale(-1, 1);
  -ms-transform: scale(-1, 1);
  transform: scale(-1, 1);
}
.fa-flip-vertical {
  -ms-filter: "progid:DXImageTransform.Microsoft.BasicImage(rotation=2, mirror=1)";
  -webkit-transform: scale(1, -1);
  -ms-transform: scale(1, -1);
  transform: scale(1, -1);
}
:root .fa-rotate-90,
:root .fa-rotate-180,
:root .fa-rotate-270,
:root .fa-flip-horizontal,
:root .fa-flip-vertical {
  filter: none;
}
.fa-stack {
  position: relative;
  display: inline-block;
  width: 2em;
  height: 2em;
  line-height: 2em;
  vertical-align: middle;
}
.fa-stack-1x,
.fa-stack-2x {
  position: absolute;
  left: 0;
  width: 100%;
  text-align: center;
}
.fa-stack-1x {
  line-height: inherit;
}
.fa-stack-2x {
  font-size: 2em;
}
.fa-inverse {
  color: #fff;
}
/* Font Awesome uses the Unicode Private Use Area (PUA) to ensure screen
   readers do not read off random characters that represent icons */
.fa-glass:before {
  content: "\f000";
}
.fa-music:before {
  content: "\f001";
}
.fa-search:before {
  content: "\f002";
}
.fa-envelope-o:before {
  content: "\f003";
}
.fa-heart:before {
  content: "\f004";
}
.fa-star:before {
  content: "\f005";
}
.fa-star-o:before {
  content: "\f006";
}
.fa-user:before {
  content: "\f007";
}
.fa-film:before {
  content: "\f008";
}
.fa-th-large:before {
  content: "\f009";
}
.fa-th:before {
  content: "\f00a";
}
.fa-th-list:before {
  content: "\f00b";
}
.fa-check:before {
  content: "\f00c";
}
.fa-remove:before,
.fa-close:before,
.fa-times:before {
  content: "\f00d";
}
.fa-search-plus:before {
  content: "\f00e";
}
.fa-search-minus:before {
  content: "\f010";
}
.fa-power-off:before {
  content: "\f011";
}
.fa-signal:before {
  content: "\f012";
}
.fa-gear:before,
.fa-cog:before {
  content: "\f013";
}
.fa-trash-o:before {
  content: "\f014";
}
.fa-home:before {
  content: "\f015";
}
.fa-file-o:before {
  content: "\f016";
}
.fa-clock-o:before {
  content: "\f017";
}
.fa-road:before {
  content: "\f018";
}
.fa-download:before {
  content: "\f019";
}
.fa-arrow-circle-o-down:before {
  content: "\f01a";
}
.fa-arrow-circle-o-up:before {
  content: "\f01b";
}
.fa-inbox:before {
  content: "\f01c";
}
.fa-play-circle-o:before {
  content: "\f01d";
}
.fa-rotate-right:before,
.fa-repeat:before {
  content: "\f01e";
}
.fa-refresh:before {
  content: "\f021";
}
.fa-list-alt:before {
  content: "\f022";
}
.fa-lock:before {
  content: "\f023";
}
.fa-flag:before {
  content: "\f024";
}
.fa-headphones:before {
  content: "\f025";
}
.fa-volume-off:before {
  content: "\f026";
}
.fa-volume-down:before {
  content: "\f027";
}
.fa-volume-up:before {
  content: "\f028";
}
.fa-qrcode:before {
  content: "\f029";
}
.fa-barcode:before {
  content: "\f02a";
}
.fa-tag:before {
  content: "\f02b";
}
.fa-tags:before {
  content: "\f02c";
}
.fa-book:before {
  content: "\f02d";
}
.fa-bookmark:before {
  content: "\f02e";
}
.fa-print:before {
  content: "\f02f";
}
.fa-camera:before {
  content: "\f030";
}
.fa-font:before {
  content: "\f031";
}
.fa-bold:before {
  content: "\f032";
}
.fa-italic:before {
  content: "\f033";
}
.fa-text-height:before {
  content: "\f034";
}
.fa-text-width:before {
  content: "\f035";
}
.fa-align-left:before {
  content: "\f036";
}
.fa-align-center:before {
  content: "\f037";
}
.fa-align-right:before {
  content: "\f038";
}
.fa-align-justify:before {
  content: "\f039";
}
.fa-list:before {
  content: "\f03a";
}
.fa-dedent:before,
.fa-outdent:before {
  content: "\f03b";
}
.fa-indent:before {
  content: "\f03c";
}
.fa-video-camera:before {
  content: "\f03d";
}
.fa-photo:before,
.fa-image:before,
.fa-picture-o:before {
  content: "\f03e";
}
.fa-pencil:before {
  content: "\f040";
}
.fa-map-marker:before {
  content: "\f041";
}
.fa-adjust:before {
  content: "\f042";
}
.fa-tint:before {
  content: "\f043";
}
.fa-edit:before,
.fa-pencil-square-o:before {
  content: "\f044";
}
.fa-share-square-o:before {
  content: "\f045";
}
.fa-check-square-o:before {
  content: "\f046";
}
.fa-arrows:before {
  content: "\f047";
}
.fa-step-backward:before {
  content: "\f048";
}
.fa-fast-backward:before {
  content: "\f049";
}
.fa-backward:before {
  content: "\f04a";
}
.fa-play:before {
  content: "\f04b";
}
.fa-pause:before {
  content: "\f04c";
}
.fa-stop:before {
  content: "\f04d";
}
.fa-forward:before {
  content: "\f04e";
}
.fa-fast-forward:before {
  content: "\f050";
}
.fa-step-forward:before {
  content: "\f051";
}
.fa-eject:before {
  content: "\f052";
}
.fa-chevron-left:before {
  content: "\f053";
}
.fa-chevron-right:before {
  content: "\f054";
}
.fa-plus-circle:before {
  content: "\f055";
}
.fa-minus-circle:before {
  content: "\f056";
}
.fa-times-circle:before {
  content: "\f057";
}
.fa-check-circle:before {
  content: "\f058";
}
.fa-question-circle:before {
  content: "\f059";
}
.fa-info-circle:before {
  content: "\f05a";
}
.fa-crosshairs:before {
  content: "\f05b";
}
.fa-times-circle-o:before {
  content: "\f05c";
}
.fa-check-circle-o:before {
  content: "\f05d";
}
.fa-ban:before {
  content: "\f05e";
}
.fa-arrow-left:before {
  content: "\f060";
}
.fa-arrow-right:before {
  content: "\f061";
}
.fa-arrow-up:before {
  content: "\f062";
}
.fa-arrow-down:before {
  content: "\f063";
}
.fa-mail-forward:before,
.fa-share:before {
  content: "\f064";
}
.fa-expand:before {
  content: "\f065";
}
.fa-compress:before {
  content: "\f066";
}
.fa-plus:before {
  content: "\f067";
}
.fa-minus:before {
  content: "\f068";
}
.fa-asterisk:before {
  content: "\f069";
}
.fa-exclamation-circle:before {
  content: "\f06a";
}
.fa-gift:before {
  content: "\f06b";
}
.fa-leaf:before {
  content: "\f06c";
}
.fa-fire:before {
  content: "\f06d";
}
.fa-eye:before {
  content: "\f06e";
}
.fa-eye-slash:before {
  content: "\f070";
}
.fa-warning:before,
.fa-exclamation-triangle:before {
  content: "\f071";
}
.fa-plane:before {
  content: "\f072";
}
.fa-calendar:before {
  content: "\f073";
}
.fa-random:before {
  content: "\f074";
}
.fa-comment:before {
  content: "\f075";
}
.fa-magnet:before {
  content: "\f076";
}
.fa-chevron-up:before {
  content: "\f077";
}
.fa-chevron-down:before {
  content: "\f078";
}
.fa-retweet:before {
  content: "\f079";
}
.fa-shopping-cart:before {
  content: "\f07a";
}
.fa-folder:before {
  content: "\f07b";
}
.fa-folder-open:before {
  content: "\f07c";
}
.fa-arrows-v:before {
  content: "\f07d";
}
.fa-arrows-h:before {
  content: "\f07e";
}
.fa-bar-chart-o:before,
.fa-bar-chart:before {
  content: "\f080";
}
.fa-twitter-square:before {
  content: "\f081";
}
.fa-facebook-square:before {
  content: "\f082";
}
.fa-camera-retro:before {
  content: "\f083";
}
.fa-key:before {
  content: "\f084";
}
.fa-gears:before,
.fa-cogs:before {
  content: "\f085";
}
.fa-comments:before {
  content: "\f086";
}
.fa-thumbs-o-up:before {
  content: "\f087";
}
.fa-thumbs-o-down:before {
  content: "\f088";
}
.fa-star-half:before {
  content: "\f089";
}
.fa-heart-o:before {
  content: "\f08a";
}
.fa-sign-out:before {
  content: "\f08b";
}
.fa-linkedin-square:before {
  content: "\f08c";
}
.fa-thumb-tack:before {
  content: "\f08d";
}
.fa-external-link:before {
  content: "\f08e";
}
.fa-sign-in:before {
  content: "\f090";
}
.fa-trophy:before {
  content: "\f091";
}
.fa-github-square:before {
  content: "\f092";
}
.fa-upload:before {
  content: "\f093";
}
.fa-lemon-o:before {
  content: "\f094";
}
.fa-phone:before {
  content: "\f095";
}
.fa-square-o:before {
  content: "\f096";
}
.fa-bookmark-o:before {
  content: "\f097";
}
.fa-phone-square:before {
  content: "\f098";
}
.fa-twitter:before {
  content: "\f099";
}
.fa-facebook-f:before,
.fa-facebook:before {
  content: "\f09a";
}
.fa-github:before {
  content: "\f09b";
}
.fa-unlock:before {
  content: "\f09c";
}
.fa-credit-card:before {
  content: "\f09d";
}
.fa-feed:before,
.fa-rss:before {
  content: "\f09e";
}
.fa-hdd-o:before {
  content: "\f0a0";
}
.fa-bullhorn:before {
  content: "\f0a1";
}
.fa-bell:before {
  content: "\f0f3";
}
.fa-certificate:before {
  content: "\f0a3";
}
.fa-hand-o-right:before {
  content: "\f0a4";
}
.fa-hand-o-left:before {
  content: "\f0a5";
}
.fa-hand-o-up:before {
  content: "\f0a6";
}
.fa-hand-o-down:before {
  content: "\f0a7";
}
.fa-arrow-circle-left:before {
  content: "\f0a8";
}
.fa-arrow-circle-right:before {
  content: "\f0a9";
}
.fa-arrow-circle-up:before {
  content: "\f0aa";
}
.fa-arrow-circle-down:before {
  content: "\f0ab";
}
.fa-globe:before {
  content: "\f0ac";
}
.fa-wrench:before {
  content: "\f0ad";
}
.fa-tasks:before {
  content: "\f0ae";
}
.fa-filter:before {
  content: "\f0b0";
}
.fa-briefcase:before {
  content: "\f0b1";
}
.fa-arrows-alt:before {
  content: "\f0b2";
}
.fa-group:before,
.fa-users:before {
  content: "\f0c0";
}
.fa-chain:before,
.fa-link:before {
  content: "\f0c1";
}
.fa-cloud:before {
  content: "\f0c2";
}
.fa-flask:before {
  content: "\f0c3";
}
.fa-cut:before,
.fa-scissors:before {
  content: "\f0c4";
}
.fa-copy:before,
.fa-files-o:before {
  content: "\f0c5";
}
.fa-paperclip:before {
  content: "\f0c6";
}
.fa-save:before,
.fa-floppy-o:before {
  content: "\f0c7";
}
.fa-square:before {
  content: "\f0c8";
}
.fa-navicon:before,
.fa-reorder:before,
.fa-bars:before {
  content: "\f0c9";
}
.fa-list-ul:before {
  content: "\f0ca";
}
.fa-list-ol:before {
  content: "\f0cb";
}
.fa-strikethrough:before {
  content: "\f0cc";
}
.fa-underline:before {
  content: "\f0cd";
}
.fa-table:before {
  content: "\f0ce";
}
.fa-magic:before {
  content: "\f0d0";
}
.fa-truck:before {
  content: "\f0d1";
}
.fa-pinterest:before {
  content: "\f0d2";
}
.fa-pinterest-square:before {
  content: "\f0d3";
}
.fa-google-plus-square:before {
  content: "\f0d4";
}
.fa-google-plus:before {
  content: "\f0d5";
}
.fa-money:before {
  content: "\f0d6";
}
.fa-caret-down:before {
  content: "\f0d7";
}
.fa-caret-up:before {
  content: "\f0d8";
}
.fa-caret-left:before {
  content: "\f0d9";
}
.fa-caret-right:before {
  content: "\f0da";
}
.fa-columns:before {
  content: "\f0db";
}
.fa-unsorted:before,
.fa-sort:before {
  content: "\f0dc";
}
.fa-sort-down:before,
.fa-sort-desc:before {
  content: "\f0dd";
}
.fa-sort-up:before,
.fa-sort-asc:before {
  content: "\f0de";
}
.fa-envelope:before {
  content: "\f0e0";
}
.fa-linkedin:before {
  content: "\f0e1";
}
.fa-rotate-left:before,
.fa-undo:before {
  content: "\f0e2";
}
.fa-legal:before,
.fa-gavel:before {
  content: "\f0e3";
}
.fa-dashboard:before,
.fa-tachometer:before {
  content: "\f0e4";
}
.fa-comment-o:before {
  content: "\f0e5";
}
.fa-comments-o:before {
  content: "\f0e6";
}
.fa-flash:before,
.fa-bolt:before {
  content: "\f0e7";
}
.fa-sitemap:before {
  content: "\f0e8";
}
.fa-umbrella:before {
  content: "\f0e9";
}
.fa-paste:before,
.fa-clipboard:before {
  content: "\f0ea";
}
.fa-lightbulb-o:before {
  content: "\f0eb";
}
.fa-exchange:before {
  content: "\f0ec";
}
.fa-cloud-download:before {
  content: "\f0ed";
}
.fa-cloud-upload:before {
  content: "\f0ee";
}
.fa-user-md:before {
  content: "\f0f0";
}
.fa-stethoscope:before {
  content: "\f0f1";
}
.fa-suitcase:before {
  content: "\f0f2";
}
.fa-bell-o:before {
  content: "\f0a2";
}
.fa-coffee:before {
  content: "\f0f4";
}
.fa-cutlery:before {
  content: "\f0f5";
}
.fa-file-text-o:before {
  content: "\f0f6";
}
.fa-building-o:before {
  content: "\f0f7";
}
.fa-hospital-o:before {
  content: "\f0f8";
}
.fa-ambulance:before {
  content: "\f0f9";
}
.fa-medkit:before {
  content: "\f0fa";
}
.fa-fighter-jet:before {
  content: "\f0fb";
}
.fa-beer:before {
  content: "\f0fc";
}
.fa-h-square:before {
  content: "\f0fd";
}
.fa-plus-square:before {
  content: "\f0fe";
}
.fa-angle-double-left:before {
  content: "\f100";
}
.fa-angle-double-right:before {
  content: "\f101";
}
.fa-angle-double-up:before {
  content: "\f102";
}
.fa-angle-double-down:before {
  content: "\f103";
}
.fa-angle-left:before {
  content: "\f104";
}
.fa-angle-right:before {
  content: "\f105";
}
.fa-angle-up:before {
  content: "\f106";
}
.fa-angle-down:before {
  content: "\f107";
}
.fa-desktop:before {
  content: "\f108";
}
.fa-laptop:before {
  content: "\f109";
}
.fa-tablet:before {
  content: "\f10a";
}
.fa-mobile-phone:before,
.fa-mobile:before {
  content: "\f10b";
}
.fa-circle-o:before {
  content: "\f10c";
}
.fa-quote-left:before {
  content: "\f10d";
}
.fa-quote-right:before {
  content: "\f10e";
}
.fa-spinner:before {
  content: "\f110";
}
.fa-circle:before {
  content: "\f111";
}
.fa-mail-reply:before,
.fa-reply:before {
  content: "\f112";
}
.fa-github-alt:before {
  content: "\f113";
}
.fa-folder-o:before {
  content: "\f114";
}
.fa-folder-open-o:before {
  content: "\f115";
}
.fa-smile-o:before {
  content: "\f118";
}
.fa-frown-o:before {
  content: "\f119";
}
.fa-meh-o:before {
  content: "\f11a";
}
.fa-gamepad:before {
  content: "\f11b";
}
.fa-keyboard-o:before {
  content: "\f11c";
}
.fa-flag-o:before {
  content: "\f11d";
}
.fa-flag-checkered:before {
  content: "\f11e";
}
.fa-terminal:before {
  content: "\f120";
}
.fa-code:before {
  content: "\f121";
}
.fa-mail-reply-all:before,
.fa-reply-all:before {
  content: "\f122";
}
.fa-star-half-empty:before,
.fa-star-half-full:before,
.fa-star-half-o:before {
  content: "\f123";
}
.fa-location-arrow:before {
  content: "\f124";
}
.fa-crop:before {
  content: "\f125";
}
.fa-code-fork:before {
  content: "\f126";
}
.fa-unlink:before,
.fa-chain-broken:before {
  content: "\f127";
}
.fa-question:before {
  content: "\f128";
}
.fa-info:before {
  content: "\f129";
}
.fa-exclamation:before {
  content: "\f12a";
}
.fa-superscript:before {
  content: "\f12b";
}
.fa-subscript:before {
  content: "\f12c";
}
.fa-eraser:before {
  content: "\f12d";
}
.fa-puzzle-piece:before {
  content: "\f12e";
}
.fa-microphone:before {
  content: "\f130";
}
.fa-microphone-slash:before {
  content: "\f131";
}
.fa-shield:before {
  content: "\f132";
}
.fa-calendar-o:before {
  content: "\f133";
}
.fa-fire-extinguisher:before {
  content: "\f134";
}
.fa-rocket:before {
  content: "\f135";
}
.fa-maxcdn:before {
  content: "\f136";
}
.fa-chevron-circle-left:before {
  content: "\f137";
}
.fa-chevron-circle-right:before {
  content: "\f138";
}
.fa-chevron-circle-up:before {
  content: "\f139";
}
.fa-chevron-circle-down:before {
  content: "\f13a";
}
.fa-html5:before {
  content: "\f13b";
}
.fa-css3:before {
  content: "\f13c";
}
.fa-anchor:before {
  content: "\f13d";
}
.fa-unlock-alt:before {
  content: "\f13e";
}
.fa-bullseye:before {
  content: "\f140";
}
.fa-ellipsis-h:before {
  content: "\f141";
}
.fa-ellipsis-v:before {
  content: "\f142";
}
.fa-rss-square:before {
  content: "\f143";
}
.fa-play-circle:before {
  content: "\f144";
}
.fa-ticket:before {
  content: "\f145";
}
.fa-minus-square:before {
  content: "\f146";
}
.fa-minus-square-o:before {
  content: "\f147";
}
.fa-level-up:before {
  content: "\f148";
}
.fa-level-down:before {
  content: "\f149";
}
.fa-check-square:before {
  content: "\f14a";
}
.fa-pencil-square:before {
  content: "\f14b";
}
.fa-external-link-square:before {
  content: "\f14c";
}
.fa-share-square:before {
  content: "\f14d";
}
.fa-compass:before {
  content: "\f14e";
}
.fa-toggle-down:before,
.fa-caret-square-o-down:before {
  content: "\f150";
}
.fa-toggle-up:before,
.fa-caret-square-o-up:before {
  content: "\f151";
}
.fa-toggle-right:before,
.fa-caret-square-o-right:before {
  content: "\f152";
}
.fa-euro:before,
.fa-eur:before {
  content: "\f153";
}
.fa-gbp:before {
  content: "\f154";
}
.fa-dollar:before,
.fa-usd:before {
  content: "\f155";
}
.fa-rupee:before,
.fa-inr:before {
  content: "\f156";
}
.fa-cny:before,
.fa-rmb:before,
.fa-yen:before,
.fa-jpy:before {
  content: "\f157";
}
.fa-ruble:before,
.fa-rouble:before,
.fa-rub:before {
  content: "\f158";
}
.fa-won:before,
.fa-krw:before {
  content: "\f159";
}
.fa-bitcoin:before,
.fa-btc:before {
  content: "\f15a";
}
.fa-file:before {
  content: "\f15b";
}
.fa-file-text:before {
  content: "\f15c";
}
.fa-sort-alpha-asc:before {
  content: "\f15d";
}
.fa-sort-alpha-desc:before {
  content: "\f15e";
}
.fa-sort-amount-asc:before {
  content: "\f160";
}
.fa-sort-amount-desc:before {
  content: "\f161";
}
.fa-sort-numeric-asc:before {
  content: "\f162";
}
.fa-sort-numeric-desc:before {
  content: "\f163";
}
.fa-thumbs-up:before {
  content: "\f164";
}
.fa-thumbs-down:before {
  content: "\f165";
}
.fa-youtube-square:before {
  content: "\f166";
}
.fa-youtube:before {
  content: "\f167";
}
.fa-xing:before {
  content: "\f168";
}
.fa-xing-square:before {
  content: "\f169";
}
.fa-youtube-play:before {
  content: "\f16a";
}
.fa-dropbox:before {
  content: "\f16b";
}
.fa-stack-overflow:before {
  content: "\f16c";
}
.fa-instagram:before {
  content: "\f16d";
}
.fa-flickr:before {
  content: "\f16e";
}
.fa-adn:before {
  content: "\f170";
}
.fa-bitbucket:before {
  content: "\f171";
}
.fa-bitbucket-square:before {
  content: "\f172";
}
.fa-tumblr:before {
  content: "\f173";
}
.fa-tumblr-square:before {
  content: "\f174";
}
.fa-long-arrow-down:before {
  content: "\f175";
}
.fa-long-arrow-up:before {
  content: "\f176";
}
.fa-long-arrow-left:before {
  content: "\f177";
}
.fa-long-arrow-right:before {
  content: "\f178";
}
.fa-apple:before {
  content: "\f179";
}
.fa-windows:before {
  content: "\f17a";
}
.fa-android:before {
  content: "\f17b";
}
.fa-linux:before {
  content: "\f17c";
}
.fa-dribbble:before {
  content: "\f17d";
}
.fa-skype:before {
  content: "\f17e";
}
.fa-foursquare:before {
  content: "\f180";
}
.fa-trello:before {
  content: "\f181";
}
.fa-female:before {
  content: "\f182";
}
.fa-male:before {
  content: "\f183";
}
.fa-gittip:before,
.fa-gratipay:before {
  content: "\f184";
}
.fa-sun-o:before {
  content: "\f185";
}
.fa-moon-o:before {
  content: "\f186";
}
.fa-archive:before {
  content: "\f187";
}
.fa-bug:before {
  content: "\f188";
}
.fa-vk:before {
  content: "\f189";
}
.fa-weibo:before {
  content: "\f18a";
}
.fa-renren:before {
  content: "\f18b";
}
.fa-pagelines:before {
  content: "\f18c";
}
.fa-stack-exchange:before {
  content: "\f18d";
}
.fa-arrow-circle-o-right:before {
  content: "\f18e";
}
.fa-arrow-circle-o-left:before {
  content: "\f190";
}
.fa-toggle-left:before,
.fa-caret-square-o-left:before {
  content: "\f191";
}
.fa-dot-circle-o:before {
  content: "\f192";
}
.fa-wheelchair:before {
  content: "\f193";
}
.fa-vimeo-square:before {
  content: "\f194";
}
.fa-turkish-lira:before,
.fa-try:before {
  content: "\f195";
}
.fa-plus-square-o:before {
  content: "\f196";
}
.fa-space-shuttle:before {
  content: "\f197";
}
.fa-slack:before {
  content: "\f198";
}
.fa-envelope-square:before {
  content: "\f199";
}
.fa-wordpress:before {
  content: "\f19a";
}
.fa-openid:before {
  content: "\f19b";
}
.fa-institution:before,
.fa-bank:before,
.fa-university:before {
  content: "\f19c";
}
.fa-mortar-board:before,
.fa-graduation-cap:before {
  content: "\f19d";
}
.fa-yahoo:before {
  content: "\f19e";
}
.fa-google:before {
  content: "\f1a0";
}
.fa-reddit:before {
  content: "\f1a1";
}
.fa-reddit-square:before {
  content: "\f1a2";
}
.fa-stumbleupon-circle:before {
  content: "\f1a3";
}
.fa-stumbleupon:before {
  content: "\f1a4";
}
.fa-delicious:before {
  content: "\f1a5";
}
.fa-digg:before {
  content: "\f1a6";
}
.fa-pied-piper-pp:before {
  content: "\f1a7";
}
.fa-pied-piper-alt:before {
  content: "\f1a8";
}
.fa-drupal:before {
  content: "\f1a9";
}
.fa-joomla:before {
  content: "\f1aa";
}
.fa-language:before {
  content: "\f1ab";
}
.fa-fax:before {
  content: "\f1ac";
}
.fa-building:before {
  content: "\f1ad";
}
.fa-child:before {
  content: "\f1ae";
}
.fa-paw:before {
  content: "\f1b0";
}
.fa-spoon:before {
  content: "\f1b1";
}
.fa-cube:before {
  content: "\f1b2";
}
.fa-cubes:before {
  content: "\f1b3";
}
.fa-behance:before {
  content: "\f1b4";
}
.fa-behance-square:before {
  content: "\f1b5";
}
.fa-steam:before {
  content: "\f1b6";
}
.fa-steam-square:before {
  content: "\f1b7";
}
.fa-recycle:before {
  content: "\f1b8";
}
.fa-automobile:before,
.fa-car:before {
  content: "\f1b9";
}
.fa-cab:before,
.fa-taxi:before {
  content: "\f1ba";
}
.fa-tree:before {
  content: "\f1bb";
}
.fa-spotify:before {
  content: "\f1bc";
}
.fa-deviantart:before {
  content: "\f1bd";
}
.fa-soundcloud:before {
  content: "\f1be";
}
.fa-database:before {
  content: "\f1c0";
}
.fa-file-pdf-o:before {
  content: "\f1c1";
}
.fa-file-word-o:before {
  content: "\f1c2";
}
.fa-file-excel-o:before {
  content: "\f1c3";
}
.fa-file-powerpoint-o:before {
  content: "\f1c4";
}
.fa-file-photo-o:before,
.fa-file-picture-o:before,
.fa-file-image-o:before {
  content: "\f1c5";
}
.fa-file-zip-o:before,
.fa-file-archive-o:before {
  content: "\f1c6";
}
.fa-file-sound-o:before,
.fa-file-audio-o:before {
  content: "\f1c7";
}
.fa-file-movie-o:before,
.fa-file-video-o:before {
  content: "\f1c8";
}
.fa-file-code-o:before {
  content: "\f1c9";
}
.fa-vine:before {
  content: "\f1ca";
}
.fa-codepen:before {
  content: "\f1cb";
}
.fa-jsfiddle:before {
  content: "\f1cc";
}
.fa-life-bouy:before,
.fa-life-buoy:before,
.fa-life-saver:before,
.fa-support:before,
.fa-life-ring:before {
  content: "\f1cd";
}
.fa-circle-o-notch:before {
  content: "\f1ce";
}
.fa-ra:before,
.fa-resistance:before,
.fa-rebel:before {
  content: "\f1d0";
}
.fa-ge:before,
.fa-empire:before {
  content: "\f1d1";
}
.fa-git-square:before {
  content: "\f1d2";
}
.fa-git:before {
  content: "\f1d3";
}
.fa-y-combinator-square:before,
.fa-yc-square:before,
.fa-hacker-news:before {
  content: "\f1d4";
}
.fa-tencent-weibo:before {
  content: "\f1d5";
}
.fa-qq:before {
  content: "\f1d6";
}
.fa-wechat:before,
.fa-weixin:before {
  content: "\f1d7";
}
.fa-send:before,
.fa-paper-plane:before {
  content: "\f1d8";
}
.fa-send-o:before,
.fa-paper-plane-o:before {
  content: "\f1d9";
}
.fa-history:before {
  content: "\f1da";
}
.fa-circle-thin:before {
  content: "\f1db";
}
.fa-header:before {
  content: "\f1dc";
}
.fa-paragraph:before {
  content: "\f1dd";
}
.fa-sliders:before {
  content: "\f1de";
}
.fa-share-alt:before {
  content: "\f1e0";
}
.fa-share-alt-square:before {
  content: "\f1e1";
}
.fa-bomb:before {
  content: "\f1e2";
}
.fa-soccer-ball-o:before,
.fa-futbol-o:before {
  content: "\f1e3";
}
.fa-tty:before {
  content: "\f1e4";
}
.fa-binoculars:before {
  content: "\f1e5";
}
.fa-plug:before {
  content: "\f1e6";
}
.fa-slideshare:before {
  content: "\f1e7";
}
.fa-twitch:before {
  content: "\f1e8";
}
.fa-yelp:before {
  content: "\f1e9";
}
.fa-newspaper-o:before {
  content: "\f1ea";
}
.fa-wifi:before {
  content: "\f1eb";
}
.fa-calculator:before {
  content: "\f1ec";
}
.fa-paypal:before {
  content: "\f1ed";
}
.fa-google-wallet:before {
  content: "\f1ee";
}
.fa-cc-visa:before {
  content: "\f1f0";
}
.fa-cc-mastercard:before {
  content: "\f1f1";
}
.fa-cc-discover:before {
  content: "\f1f2";
}
.fa-cc-amex:before {
  content: "\f1f3";
}
.fa-cc-paypal:before {
  content: "\f1f4";
}
.fa-cc-stripe:before {
  content: "\f1f5";
}
.fa-bell-slash:before {
  content: "\f1f6";
}
.fa-bell-slash-o:before {
  content: "\f1f7";
}
.fa-trash:before {
  content: "\f1f8";
}
.fa-copyright:before {
  content: "\f1f9";
}
.fa-at:before {
  content: "\f1fa";
}
.fa-eyedropper:before {
  content: "\f1fb";
}
.fa-paint-brush:before {
  content: "\f1fc";
}
.fa-birthday-cake:before {
  content: "\f1fd";
}
.fa-area-chart:before {
  content: "\f1fe";
}
.fa-pie-chart:before {
  content: "\f200";
}
.fa-line-chart:before {
  content: "\f201";
}
.fa-lastfm:before {
  content: "\f202";
}
.fa-lastfm-square:before {
  content: "\f203";
}
.fa-toggle-off:before {
  content: "\f204";
}
.fa-toggle-on:before {
  content: "\f205";
}
.fa-bicycle:before {
  content: "\f206";
}
.fa-bus:before {
  content: "\f207";
}
.fa-ioxhost:before {
  content: "\f208";
}
.fa-angellist:before {
  content: "\f209";
}
.fa-cc:before {
  content: "\f20a";
}
.fa-shekel:before,
.fa-sheqel:before,
.fa-ils:before {
  content: "\f20b";
}
.fa-meanpath:before {
  content: "\f20c";
}
.fa-buysellads:before {
  content: "\f20d";
}
.fa-connectdevelop:before {
  content: "\f20e";
}
.fa-dashcube:before {
  content: "\f210";
}
.fa-forumbee:before {
  content: "\f211";
}
.fa-leanpub:before {
  content: "\f212";
}
.fa-sellsy:before {
  content: "\f213";
}
.fa-shirtsinbulk:before {
  content: "\f214";
}
.fa-simplybuilt:before {
  content: "\f215";
}
.fa-skyatlas:before {
  content: "\f216";
}
.fa-cart-plus:before {
  content: "\f217";
}
.fa-cart-arrow-down:before {
  content: "\f218";
}
.fa-diamond:before {
  content: "\f219";
}
.fa-ship:before {
  content: "\f21a";
}
.fa-user-secret:before {
  content: "\f21b";
}
.fa-motorcycle:before {
  content: "\f21c";
}
.fa-street-view:before {
  content: "\f21d";
}
.fa-heartbeat:before {
  content: "\f21e";
}
.fa-venus:before {
  content: "\f221";
}
.fa-mars:before {
  content: "\f222";
}
.fa-mercury:before {
  content: "\f223";
}
.fa-intersex:before,
.fa-transgender:before {
  content: "\f224";
}
.fa-transgender-alt:before {
  content: "\f225";
}
.fa-venus-double:before {
  content: "\f226";
}
.fa-mars-double:before {
  content: "\f227";
}
.fa-venus-mars:before {
  content: "\f228";
}
.fa-mars-stroke:before {
  content: "\f229";
}
.fa-mars-stroke-v:before {
  content: "\f22a";
}
.fa-mars-stroke-h:before {
  content: "\f22b";
}
.fa-neuter:before {
  content: "\f22c";
}
.fa-genderless:before {
  content: "\f22d";
}
.fa-facebook-official:before {
  content: "\f230";
}
.fa-pinterest-p:before {
  content: "\f231";
}
.fa-whatsapp:before {
  content: "\f232";
}
.fa-server:before {
  content: "\f233";
}
.fa-user-plus:before {
  content: "\f234";
}
.fa-user-times:before {
  content: "\f235";
}
.fa-hotel:before,
.fa-bed:before {
  content: "\f236";
}
.fa-viacoin:before {
  content: "\f237";
}
.fa-train:before {
  content: "\f238";
}
.fa-subway:before {
  content: "\f239";
}
.fa-medium:before {
  content: "\f23a";
}
.fa-yc:before,
.fa-y-combinator:before {
  content: "\f23b";
}
.fa-optin-monster:before {
  content: "\f23c";
}
.fa-opencart:before {
  content: "\f23d";
}
.fa-expeditedssl:before {
  content: "\f23e";
}
.fa-battery-4:before,
.fa-battery:before,
.fa-battery-full:before {
  content: "\f240";
}
.fa-battery-3:before,
.fa-battery-three-quarters:before {
  content: "\f241";
}
.fa-battery-2:before,
.fa-battery-half:before {
  content: "\f242";
}
.fa-battery-1:before,
.fa-battery-quarter:before {
  content: "\f243";
}
.fa-battery-0:before,
.fa-battery-empty:before {
  content: "\f244";
}
.fa-mouse-pointer:before {
  content: "\f245";
}
.fa-i-cursor:before {
  content: "\f246";
}
.fa-object-group:before {
  content: "\f247";
}
.fa-object-ungroup:before {
  content: "\f248";
}
.fa-sticky-note:before {
  content: "\f249";
}
.fa-sticky-note-o:before {
  content: "\f24a";
}
.fa-cc-jcb:before {
  content: "\f24b";
}
.fa-cc-diners-club:before {
  content: "\f24c";
}
.fa-clone:before {
  content: "\f24d";
}
.fa-balance-scale:before {
  content: "\f24e";
}
.fa-hourglass-o:before {
  content: "\f250";
}
.fa-hourglass-1:before,
.fa-hourglass-start:before {
  content: "\f251";
}
.fa-hourglass-2:before,
.fa-hourglass-half:before {
  content: "\f252";
}
.fa-hourglass-3:before,
.fa-hourglass-end:before {
  content: "\f253";
}
.fa-hourglass:before {
  content: "\f254";
}
.fa-hand-grab-o:before,
.fa-hand-rock-o:before {
  content: "\f255";
}
.fa-hand-stop-o:before,
.fa-hand-paper-o:before {
  content: "\f256";
}
.fa-hand-scissors-o:before {
  content: "\f257";
}
.fa-hand-lizard-o:before {
  content: "\f258";
}
.fa-hand-spock-o:before {
  content: "\f259";
}
.fa-hand-pointer-o:before {
  content: "\f25a";
}
.fa-hand-peace-o:before {
  content: "\f25b";
}
.fa-trademark:before {
  content: "\f25c";
}
.fa-registered:before {
  content: "\f25d";
}
.fa-creative-commons:before {
  content: "\f25e";
}
.fa-gg:before {
  content: "\f260";
}
.fa-gg-circle:before {
  content: "\f261";
}
.fa-tripadvisor:before {
  content: "\f262";
}
.fa-odnoklassniki:before {
  content: "\f263";
}
.fa-odnoklassniki-square:before {
  content: "\f264";
}
.fa-get-pocket:before {
  content: "\f265";
}
.fa-wikipedia-w:before {
  content: "\f266";
}
.fa-safari:before {
  content: "\f267";
}
.fa-chrome:before {
  content: "\f268";
}
.fa-firefox:before {
  content: "\f269";
}
.fa-opera:before {
  content: "\f26a";
}
.fa-internet-explorer:before {
  content: "\f26b";
}
.fa-tv:before,
.fa-television:before {
  content: "\f26c";
}
.fa-contao:before {
  content: "\f26d";
}
.fa-500px:before {
  content: "\f26e";
}
.fa-amazon:before {
  content: "\f270";
}
.fa-calendar-plus-o:before {
  content: "\f271";
}
.fa-calendar-minus-o:before {
  content: "\f272";
}
.fa-calendar-times-o:before {
  content: "\f273";
}
.fa-calendar-check-o:before {
  content: "\f274";
}
.fa-industry:before {
  content: "\f275";
}
.fa-map-pin:before {
  content: "\f276";
}
.fa-map-signs:before {
  content: "\f277";
}
.fa-map-o:before {
  content: "\f278";
}
.fa-map:before {
  content: "\f279";
}
.fa-commenting:before {
  content: "\f27a";
}
.fa-commenting-o:before {
  content: "\f27b";
}
.fa-houzz:before {
  content: "\f27c";
}
.fa-vimeo:before {
  content: "\f27d";
}
.fa-black-tie:before {
  content: "\f27e";
}
.fa-fonticons:before {
  content: "\f280";
}
.fa-reddit-alien:before {
  content: "\f281";
}
.fa-edge:before {
  content: "\f282";
}
.fa-credit-card-alt:before {
  content: "\f283";
}
.fa-codiepie:before {
  content: "\f284";
}
.fa-modx:before {
  content: "\f285";
}
.fa-fort-awesome:before {
  content: "\f286";
}
.fa-usb:before {
  content: "\f287";
}
.fa-product-hunt:before {
  content: "\f288";
}
.fa-mixcloud:before {
  content: "\f289";
}
.fa-scribd:before {
  content: "\f28a";
}
.fa-pause-circle:before {
  content: "\f28b";
}
.fa-pause-circle-o:before {
  content: "\f28c";
}
.fa-stop-circle:before {
  content: "\f28d";
}
.fa-stop-circle-o:before {
  content: "\f28e";
}
.fa-shopping-bag:before {
  content: "\f290";
}
.fa-shopping-basket:before {
  content: "\f291";
}
.fa-hashtag:before {
  content: "\f292";
}
.fa-bluetooth:before {
  content: "\f293";
}
.fa-bluetooth-b:before {
  content: "\f294";
}
.fa-percent:before {
  content: "\f295";
}
.fa-gitlab:before {
  content: "\f296";
}
.fa-wpbeginner:before {
  content: "\f297";
}
.fa-wpforms:before {
  content: "\f298";
}
.fa-envira:before {
  content: "\f299";
}
.fa-universal-access:before {
  content: "\f29a";
}
.fa-wheelchair-alt:before {
  content: "\f29b";
}
.fa-question-circle-o:before {
  content: "\f29c";
}
.fa-blind:before {
  content: "\f29d";
}
.fa-audio-description:before {
  content: "\f29e";
}
.fa-volume-control-phone:before {
  content: "\f2a0";
}
.fa-braille:before {
  content: "\f2a1";
}
.fa-assistive-listening-systems:before {
  content: "\f2a2";
}
.fa-asl-interpreting:before,
.fa-american-sign-language-interpreting:before {
  content: "\f2a3";
}
.fa-deafness:before,
.fa-hard-of-hearing:before,
.fa-deaf:before {
  content: "\f2a4";
}
.fa-glide:before {
  content: "\f2a5";
}
.fa-glide-g:before {
  content: "\f2a6";
}
.fa-signing:before,
.fa-sign-language:before {
  content: "\f2a7";
}
.fa-low-vision:before {
  content: "\f2a8";
}
.fa-viadeo:before {
  content: "\f2a9";
}
.fa-viadeo-square:before {
  content: "\f2aa";
}
.fa-snapchat:before {
  content: "\f2ab";
}
.fa-snapchat-ghost:before {
  content: "\f2ac";
}
.fa-snapchat-square:before {
  content: "\f2ad";
}
.fa-pied-piper:before {
  content: "\f2ae";
}
.fa-first-order:before {
  content: "\f2b0";
}
.fa-yoast:before {
  content: "\f2b1";
}
.fa-themeisle:before {
  content: "\f2b2";
}
.fa-google-plus-circle:before,
.fa-google-plus-official:before {
  content: "\f2b3";
}
.fa-fa:before,
.fa-font-awesome:before {
  content: "\f2b4";
}
.fa-handshake-o:before {
  content: "\f2b5";
}
.fa-envelope-open:before {
  content: "\f2b6";
}
.fa-envelope-open-o:before {
  content: "\f2b7";
}
.fa-linode:before {
  content: "\f2b8";
}
.fa-address-book:before {
  content: "\f2b9";
}
.fa-address-book-o:before {
  content: "\f2ba";
}
.fa-vcard:before,
.fa-address-card:before {
  content: "\f2bb";
}
.fa-vcard-o:before,
.fa-address-card-o:before {
  content: "\f2bc";
}
.fa-user-circle:before {
  content: "\f2bd";
}
.fa-user-circle-o:before {
  content: "\f2be";
}
.fa-user-o:before {
  content: "\f2c0";
}
.fa-id-badge:before {
  content: "\f2c1";
}
.fa-drivers-license:before,
.fa-id-card:before {
  content: "\f2c2";
}
.fa-drivers-license-o:before,
.fa-id-card-o:before {
  content: "\f2c3";
}
.fa-quora:before {
  content: "\f2c4";
}
.fa-free-code-camp:before {
  content: "\f2c5";
}
.fa-telegram:before {
  content: "\f2c6";
}
.fa-thermometer-4:before,
.fa-thermometer:before,
.fa-thermometer-full:before {
  content: "\f2c7";
}
.fa-thermometer-3:before,
.fa-thermometer-three-quarters:before {
  content: "\f2c8";
}
.fa-thermometer-2:before,
.fa-thermometer-half:before {
  content: "\f2c9";
}
.fa-thermometer-1:before,
.fa-thermometer-quarter:before {
  content: "\f2ca";
}
.fa-thermometer-0:before,
.fa-thermometer-empty:before {
  content: "\f2cb";
}
.fa-shower:before {
  content: "\f2cc";
}
.fa-bathtub:before,
.fa-s15:before,
.fa-bath:before {
  content: "\f2cd";
}
.fa-podcast:before {
  content: "\f2ce";
}
.fa-window-maximize:before {
  content: "\f2d0";
}
.fa-window-minimize:before {
  content: "\f2d1";
}
.fa-window-restore:before {
  content: "\f2d2";
}
.fa-times-rectangle:before,
.fa-window-close:before {
  content: "\f2d3";
}
.fa-times-rectangle-o:before,
.fa-window-close-o:before {
  content: "\f2d4";
}
.fa-bandcamp:before {
  content: "\f2d5";
}
.fa-grav:before {
  content: "\f2d6";
}
.fa-etsy:before {
  content: "\f2d7";
}
.fa-imdb:before {
  content: "\f2d8";
}
.fa-ravelry:before {
  content: "\f2d9";
}
.fa-eercast:before {
  content: "\f2da";
}
.fa-microchip:before {
  content: "\f2db";
}
.fa-snowflake-o:before {
  content: "\f2dc";
}
.fa-superpowers:before {
  content: "\f2dd";
}
.fa-wpexplorer:before {
  content: "\f2de";
}
.fa-meetup:before {
  content: "\f2e0";
}
.sr-only {
  position: absolute;
  width: 1px;
  height: 1px;
  padding: 0;
  margin: -1px;
  overflow: hidden;
  clip: rect(0, 0, 0, 0);
  border: 0;
}
.sr-only-focusable:active,
.sr-only-focusable:focus {
  position: static;
  width: auto;
  height: auto;
  margin: 0;
  overflow: visible;
  clip: auto;
}
.sr-only-focusable:active,
.sr-only-focusable:focus {
  position: static;
  width: auto;
  height: auto;
  margin: 0;
  overflow: visible;
  clip: auto;
}
/*!
*
* IPython base
*
*/
.modal.fade .modal-dialog {
  -webkit-transform: translate(0, 0);
  -ms-transform: translate(0, 0);
  -o-transform: translate(0, 0);
  transform: translate(0, 0);
}
code {
  color: #000;
}
pre {
  font-size: inherit;
  line-height: inherit;
}
label {
  font-weight: normal;
}
/* Make the page background atleast 100% the height of the view port */
/* Make the page itself atleast 70% the height of the view port */
.border-box-sizing {
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
}
.corner-all {
  border-radius: 2px;
}
.no-padding {
  padding: 0px;
}
/* Flexible box model classes */
/* Taken from Alex Russell http://infrequently.org/2009/08/css-3-progress/ */
/* This file is a compatability layer.  It allows the usage of flexible box 
model layouts accross multiple browsers, including older browsers.  The newest,
universal implementation of the flexible box model is used when available (see
`Modern browsers` comments below).  Browsers that are known to implement this 
new spec completely include:

    Firefox 28.0+
    Chrome 29.0+
    Internet Explorer 11+ 
    Opera 17.0+

Browsers not listed, including Safari, are supported via the styling under the
`Old browsers` comments below.
*/
.hbox {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
}
.hbox > * {
  /* Old browsers */
  -webkit-box-flex: 0;
  -moz-box-flex: 0;
  box-flex: 0;
  /* Modern browsers */
  flex: none;
}
.vbox {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
}
.vbox > * {
  /* Old browsers */
  -webkit-box-flex: 0;
  -moz-box-flex: 0;
  box-flex: 0;
  /* Modern browsers */
  flex: none;
}
.hbox.reverse,
.vbox.reverse,
.reverse {
  /* Old browsers */
  -webkit-box-direction: reverse;
  -moz-box-direction: reverse;
  box-direction: reverse;
  /* Modern browsers */
  flex-direction: row-reverse;
}
.hbox.box-flex0,
.vbox.box-flex0,
.box-flex0 {
  /* Old browsers */
  -webkit-box-flex: 0;
  -moz-box-flex: 0;
  box-flex: 0;
  /* Modern browsers */
  flex: none;
  width: auto;
}
.hbox.box-flex1,
.vbox.box-flex1,
.box-flex1 {
  /* Old browsers */
  -webkit-box-flex: 1;
  -moz-box-flex: 1;
  box-flex: 1;
  /* Modern browsers */
  flex: 1;
}
.hbox.box-flex,
.vbox.box-flex,
.box-flex {
  /* Old browsers */
  /* Old browsers */
  -webkit-box-flex: 1;
  -moz-box-flex: 1;
  box-flex: 1;
  /* Modern browsers */
  flex: 1;
}
.hbox.box-flex2,
.vbox.box-flex2,
.box-flex2 {
  /* Old browsers */
  -webkit-box-flex: 2;
  -moz-box-flex: 2;
  box-flex: 2;
  /* Modern browsers */
  flex: 2;
}
.box-group1 {
  /*  Deprecated */
  -webkit-box-flex-group: 1;
  -moz-box-flex-group: 1;
  box-flex-group: 1;
}
.box-group2 {
  /* Deprecated */
  -webkit-box-flex-group: 2;
  -moz-box-flex-group: 2;
  box-flex-group: 2;
}
.hbox.start,
.vbox.start,
.start {
  /* Old browsers */
  -webkit-box-pack: start;
  -moz-box-pack: start;
  box-pack: start;
  /* Modern browsers */
  justify-content: flex-start;
}
.hbox.end,
.vbox.end,
.end {
  /* Old browsers */
  -webkit-box-pack: end;
  -moz-box-pack: end;
  box-pack: end;
  /* Modern browsers */
  justify-content: flex-end;
}
.hbox.center,
.vbox.center,
.center {
  /* Old browsers */
  -webkit-box-pack: center;
  -moz-box-pack: center;
  box-pack: center;
  /* Modern browsers */
  justify-content: center;
}
.hbox.baseline,
.vbox.baseline,
.baseline {
  /* Old browsers */
  -webkit-box-pack: baseline;
  -moz-box-pack: baseline;
  box-pack: baseline;
  /* Modern browsers */
  justify-content: baseline;
}
.hbox.stretch,
.vbox.stretch,
.stretch {
  /* Old browsers */
  -webkit-box-pack: stretch;
  -moz-box-pack: stretch;
  box-pack: stretch;
  /* Modern browsers */
  justify-content: stretch;
}
.hbox.align-start,
.vbox.align-start,
.align-start {
  /* Old browsers */
  -webkit-box-align: start;
  -moz-box-align: start;
  box-align: start;
  /* Modern browsers */
  align-items: flex-start;
}
.hbox.align-end,
.vbox.align-end,
.align-end {
  /* Old browsers */
  -webkit-box-align: end;
  -moz-box-align: end;
  box-align: end;
  /* Modern browsers */
  align-items: flex-end;
}
.hbox.align-center,
.vbox.align-center,
.align-center {
  /* Old browsers */
  -webkit-box-align: center;
  -moz-box-align: center;
  box-align: center;
  /* Modern browsers */
  align-items: center;
}
.hbox.align-baseline,
.vbox.align-baseline,
.align-baseline {
  /* Old browsers */
  -webkit-box-align: baseline;
  -moz-box-align: baseline;
  box-align: baseline;
  /* Modern browsers */
  align-items: baseline;
}
.hbox.align-stretch,
.vbox.align-stretch,
.align-stretch {
  /* Old browsers */
  -webkit-box-align: stretch;
  -moz-box-align: stretch;
  box-align: stretch;
  /* Modern browsers */
  align-items: stretch;
}
div.error {
  margin: 2em;
  text-align: center;
}
div.error > h1 {
  font-size: 500%;
  line-height: normal;
}
div.error > p {
  font-size: 200%;
  line-height: normal;
}
div.traceback-wrapper {
  text-align: left;
  max-width: 800px;
  margin: auto;
}
div.traceback-wrapper pre.traceback {
  max-height: 600px;
  overflow: auto;
}
/**
 * Primary styles
 *
 * Author: Jupyter Development Team
 */
body {
  background-color: #fff;
  /* This makes sure that the body covers the entire window and needs to
       be in a different element than the display: box in wrapper below */
  position: absolute;
  left: 0px;
  right: 0px;
  top: 0px;
  bottom: 0px;
  overflow: visible;
}
body > #header {
  /* Initially hidden to prevent FLOUC */
  display: none;
  background-color: #fff;
  /* Display over codemirror */
  position: relative;
  z-index: 100;
}
body > #header #header-container {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  padding: 5px;
  padding-bottom: 5px;
  padding-top: 5px;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
}
body > #header .header-bar {
  width: 100%;
  height: 1px;
  background: #e7e7e7;
  margin-bottom: -1px;
}
@media print {
  body > #header {
    display: none !important;
  }
}
#header-spacer {
  width: 100%;
  visibility: hidden;
}
@media print {
  #header-spacer {
    display: none;
  }
}
#ipython_notebook {
  padding-left: 0px;
  padding-top: 1px;
  padding-bottom: 1px;
}
[dir="rtl"] #ipython_notebook {
  margin-right: 10px;
  margin-left: 0;
}
[dir="rtl"] #ipython_notebook.pull-left {
  float: right !important;
  float: right;
}
.flex-spacer {
  flex: 1;
}
#noscript {
  width: auto;
  padding-top: 16px;
  padding-bottom: 16px;
  text-align: center;
  font-size: 22px;
  color: red;
  font-weight: bold;
}
#ipython_notebook img {
  height: 28px;
}
#site {
  width: 100%;
  display: none;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  overflow: auto;
}
@media print {
  #site {
    height: auto !important;
  }
}
/* Smaller buttons */
.ui-button .ui-button-text {
  padding: 0.2em 0.8em;
  font-size: 77%;
}
input.ui-button {
  padding: 0.3em 0.9em;
}
span#kernel_logo_widget {
  margin: 0 10px;
}
span#login_widget {
  float: right;
}
[dir="rtl"] span#login_widget {
  float: left;
}
span#login_widget > .button,
#logout {
  color: #333;
  background-color: #fff;
  border-color: #ccc;
}
span#login_widget > .button:focus,
#logout:focus,
span#login_widget > .button.focus,
#logout.focus {
  color: #333;
  background-color: #e6e6e6;
  border-color: #8c8c8c;
}
span#login_widget > .button:hover,
#logout:hover {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
span#login_widget > .button:active,
#logout:active,
span#login_widget > .button.active,
#logout.active,
.open > .dropdown-togglespan#login_widget > .button,
.open > .dropdown-toggle#logout {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
span#login_widget > .button:active:hover,
#logout:active:hover,
span#login_widget > .button.active:hover,
#logout.active:hover,
.open > .dropdown-togglespan#login_widget > .button:hover,
.open > .dropdown-toggle#logout:hover,
span#login_widget > .button:active:focus,
#logout:active:focus,
span#login_widget > .button.active:focus,
#logout.active:focus,
.open > .dropdown-togglespan#login_widget > .button:focus,
.open > .dropdown-toggle#logout:focus,
span#login_widget > .button:active.focus,
#logout:active.focus,
span#login_widget > .button.active.focus,
#logout.active.focus,
.open > .dropdown-togglespan#login_widget > .button.focus,
.open > .dropdown-toggle#logout.focus {
  color: #333;
  background-color: #d4d4d4;
  border-color: #8c8c8c;
}
span#login_widget > .button:active,
#logout:active,
span#login_widget > .button.active,
#logout.active,
.open > .dropdown-togglespan#login_widget > .button,
.open > .dropdown-toggle#logout {
  background-image: none;
}
span#login_widget > .button.disabled:hover,
#logout.disabled:hover,
span#login_widget > .button[disabled]:hover,
#logout[disabled]:hover,
fieldset[disabled] span#login_widget > .button:hover,
fieldset[disabled] #logout:hover,
span#login_widget > .button.disabled:focus,
#logout.disabled:focus,
span#login_widget > .button[disabled]:focus,
#logout[disabled]:focus,
fieldset[disabled] span#login_widget > .button:focus,
fieldset[disabled] #logout:focus,
span#login_widget > .button.disabled.focus,
#logout.disabled.focus,
span#login_widget > .button[disabled].focus,
#logout[disabled].focus,
fieldset[disabled] span#login_widget > .button.focus,
fieldset[disabled] #logout.focus {
  background-color: #fff;
  border-color: #ccc;
}
span#login_widget > .button .badge,
#logout .badge {
  color: #fff;
  background-color: #333;
}
.nav-header {
  text-transform: none;
}
#header > span {
  margin-top: 10px;
}
.modal_stretch .modal-dialog {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
  min-height: 80vh;
}
.modal_stretch .modal-dialog .modal-body {
  max-height: calc(100vh - 200px);
  overflow: auto;
  flex: 1;
}
.modal-header {
  cursor: move;
}
@media (min-width: 768px) {
  .modal .modal-dialog {
    width: 700px;
  }
}
@media (min-width: 768px) {
  select.form-control {
    margin-left: 12px;
    margin-right: 12px;
  }
}
/*!
*
* IPython auth
*
*/
.center-nav {
  display: inline-block;
  margin-bottom: -4px;
}
[dir="rtl"] .center-nav form.pull-left {
  float: right !important;
  float: right;
}
[dir="rtl"] .center-nav .navbar-text {
  float: right;
}
[dir="rtl"] .navbar-inner {
  text-align: right;
}
[dir="rtl"] div.text-left {
  text-align: right;
}
/*!
*
* IPython tree view
*
*/
/* We need an invisible input field on top of the sentense*/
/* "Drag file onto the list ..." */
.alternate_upload {
  background-color: none;
  display: inline;
}
.alternate_upload.form {
  padding: 0;
  margin: 0;
}
.alternate_upload input.fileinput {
  position: absolute;
  display: block;
  width: 100%;
  height: 100%;
  overflow: hidden;
  cursor: pointer;
  opacity: 0;
  z-index: 2;
}
.alternate_upload .btn-xs > input.fileinput {
  margin: -1px -5px;
}
.alternate_upload .btn-upload {
  position: relative;
  height: 22px;
}
::-webkit-file-upload-button {
  cursor: pointer;
}
/**
 * Primary styles
 *
 * Author: Jupyter Development Team
 */
ul#tabs {
  margin-bottom: 4px;
}
ul#tabs a {
  padding-top: 6px;
  padding-bottom: 4px;
}
[dir="rtl"] ul#tabs.nav-tabs > li {
  float: right;
}
[dir="rtl"] ul#tabs.nav.nav-tabs {
  padding-right: 0;
}
ul.breadcrumb a:focus,
ul.breadcrumb a:hover {
  text-decoration: none;
}
ul.breadcrumb i.icon-home {
  font-size: 16px;
  margin-right: 4px;
}
ul.breadcrumb span {
  color: #5e5e5e;
}
.list_toolbar {
  padding: 4px 0 4px 0;
  vertical-align: middle;
}
.list_toolbar .tree-buttons {
  padding-top: 1px;
}
[dir="rtl"] .list_toolbar .tree-buttons .pull-right {
  float: left !important;
  float: left;
}
[dir="rtl"] .list_toolbar .col-sm-4,
[dir="rtl"] .list_toolbar .col-sm-8 {
  float: right;
}
.dynamic-buttons {
  padding-top: 3px;
  display: inline-block;
}
.list_toolbar [class*="span"] {
  min-height: 24px;
}
.list_header {
  font-weight: bold;
  background-color: #EEE;
}
.list_placeholder {
  font-weight: bold;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 7px;
  padding-right: 7px;
}
.list_container {
  margin-top: 4px;
  margin-bottom: 20px;
  border: 1px solid #ddd;
  border-radius: 2px;
}
.list_container > div {
  border-bottom: 1px solid #ddd;
}
.list_container > div:hover .list-item {
  background-color: red;
}
.list_container > div:last-child {
  border: none;
}
.list_item:hover .list_item {
  background-color: #ddd;
}
.list_item a {
  text-decoration: none;
}
.list_item:hover {
  background-color: #fafafa;
}
.list_header > div,
.list_item > div {
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 7px;
  padding-right: 7px;
  line-height: 22px;
}
.list_header > div input,
.list_item > div input {
  margin-right: 7px;
  margin-left: 14px;
  vertical-align: text-bottom;
  line-height: 22px;
  position: relative;
  top: -1px;
}
.list_header > div .item_link,
.list_item > div .item_link {
  margin-left: -1px;
  vertical-align: baseline;
  line-height: 22px;
}
[dir="rtl"] .list_item > div input {
  margin-right: 0;
}
.new-file input[type=checkbox] {
  visibility: hidden;
}
.item_name {
  line-height: 22px;
  height: 24px;
}
.item_icon {
  font-size: 14px;
  color: #5e5e5e;
  margin-right: 7px;
  margin-left: 7px;
  line-height: 22px;
  vertical-align: baseline;
}
.item_modified {
  margin-right: 7px;
  margin-left: 7px;
}
[dir="rtl"] .item_modified.pull-right {
  float: left !important;
  float: left;
}
.item_buttons {
  line-height: 1em;
  margin-left: -5px;
}
.item_buttons .btn,
.item_buttons .btn-group,
.item_buttons .input-group {
  float: left;
}
.item_buttons > .btn,
.item_buttons > .btn-group,
.item_buttons > .input-group {
  margin-left: 5px;
}
.item_buttons .btn {
  min-width: 13ex;
}
.item_buttons .running-indicator {
  padding-top: 4px;
  color: #5cb85c;
}
.item_buttons .kernel-name {
  padding-top: 4px;
  color: #5bc0de;
  margin-right: 7px;
  float: left;
}
[dir="rtl"] .item_buttons.pull-right {
  float: left !important;
  float: left;
}
[dir="rtl"] .item_buttons .kernel-name {
  margin-left: 7px;
  float: right;
}
.toolbar_info {
  height: 24px;
  line-height: 24px;
}
.list_item input:not([type=checkbox]) {
  padding-top: 3px;
  padding-bottom: 3px;
  height: 22px;
  line-height: 14px;
  margin: 0px;
}
.highlight_text {
  color: blue;
}
#project_name {
  display: inline-block;
  padding-left: 7px;
  margin-left: -2px;
}
#project_name > .breadcrumb {
  padding: 0px;
  margin-bottom: 0px;
  background-color: transparent;
  font-weight: bold;
}
.sort_button {
  display: inline-block;
  padding-left: 7px;
}
[dir="rtl"] .sort_button.pull-right {
  float: left !important;
  float: left;
}
#tree-selector {
  padding-right: 0px;
}
#button-select-all {
  min-width: 50px;
}
[dir="rtl"] #button-select-all.btn {
  float: right ;
}
#select-all {
  margin-left: 7px;
  margin-right: 2px;
  margin-top: 2px;
  height: 16px;
}
[dir="rtl"] #select-all.pull-left {
  float: right !important;
  float: right;
}
.menu_icon {
  margin-right: 2px;
}
.tab-content .row {
  margin-left: 0px;
  margin-right: 0px;
}
.folder_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f114";
}
.folder_icon:before.fa-pull-left {
  margin-right: .3em;
}
.folder_icon:before.fa-pull-right {
  margin-left: .3em;
}
.folder_icon:before.pull-left {
  margin-right: .3em;
}
.folder_icon:before.pull-right {
  margin-left: .3em;
}
.notebook_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f02d";
  position: relative;
  top: -1px;
}
.notebook_icon:before.fa-pull-left {
  margin-right: .3em;
}
.notebook_icon:before.fa-pull-right {
  margin-left: .3em;
}
.notebook_icon:before.pull-left {
  margin-right: .3em;
}
.notebook_icon:before.pull-right {
  margin-left: .3em;
}
.running_notebook_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f02d";
  position: relative;
  top: -1px;
  color: #5cb85c;
}
.running_notebook_icon:before.fa-pull-left {
  margin-right: .3em;
}
.running_notebook_icon:before.fa-pull-right {
  margin-left: .3em;
}
.running_notebook_icon:before.pull-left {
  margin-right: .3em;
}
.running_notebook_icon:before.pull-right {
  margin-left: .3em;
}
.file_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f016";
  position: relative;
  top: -2px;
}
.file_icon:before.fa-pull-left {
  margin-right: .3em;
}
.file_icon:before.fa-pull-right {
  margin-left: .3em;
}
.file_icon:before.pull-left {
  margin-right: .3em;
}
.file_icon:before.pull-right {
  margin-left: .3em;
}
#notebook_toolbar .pull-right {
  padding-top: 0px;
  margin-right: -1px;
}
ul#new-menu {
  left: auto;
  right: 0;
}
#new-menu .dropdown-header {
  font-size: 10px;
  border-bottom: 1px solid #e5e5e5;
  padding: 0 0 3px;
  margin: -3px 20px 0;
}
.kernel-menu-icon {
  padding-right: 12px;
  width: 24px;
  content: "\f096";
}
.kernel-menu-icon:before {
  content: "\f096";
}
.kernel-menu-icon-current:before {
  content: "\f00c";
}
#tab_content {
  padding-top: 20px;
}
#running .panel-group .panel {
  margin-top: 3px;
  margin-bottom: 1em;
}
#running .panel-group .panel .panel-heading {
  background-color: #EEE;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 7px;
  padding-right: 7px;
  line-height: 22px;
}
#running .panel-group .panel .panel-heading a:focus,
#running .panel-group .panel .panel-heading a:hover {
  text-decoration: none;
}
#running .panel-group .panel .panel-body {
  padding: 0px;
}
#running .panel-group .panel .panel-body .list_container {
  margin-top: 0px;
  margin-bottom: 0px;
  border: 0px;
  border-radius: 0px;
}
#running .panel-group .panel .panel-body .list_container .list_item {
  border-bottom: 1px solid #ddd;
}
#running .panel-group .panel .panel-body .list_container .list_item:last-child {
  border-bottom: 0px;
}
.delete-button {
  display: none;
}
.duplicate-button {
  display: none;
}
.rename-button {
  display: none;
}
.move-button {
  display: none;
}
.download-button {
  display: none;
}
.shutdown-button {
  display: none;
}
.dynamic-instructions {
  display: inline-block;
  padding-top: 4px;
}
/*!
*
* IPython text editor webapp
*
*/
.selected-keymap i.fa {
  padding: 0px 5px;
}
.selected-keymap i.fa:before {
  content: "\f00c";
}
#mode-menu {
  overflow: auto;
  max-height: 20em;
}
.edit_app #header {
  -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
}
.edit_app #menubar .navbar {
  /* Use a negative 1 bottom margin, so the border overlaps the border of the
    header */
  margin-bottom: -1px;
}
.dirty-indicator {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  width: 20px;
}
.dirty-indicator.fa-pull-left {
  margin-right: .3em;
}
.dirty-indicator.fa-pull-right {
  margin-left: .3em;
}
.dirty-indicator.pull-left {
  margin-right: .3em;
}
.dirty-indicator.pull-right {
  margin-left: .3em;
}
.dirty-indicator-dirty {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  width: 20px;
}
.dirty-indicator-dirty.fa-pull-left {
  margin-right: .3em;
}
.dirty-indicator-dirty.fa-pull-right {
  margin-left: .3em;
}
.dirty-indicator-dirty.pull-left {
  margin-right: .3em;
}
.dirty-indicator-dirty.pull-right {
  margin-left: .3em;
}
.dirty-indicator-clean {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  width: 20px;
}
.dirty-indicator-clean.fa-pull-left {
  margin-right: .3em;
}
.dirty-indicator-clean.fa-pull-right {
  margin-left: .3em;
}
.dirty-indicator-clean.pull-left {
  margin-right: .3em;
}
.dirty-indicator-clean.pull-right {
  margin-left: .3em;
}
.dirty-indicator-clean:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f00c";
}
.dirty-indicator-clean:before.fa-pull-left {
  margin-right: .3em;
}
.dirty-indicator-clean:before.fa-pull-right {
  margin-left: .3em;
}
.dirty-indicator-clean:before.pull-left {
  margin-right: .3em;
}
.dirty-indicator-clean:before.pull-right {
  margin-left: .3em;
}
#filename {
  font-size: 16pt;
  display: table;
  padding: 0px 5px;
}
#current-mode {
  padding-left: 5px;
  padding-right: 5px;
}
#texteditor-backdrop {
  padding-top: 20px;
  padding-bottom: 20px;
}
@media not print {
  #texteditor-backdrop {
    background-color: #EEE;
  }
}
@media print {
  #texteditor-backdrop #texteditor-container .CodeMirror-gutter,
  #texteditor-backdrop #texteditor-container .CodeMirror-gutters {
    background-color: #fff;
  }
}
@media not print {
  #texteditor-backdrop #texteditor-container .CodeMirror-gutter,
  #texteditor-backdrop #texteditor-container .CodeMirror-gutters {
    background-color: #fff;
  }
}
@media not print {
  #texteditor-backdrop #texteditor-container {
    padding: 0px;
    background-color: #fff;
    -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
    box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  }
}
.CodeMirror-dialog {
  background-color: #fff;
}
/*!
*
* IPython notebook
*
*/
/* CSS font colors for translated ANSI escape sequences */
/* The color values are a mix of
   http://www.xcolors.net/dl/baskerville-ivorylight and
   http://www.xcolors.net/dl/euphrasia */
.ansi-black-fg {
  color: #3E424D;
}
.ansi-black-bg {
  background-color: #3E424D;
}
.ansi-black-intense-fg {
  color: #282C36;
}
.ansi-black-intense-bg {
  background-color: #282C36;
}
.ansi-red-fg {
  color: #E75C58;
}
.ansi-red-bg {
  background-color: #E75C58;
}
.ansi-red-intense-fg {
  color: #B22B31;
}
.ansi-red-intense-bg {
  background-color: #B22B31;
}
.ansi-green-fg {
  color: #00A250;
}
.ansi-green-bg {
  background-color: #00A250;
}
.ansi-green-intense-fg {
  color: #007427;
}
.ansi-green-intense-bg {
  background-color: #007427;
}
.ansi-yellow-fg {
  color: #DDB62B;
}
.ansi-yellow-bg {
  background-color: #DDB62B;
}
.ansi-yellow-intense-fg {
  color: #B27D12;
}
.ansi-yellow-intense-bg {
  background-color: #B27D12;
}
.ansi-blue-fg {
  color: #208FFB;
}
.ansi-blue-bg {
  background-color: #208FFB;
}
.ansi-blue-intense-fg {
  color: #0065CA;
}
.ansi-blue-intense-bg {
  background-color: #0065CA;
}
.ansi-magenta-fg {
  color: #D160C4;
}
.ansi-magenta-bg {
  background-color: #D160C4;
}
.ansi-magenta-intense-fg {
  color: #A03196;
}
.ansi-magenta-intense-bg {
  background-color: #A03196;
}
.ansi-cyan-fg {
  color: #60C6C8;
}
.ansi-cyan-bg {
  background-color: #60C6C8;
}
.ansi-cyan-intense-fg {
  color: #258F8F;
}
.ansi-cyan-intense-bg {
  background-color: #258F8F;
}
.ansi-white-fg {
  color: #C5C1B4;
}
.ansi-white-bg {
  background-color: #C5C1B4;
}
.ansi-white-intense-fg {
  color: #A1A6B2;
}
.ansi-white-intense-bg {
  background-color: #A1A6B2;
}
.ansi-default-inverse-fg {
  color: #FFFFFF;
}
.ansi-default-inverse-bg {
  background-color: #000000;
}
.ansi-bold {
  font-weight: bold;
}
.ansi-underline {
  text-decoration: underline;
}
/* The following styles are deprecated an will be removed in a future version */
.ansibold {
  font-weight: bold;
}
.ansi-inverse {
  outline: 0.5px dotted;
}
/* use dark versions for foreground, to improve visibility */
.ansiblack {
  color: black;
}
.ansired {
  color: darkred;
}
.ansigreen {
  color: darkgreen;
}
.ansiyellow {
  color: #c4a000;
}
.ansiblue {
  color: darkblue;
}
.ansipurple {
  color: darkviolet;
}
.ansicyan {
  color: steelblue;
}
.ansigray {
  color: gray;
}
/* and light for background, for the same reason */
.ansibgblack {
  background-color: black;
}
.ansibgred {
  background-color: red;
}
.ansibggreen {
  background-color: green;
}
.ansibgyellow {
  background-color: yellow;
}
.ansibgblue {
  background-color: blue;
}
.ansibgpurple {
  background-color: magenta;
}
.ansibgcyan {
  background-color: cyan;
}
.ansibggray {
  background-color: gray;
}
div.cell {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
  border-radius: 2px;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  border-width: 1px;
  border-style: solid;
  border-color: transparent;
  width: 100%;
  padding: 5px;
  /* This acts as a spacer between cells, that is outside the border */
  margin: 0px;
  outline: none;
  position: relative;
  overflow: visible;
}
div.cell:before {
  position: absolute;
  display: block;
  top: -1px;
  left: -1px;
  width: 5px;
  height: calc(100% +  2px);
  content: '';
  background: transparent;
}
div.cell.jupyter-soft-selected {
  border-left-color: #E3F2FD;
  border-left-width: 1px;
  padding-left: 5px;
  border-right-color: #E3F2FD;
  border-right-width: 1px;
  background: #E3F2FD;
}
@media print {
  div.cell.jupyter-soft-selected {
    border-color: transparent;
  }
}
div.cell.selected,
div.cell.selected.jupyter-soft-selected {
  border-color: #ababab;
}
div.cell.selected:before,
div.cell.selected.jupyter-soft-selected:before {
  position: absolute;
  display: block;
  top: -1px;
  left: -1px;
  width: 5px;
  height: calc(100% +  2px);
  content: '';
  background: #42A5F5;
}
@media print {
  div.cell.selected,
  div.cell.selected.jupyter-soft-selected {
    border-color: transparent;
  }
}
.edit_mode div.cell.selected {
  border-color: #66BB6A;
}
.edit_mode div.cell.selected:before {
  position: absolute;
  display: block;
  top: -1px;
  left: -1px;
  width: 5px;
  height: calc(100% +  2px);
  content: '';
  background: #66BB6A;
}
@media print {
  .edit_mode div.cell.selected {
    border-color: transparent;
  }
}
.prompt {
  /* This needs to be wide enough for 3 digit prompt numbers: In[100]: */
  min-width: 14ex;
  /* This padding is tuned to match the padding on the CodeMirror editor. */
  padding: 0.4em;
  margin: 0px;
  font-family: monospace;
  text-align: right;
  /* This has to match that of the the CodeMirror class line-height below */
  line-height: 1.21429em;
  /* Don't highlight prompt number selection */
  -webkit-touch-callout: none;
  -webkit-user-select: none;
  -khtml-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
  /* Use default cursor */
  cursor: default;
}
@media (max-width: 540px) {
  .prompt {
    text-align: left;
  }
}
div.inner_cell {
  min-width: 0;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
  /* Old browsers */
  -webkit-box-flex: 1;
  -moz-box-flex: 1;
  box-flex: 1;
  /* Modern browsers */
  flex: 1;
}
/* input_area and input_prompt must match in top border and margin for alignment */
div.input_area {
  border: 1px solid #cfcfcf;
  border-radius: 2px;
  background: #f7f7f7;
  line-height: 1.21429em;
}
/* This is needed so that empty prompt areas can collapse to zero height when there
   is no content in the output_subarea and the prompt. The main purpose of this is
   to make sure that empty JavaScript output_subareas have no height. */
div.prompt:empty {
  padding-top: 0;
  padding-bottom: 0;
}
div.unrecognized_cell {
  padding: 5px 5px 5px 0px;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
}
div.unrecognized_cell .inner_cell {
  border-radius: 2px;
  padding: 5px;
  font-weight: bold;
  color: red;
  border: 1px solid #cfcfcf;
  background: #eaeaea;
}
div.unrecognized_cell .inner_cell a {
  color: inherit;
  text-decoration: none;
}
div.unrecognized_cell .inner_cell a:hover {
  color: inherit;
  text-decoration: none;
}
@media (max-width: 540px) {
  div.unrecognized_cell > div.prompt {
    display: none;
  }
}
div.code_cell {
  /* avoid page breaking on code cells when printing */
}
@media print {
  div.code_cell {
    page-break-inside: avoid;
  }
}
/* any special styling for code cells that are currently running goes here */
div.input {
  page-break-inside: avoid;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
}
@media (max-width: 540px) {
  div.input {
    /* Old browsers */
    display: -webkit-box;
    -webkit-box-orient: vertical;
    -webkit-box-align: stretch;
    display: -moz-box;
    -moz-box-orient: vertical;
    -moz-box-align: stretch;
    display: box;
    box-orient: vertical;
    box-align: stretch;
    /* Modern browsers */
    display: flex;
    flex-direction: column;
    align-items: stretch;
  }
}
/* input_area and input_prompt must match in top border and margin for alignment */
div.input_prompt {
  color: #303F9F;
  border-top: 1px solid transparent;
}
div.input_area > div.highlight {
  margin: 0.4em;
  border: none;
  padding: 0px;
  background-color: transparent;
}
div.input_area > div.highlight > pre {
  margin: 0px;
  border: none;
  padding: 0px;
  background-color: transparent;
}
/* The following gets added to the <head> if it is detected that the user has a
 * monospace font with inconsistent normal/bold/italic height.  See
 * notebookmain.js.  Such fonts will have keywords vertically offset with
 * respect to the rest of the text.  The user should select a better font.
 * See: https://github.com/ipython/ipython/issues/1503
 *
 * .CodeMirror span {
 *      vertical-align: bottom;
 * }
 */
.CodeMirror {
  line-height: 1.21429em;
  /* Changed from 1em to our global default */
  font-size: 14px;
  height: auto;
  /* Changed to auto to autogrow */
  background: none;
  /* Changed from white to allow our bg to show through */
}
.CodeMirror-scroll {
  /*  The CodeMirror docs are a bit fuzzy on if overflow-y should be hidden or visible.*/
  /*  We have found that if it is visible, vertical scrollbars appear with font size changes.*/
  overflow-y: hidden;
  overflow-x: auto;
}
.CodeMirror-lines {
  /* In CM2, this used to be 0.4em, but in CM3 it went to 4px. We need the em value because */
  /* we have set a different line-height and want this to scale with that. */
  /* Note that this should set vertical padding only, since CodeMirror assumes
       that horizontal padding will be set on CodeMirror pre */
  padding: 0.4em 0;
}
.CodeMirror-linenumber {
  padding: 0 8px 0 4px;
}
.CodeMirror-gutters {
  border-bottom-left-radius: 2px;
  border-top-left-radius: 2px;
}
.CodeMirror pre {
  /* In CM3 this went to 4px from 0 in CM2. This sets horizontal padding only,
    use .CodeMirror-lines for vertical */
  padding: 0 0.4em;
  border: 0;
  border-radius: 0;
}
.CodeMirror-cursor {
  border-left: 1.4px solid black;
}
@media screen and (min-width: 2138px) and (max-width: 4319px) {
  .CodeMirror-cursor {
    border-left: 2px solid black;
  }
}
@media screen and (min-width: 4320px) {
  .CodeMirror-cursor {
    border-left: 4px solid black;
  }
}
/*

Original style from softwaremaniacs.org (c) Ivan Sagalaev <Maniac@SoftwareManiacs.Org>
Adapted from GitHub theme

*/
.highlight-base {
  color: #000;
}
.highlight-variable {
  color: #000;
}
.highlight-variable-2 {
  color: #1a1a1a;
}
.highlight-variable-3 {
  color: #333333;
}
.highlight-string {
  color: #BA2121;
}
.highlight-comment {
  color: #408080;
  font-style: italic;
}
.highlight-number {
  color: #080;
}
.highlight-atom {
  color: #88F;
}
.highlight-keyword {
  color: #008000;
  font-weight: bold;
}
.highlight-builtin {
  color: #008000;
}
.highlight-error {
  color: #f00;
}
.highlight-operator {
  color: #AA22FF;
  font-weight: bold;
}
.highlight-meta {
  color: #AA22FF;
}
/* previously not defined, copying from default codemirror */
.highlight-def {
  color: #00f;
}
.highlight-string-2 {
  color: #f50;
}
.highlight-qualifier {
  color: #555;
}
.highlight-bracket {
  color: #997;
}
.highlight-tag {
  color: #170;
}
.highlight-attribute {
  color: #00c;
}
.highlight-header {
  color: blue;
}
.highlight-quote {
  color: #090;
}
.highlight-link {
  color: #00c;
}
/* apply the same style to codemirror */
.cm-s-ipython span.cm-keyword {
  color: #008000;
  font-weight: bold;
}
.cm-s-ipython span.cm-atom {
  color: #88F;
}
.cm-s-ipython span.cm-number {
  color: #080;
}
.cm-s-ipython span.cm-def {
  color: #00f;
}
.cm-s-ipython span.cm-variable {
  color: #000;
}
.cm-s-ipython span.cm-operator {
  color: #AA22FF;
  font-weight: bold;
}
.cm-s-ipython span.cm-variable-2 {
  color: #1a1a1a;
}
.cm-s-ipython span.cm-variable-3 {
  color: #333333;
}
.cm-s-ipython span.cm-comment {
  color: #408080;
  font-style: italic;
}
.cm-s-ipython span.cm-string {
  color: #BA2121;
}
.cm-s-ipython span.cm-string-2 {
  color: #f50;
}
.cm-s-ipython span.cm-meta {
  color: #AA22FF;
}
.cm-s-ipython span.cm-qualifier {
  color: #555;
}
.cm-s-ipython span.cm-builtin {
  color: #008000;
}
.cm-s-ipython span.cm-bracket {
  color: #997;
}
.cm-s-ipython span.cm-tag {
  color: #170;
}
.cm-s-ipython span.cm-attribute {
  color: #00c;
}
.cm-s-ipython span.cm-header {
  color: blue;
}
.cm-s-ipython span.cm-quote {
  color: #090;
}
.cm-s-ipython span.cm-link {
  color: #00c;
}
.cm-s-ipython span.cm-error {
  color: #f00;
}
.cm-s-ipython span.cm-tab {
  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADAAAAAMCAYAAAAkuj5RAAAAAXNSR0IArs4c6QAAAGFJREFUSMft1LsRQFAQheHPowAKoACx3IgEKtaEHujDjORSgWTH/ZOdnZOcM/sgk/kFFWY0qV8foQwS4MKBCS3qR6ixBJvElOobYAtivseIE120FaowJPN75GMu8j/LfMwNjh4HUpwg4LUAAAAASUVORK5CYII=);
  background-position: right;
  background-repeat: no-repeat;
}
div.output_wrapper {
  /* this position must be relative to enable descendents to be absolute within it */
  position: relative;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
  z-index: 1;
}
/* class for the output area when it should be height-limited */
div.output_scroll {
  /* ideally, this would be max-height, but FF barfs all over that */
  height: 24em;
  /* FF needs this *and the wrapper* to specify full width, or it will shrinkwrap */
  width: 100%;
  overflow: auto;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 2px 8px rgba(0, 0, 0, 0.8);
  box-shadow: inset 0 2px 8px rgba(0, 0, 0, 0.8);
  display: block;
}
/* output div while it is collapsed */
div.output_collapsed {
  margin: 0px;
  padding: 0px;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
}
div.out_prompt_overlay {
  height: 100%;
  padding: 0px 0.4em;
  position: absolute;
  border-radius: 2px;
}
div.out_prompt_overlay:hover {
  /* use inner shadow to get border that is computed the same on WebKit/FF */
  -webkit-box-shadow: inset 0 0 1px #000;
  box-shadow: inset 0 0 1px #000;
  background: rgba(240, 240, 240, 0.5);
}
div.output_prompt {
  color: #D84315;
}
/* This class is the outer container of all output sections. */
div.output_area {
  padding: 0px;
  page-break-inside: avoid;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
}
div.output_area .MathJax_Display {
  text-align: left !important;
}
div.output_area .rendered_html table {
  margin-left: 0;
  margin-right: 0;
}
div.output_area .rendered_html img {
  margin-left: 0;
  margin-right: 0;
}
div.output_area img,
div.output_area svg {
  max-width: 100%;
  height: auto;
}
div.output_area img.unconfined,
div.output_area svg.unconfined {
  max-width: none;
}
div.output_area .mglyph > img {
  max-width: none;
}
/* This is needed to protect the pre formating from global settings such
   as that of bootstrap */
.output {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
}
@media (max-width: 540px) {
  div.output_area {
    /* Old browsers */
    display: -webkit-box;
    -webkit-box-orient: vertical;
    -webkit-box-align: stretch;
    display: -moz-box;
    -moz-box-orient: vertical;
    -moz-box-align: stretch;
    display: box;
    box-orient: vertical;
    box-align: stretch;
    /* Modern browsers */
    display: flex;
    flex-direction: column;
    align-items: stretch;
  }
}
div.output_area pre {
  margin: 0;
  padding: 1px 0 1px 0;
  border: 0;
  vertical-align: baseline;
  color: black;
  background-color: transparent;
  border-radius: 0;
}
/* This class is for the output subarea inside the output_area and after
   the prompt div. */
div.output_subarea {
  overflow-x: auto;
  padding: 0.4em;
  /* Old browsers */
  -webkit-box-flex: 1;
  -moz-box-flex: 1;
  box-flex: 1;
  /* Modern browsers */
  flex: 1;
  max-width: calc(100% - 14ex);
}
div.output_scroll div.output_subarea {
  overflow-x: visible;
}
/* The rest of the output_* classes are for special styling of the different
   output types */
/* all text output has this class: */
div.output_text {
  text-align: left;
  color: #000;
  /* This has to match that of the the CodeMirror class line-height below */
  line-height: 1.21429em;
}
/* stdout/stderr are 'text' as well as 'stream', but execute_result/error are *not* streams */
div.output_stderr {
  background: #fdd;
  /* very light red background for stderr */
}
div.output_latex {
  text-align: left;
}
/* Empty output_javascript divs should have no height */
div.output_javascript:empty {
  padding: 0;
}
.js-error {
  color: darkred;
}
/* raw_input styles */
div.raw_input_container {
  line-height: 1.21429em;
  padding-top: 5px;
}
pre.raw_input_prompt {
  /* nothing needed here. */
}
input.raw_input {
  font-family: monospace;
  font-size: inherit;
  color: inherit;
  width: auto;
  /* make sure input baseline aligns with prompt */
  vertical-align: baseline;
  /* padding + margin = 0.5em between prompt and cursor */
  padding: 0em 0.25em;
  margin: 0em 0.25em;
}
input.raw_input:focus {
  box-shadow: none;
}
p.p-space {
  margin-bottom: 10px;
}
div.output_unrecognized {
  padding: 5px;
  font-weight: bold;
  color: red;
}
div.output_unrecognized a {
  color: inherit;
  text-decoration: none;
}
div.output_unrecognized a:hover {
  color: inherit;
  text-decoration: none;
}
.rendered_html {
  color: #000;
  /* any extras will just be numbers: */
}
.rendered_html em {
  font-style: italic;
}
.rendered_html strong {
  font-weight: bold;
}
.rendered_html u {
  text-decoration: underline;
}
.rendered_html :link {
  text-decoration: underline;
}
.rendered_html :visited {
  text-decoration: underline;
}
.rendered_html h1 {
  font-size: 185.7%;
  margin: 1.08em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
}
.rendered_html h2 {
  font-size: 157.1%;
  margin: 1.27em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
}
.rendered_html h3 {
  font-size: 128.6%;
  margin: 1.55em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
}
.rendered_html h4 {
  font-size: 100%;
  margin: 2em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
}
.rendered_html h5 {
  font-size: 100%;
  margin: 2em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
  font-style: italic;
}
.rendered_html h6 {
  font-size: 100%;
  margin: 2em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
  font-style: italic;
}
.rendered_html h1:first-child {
  margin-top: 0.538em;
}
.rendered_html h2:first-child {
  margin-top: 0.636em;
}
.rendered_html h3:first-child {
  margin-top: 0.777em;
}
.rendered_html h4:first-child {
  margin-top: 1em;
}
.rendered_html h5:first-child {
  margin-top: 1em;
}
.rendered_html h6:first-child {
  margin-top: 1em;
}
.rendered_html ul:not(.list-inline),
.rendered_html ol:not(.list-inline) {
  padding-left: 2em;
}
.rendered_html ul {
  list-style: disc;
}
.rendered_html ul ul {
  list-style: square;
  margin-top: 0;
}
.rendered_html ul ul ul {
  list-style: circle;
}
.rendered_html ol {
  list-style: decimal;
}
.rendered_html ol ol {
  list-style: upper-alpha;
  margin-top: 0;
}
.rendered_html ol ol ol {
  list-style: lower-alpha;
}
.rendered_html ol ol ol ol {
  list-style: lower-roman;
}
.rendered_html ol ol ol ol ol {
  list-style: decimal;
}
.rendered_html * + ul {
  margin-top: 1em;
}
.rendered_html * + ol {
  margin-top: 1em;
}
.rendered_html hr {
  color: black;
  background-color: black;
}
.rendered_html pre {
  margin: 1em 2em;
  padding: 0px;
  background-color: #fff;
}
.rendered_html code {
  background-color: #eff0f1;
}
.rendered_html p code {
  padding: 1px 5px;
}
.rendered_html pre code {
  background-color: #fff;
}
.rendered_html pre,
.rendered_html code {
  border: 0;
  color: #000;
  font-size: 100%;
}
.rendered_html blockquote {
  margin: 1em 2em;
}
.rendered_html table {
  margin-left: auto;
  margin-right: auto;
  border: none;
  border-collapse: collapse;
  border-spacing: 0;
  color: black;
  font-size: 12px;
  table-layout: fixed;
}
.rendered_html thead {
  border-bottom: 1px solid black;
  vertical-align: bottom;
}
.rendered_html tr,
.rendered_html th,
.rendered_html td {
  text-align: right;
  vertical-align: middle;
  padding: 0.5em 0.5em;
  line-height: normal;
  white-space: normal;
  max-width: none;
  border: none;
}
.rendered_html th {
  font-weight: bold;
}
.rendered_html tbody tr:nth-child(odd) {
  background: #f5f5f5;
}
.rendered_html tbody tr:hover {
  background: rgba(66, 165, 245, 0.2);
}
.rendered_html * + table {
  margin-top: 1em;
}
.rendered_html p {
  text-align: left;
}
.rendered_html * + p {
  margin-top: 1em;
}
.rendered_html img {
  display: block;
  margin-left: auto;
  margin-right: auto;
}
.rendered_html * + img {
  margin-top: 1em;
}
.rendered_html img,
.rendered_html svg {
  max-width: 100%;
  height: auto;
}
.rendered_html img.unconfined,
.rendered_html svg.unconfined {
  max-width: none;
}
.rendered_html .alert {
  margin-bottom: initial;
}
.rendered_html * + .alert {
  margin-top: 1em;
}
[dir="rtl"] .rendered_html p {
  text-align: right;
}
div.text_cell {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
}
@media (max-width: 540px) {
  div.text_cell > div.prompt {
    display: none;
  }
}
div.text_cell_render {
  /*font-family: "Helvetica Neue", Arial, Helvetica, Geneva, sans-serif;*/
  outline: none;
  resize: none;
  width: inherit;
  border-style: none;
  padding: 0.5em 0.5em 0.5em 0.4em;
  color: #000;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
}
a.anchor-link:link {
  text-decoration: none;
  padding: 0px 20px;
  visibility: hidden;
}
h1:hover .anchor-link,
h2:hover .anchor-link,
h3:hover .anchor-link,
h4:hover .anchor-link,
h5:hover .anchor-link,
h6:hover .anchor-link {
  visibility: visible;
}
.text_cell.rendered .input_area {
  display: none;
}
.text_cell.rendered .rendered_html {
  overflow-x: auto;
  overflow-y: hidden;
}
.text_cell.rendered .rendered_html tr,
.text_cell.rendered .rendered_html th,
.text_cell.rendered .rendered_html td {
  max-width: none;
}
.text_cell.unrendered .text_cell_render {
  display: none;
}
.text_cell .dropzone .input_area {
  border: 2px dashed #bababa;
  margin: -1px;
}
.cm-header-1,
.cm-header-2,
.cm-header-3,
.cm-header-4,
.cm-header-5,
.cm-header-6 {
  font-weight: bold;
  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
}
.cm-header-1 {
  font-size: 185.7%;
}
.cm-header-2 {
  font-size: 157.1%;
}
.cm-header-3 {
  font-size: 128.6%;
}
.cm-header-4 {
  font-size: 110%;
}
.cm-header-5 {
  font-size: 100%;
  font-style: italic;
}
.cm-header-6 {
  font-size: 100%;
  font-style: italic;
}
/*!
*
* IPython notebook webapp
*
*/
@media (max-width: 767px) {
  .notebook_app {
    padding-left: 0px;
    padding-right: 0px;
  }
}
#ipython-main-app {
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  height: 100%;
}
div#notebook_panel {
  margin: 0px;
  padding: 0px;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  height: 100%;
}
div#notebook {
  font-size: 14px;
  line-height: 20px;
  overflow-y: hidden;
  overflow-x: auto;
  width: 100%;
  /* This spaces the page away from the edge of the notebook area */
  padding-top: 20px;
  margin: 0px;
  outline: none;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  min-height: 100%;
}
@media not print {
  #notebook-container {
    padding: 15px;
    background-color: #fff;
    min-height: 0;
    -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
    box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  }
}
@media print {
  #notebook-container {
    width: 100%;
  }
}
div.ui-widget-content {
  border: 1px solid #ababab;
  outline: none;
}
pre.dialog {
  background-color: #f7f7f7;
  border: 1px solid #ddd;
  border-radius: 2px;
  padding: 0.4em;
  padding-left: 2em;
}
p.dialog {
  padding: 0.2em;
}
/* Word-wrap output correctly.  This is the CSS3 spelling, though Firefox seems
   to not honor it correctly.  Webkit browsers (Chrome, rekonq, Safari) do.
 */
pre,
code,
kbd,
samp {
  white-space: pre-wrap;
}
#fonttest {
  font-family: monospace;
}
p {
  margin-bottom: 0;
}
.end_space {
  min-height: 100px;
  transition: height .2s ease;
}
.notebook_app > #header {
  -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
}
@media not print {
  .notebook_app {
    background-color: #EEE;
  }
}
kbd {
  border-style: solid;
  border-width: 1px;
  box-shadow: none;
  margin: 2px;
  padding-left: 2px;
  padding-right: 2px;
  padding-top: 1px;
  padding-bottom: 1px;
}
.jupyter-keybindings {
  padding: 1px;
  line-height: 24px;
  border-bottom: 1px solid gray;
}
.jupyter-keybindings input {
  margin: 0;
  padding: 0;
  border: none;
}
.jupyter-keybindings i {
  padding: 6px;
}
.well code {
  background-color: #ffffff;
  border-color: #ababab;
  border-width: 1px;
  border-style: solid;
  padding: 2px;
  padding-top: 1px;
  padding-bottom: 1px;
}
/* CSS for the cell toolbar */
.celltoolbar {
  border: thin solid #CFCFCF;
  border-bottom: none;
  background: #EEE;
  border-radius: 2px 2px 0px 0px;
  width: 100%;
  height: 29px;
  padding-right: 4px;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
  /* Old browsers */
  -webkit-box-pack: end;
  -moz-box-pack: end;
  box-pack: end;
  /* Modern browsers */
  justify-content: flex-end;
  display: -webkit-flex;
}
@media print {
  .celltoolbar {
    display: none;
  }
}
.ctb_hideshow {
  display: none;
  vertical-align: bottom;
}
/* ctb_show is added to the ctb_hideshow div to show the cell toolbar.
   Cell toolbars are only shown when the ctb_global_show class is also set.
*/
.ctb_global_show .ctb_show.ctb_hideshow {
  display: block;
}
.ctb_global_show .ctb_show + .input_area,
.ctb_global_show .ctb_show + div.text_cell_input,
.ctb_global_show .ctb_show ~ div.text_cell_render {
  border-top-right-radius: 0px;
  border-top-left-radius: 0px;
}
.ctb_global_show .ctb_show ~ div.text_cell_render {
  border: 1px solid #cfcfcf;
}
.celltoolbar {
  font-size: 87%;
  padding-top: 3px;
}
.celltoolbar select {
  display: block;
  width: 100%;
  height: 32px;
  padding: 6px 12px;
  font-size: 13px;
  line-height: 1.42857143;
  color: #555555;
  background-color: #fff;
  background-image: none;
  border: 1px solid #ccc;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  -webkit-transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  -o-transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  height: 30px;
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
  width: inherit;
  font-size: inherit;
  height: 22px;
  padding: 0px;
  display: inline-block;
}
.celltoolbar select:focus {
  border-color: #66afe9;
  outline: 0;
  -webkit-box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, 0.6);
  box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, 0.6);
}
.celltoolbar select::-moz-placeholder {
  color: #999;
  opacity: 1;
}
.celltoolbar select:-ms-input-placeholder {
  color: #999;
}
.celltoolbar select::-webkit-input-placeholder {
  color: #999;
}
.celltoolbar select::-ms-expand {
  border: 0;
  background-color: transparent;
}
.celltoolbar select[disabled],
.celltoolbar select[readonly],
fieldset[disabled] .celltoolbar select {
  background-color: #eeeeee;
  opacity: 1;
}
.celltoolbar select[disabled],
fieldset[disabled] .celltoolbar select {
  cursor: not-allowed;
}
textarea.celltoolbar select {
  height: auto;
}
select.celltoolbar select {
  height: 30px;
  line-height: 30px;
}
textarea.celltoolbar select,
select[multiple].celltoolbar select {
  height: auto;
}
.celltoolbar label {
  margin-left: 5px;
  margin-right: 5px;
}
.tags_button_container {
  width: 100%;
  display: flex;
}
.tag-container {
  display: flex;
  flex-direction: row;
  flex-grow: 1;
  overflow: hidden;
  position: relative;
}
.tag-container > * {
  margin: 0 4px;
}
.remove-tag-btn {
  margin-left: 4px;
}
.tags-input {
  display: flex;
}
.cell-tag:last-child:after {
  content: "";
  position: absolute;
  right: 0;
  width: 40px;
  height: 100%;
  /* Fade to background color of cell toolbar */
  background: linear-gradient(to right, rgba(0, 0, 0, 0), #EEE);
}
.tags-input > * {
  margin-left: 4px;
}
.cell-tag,
.tags-input input,
.tags-input button {
  display: block;
  width: 100%;
  height: 32px;
  padding: 6px 12px;
  font-size: 13px;
  line-height: 1.42857143;
  color: #555555;
  background-color: #fff;
  background-image: none;
  border: 1px solid #ccc;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  -webkit-transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  -o-transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  height: 30px;
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
  box-shadow: none;
  width: inherit;
  font-size: inherit;
  height: 22px;
  line-height: 22px;
  padding: 0px 4px;
  display: inline-block;
}
.cell-tag:focus,
.tags-input input:focus,
.tags-input button:focus {
  border-color: #66afe9;
  outline: 0;
  -webkit-box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, 0.6);
  box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, 0.6);
}
.cell-tag::-moz-placeholder,
.tags-input input::-moz-placeholder,
.tags-input button::-moz-placeholder {
  color: #999;
  opacity: 1;
}
.cell-tag:-ms-input-placeholder,
.tags-input input:-ms-input-placeholder,
.tags-input button:-ms-input-placeholder {
  color: #999;
}
.cell-tag::-webkit-input-placeholder,
.tags-input input::-webkit-input-placeholder,
.tags-input button::-webkit-input-placeholder {
  color: #999;
}
.cell-tag::-ms-expand,
.tags-input input::-ms-expand,
.tags-input button::-ms-expand {
  border: 0;
  background-color: transparent;
}
.cell-tag[disabled],
.tags-input input[disabled],
.tags-input button[disabled],
.cell-tag[readonly],
.tags-input input[readonly],
.tags-input button[readonly],
fieldset[disabled] .cell-tag,
fieldset[disabled] .tags-input input,
fieldset[disabled] .tags-input button {
  background-color: #eeeeee;
  opacity: 1;
}
.cell-tag[disabled],
.tags-input input[disabled],
.tags-input button[disabled],
fieldset[disabled] .cell-tag,
fieldset[disabled] .tags-input input,
fieldset[disabled] .tags-input button {
  cursor: not-allowed;
}
textarea.cell-tag,
textarea.tags-input input,
textarea.tags-input button {
  height: auto;
}
select.cell-tag,
select.tags-input input,
select.tags-input button {
  height: 30px;
  line-height: 30px;
}
textarea.cell-tag,
textarea.tags-input input,
textarea.tags-input button,
select[multiple].cell-tag,
select[multiple].tags-input input,
select[multiple].tags-input button {
  height: auto;
}
.cell-tag,
.tags-input button {
  padding: 0px 4px;
}
.cell-tag {
  background-color: #fff;
  white-space: nowrap;
}
.tags-input input[type=text]:focus {
  outline: none;
  box-shadow: none;
  border-color: #ccc;
}
.completions {
  position: absolute;
  z-index: 110;
  overflow: hidden;
  border: 1px solid #ababab;
  border-radius: 2px;
  -webkit-box-shadow: 0px 6px 10px -1px #adadad;
  box-shadow: 0px 6px 10px -1px #adadad;
  line-height: 1;
}
.completions select {
  background: white;
  outline: none;
  border: none;
  padding: 0px;
  margin: 0px;
  overflow: auto;
  font-family: monospace;
  font-size: 110%;
  color: #000;
  width: auto;
}
.completions select option.context {
  color: #286090;
}
#kernel_logo_widget .current_kernel_logo {
  display: none;
  margin-top: -1px;
  margin-bottom: -1px;
  width: 32px;
  height: 32px;
}
[dir="rtl"] #kernel_logo_widget {
  float: left !important;
  float: left;
}
.modal .modal-body .move-path {
  display: flex;
  flex-direction: row;
  justify-content: space;
  align-items: center;
}
.modal .modal-body .move-path .server-root {
  padding-right: 20px;
}
.modal .modal-body .move-path .path-input {
  flex: 1;
}
#menubar {
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  margin-top: 1px;
}
#menubar .navbar {
  border-top: 1px;
  border-radius: 0px 0px 2px 2px;
  margin-bottom: 0px;
}
#menubar .navbar-toggle {
  float: left;
  padding-top: 7px;
  padding-bottom: 7px;
  border: none;
}
#menubar .navbar-collapse {
  clear: left;
}
[dir="rtl"] #menubar .navbar-toggle {
  float: right;
}
[dir="rtl"] #menubar .navbar-collapse {
  clear: right;
}
[dir="rtl"] #menubar .navbar-nav {
  float: right;
}
[dir="rtl"] #menubar .nav {
  padding-right: 0px;
}
[dir="rtl"] #menubar .navbar-nav > li {
  float: right;
}
[dir="rtl"] #menubar .navbar-right {
  float: left !important;
}
[dir="rtl"] ul.dropdown-menu {
  text-align: right;
  left: auto;
}
[dir="rtl"] ul#new-menu.dropdown-menu {
  right: auto;
  left: 0;
}
.nav-wrapper {
  border-bottom: 1px solid #e7e7e7;
}
i.menu-icon {
  padding-top: 4px;
}
[dir="rtl"] i.menu-icon.pull-right {
  float: left !important;
  float: left;
}
ul#help_menu li a {
  overflow: hidden;
  padding-right: 2.2em;
}
ul#help_menu li a i {
  margin-right: -1.2em;
}
[dir="rtl"] ul#help_menu li a {
  padding-left: 2.2em;
}
[dir="rtl"] ul#help_menu li a i {
  margin-right: 0;
  margin-left: -1.2em;
}
[dir="rtl"] ul#help_menu li a i.pull-right {
  float: left !important;
  float: left;
}
.dropdown-submenu {
  position: relative;
}
.dropdown-submenu > .dropdown-menu {
  top: 0;
  left: 100%;
  margin-top: -6px;
  margin-left: -1px;
}
[dir="rtl"] .dropdown-submenu > .dropdown-menu {
  right: 100%;
  margin-right: -1px;
}
.dropdown-submenu:hover > .dropdown-menu {
  display: block;
}
.dropdown-submenu > a:after {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  display: block;
  content: "\f0da";
  float: right;
  color: #333333;
  margin-top: 2px;
  margin-right: -10px;
}
.dropdown-submenu > a:after.fa-pull-left {
  margin-right: .3em;
}
.dropdown-submenu > a:after.fa-pull-right {
  margin-left: .3em;
}
.dropdown-submenu > a:after.pull-left {
  margin-right: .3em;
}
.dropdown-submenu > a:after.pull-right {
  margin-left: .3em;
}
[dir="rtl"] .dropdown-submenu > a:after {
  float: left;
  content: "\f0d9";
  margin-right: 0;
  margin-left: -10px;
}
.dropdown-submenu:hover > a:after {
  color: #262626;
}
.dropdown-submenu.pull-left {
  float: none;
}
.dropdown-submenu.pull-left > .dropdown-menu {
  left: -100%;
  margin-left: 10px;
}
#notification_area {
  float: right !important;
  float: right;
  z-index: 10;
}
[dir="rtl"] #notification_area {
  float: left !important;
  float: left;
}
.indicator_area {
  float: right !important;
  float: right;
  color: #777;
  margin-left: 5px;
  margin-right: 5px;
  width: 11px;
  z-index: 10;
  text-align: center;
  width: auto;
}
[dir="rtl"] .indicator_area {
  float: left !important;
  float: left;
}
#kernel_indicator {
  float: right !important;
  float: right;
  color: #777;
  margin-left: 5px;
  margin-right: 5px;
  width: 11px;
  z-index: 10;
  text-align: center;
  width: auto;
  border-left: 1px solid;
}
#kernel_indicator .kernel_indicator_name {
  padding-left: 5px;
  padding-right: 5px;
}
[dir="rtl"] #kernel_indicator {
  float: left !important;
  float: left;
  border-left: 0;
  border-right: 1px solid;
}
#modal_indicator {
  float: right !important;
  float: right;
  color: #777;
  margin-left: 5px;
  margin-right: 5px;
  width: 11px;
  z-index: 10;
  text-align: center;
  width: auto;
}
[dir="rtl"] #modal_indicator {
  float: left !important;
  float: left;
}
#readonly-indicator {
  float: right !important;
  float: right;
  color: #777;
  margin-left: 5px;
  margin-right: 5px;
  width: 11px;
  z-index: 10;
  text-align: center;
  width: auto;
  margin-top: 2px;
  margin-bottom: 0px;
  margin-left: 0px;
  margin-right: 0px;
  display: none;
}
.modal_indicator:before {
  width: 1.28571429em;
  text-align: center;
}
.edit_mode .modal_indicator:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f040";
}
.edit_mode .modal_indicator:before.fa-pull-left {
  margin-right: .3em;
}
.edit_mode .modal_indicator:before.fa-pull-right {
  margin-left: .3em;
}
.edit_mode .modal_indicator:before.pull-left {
  margin-right: .3em;
}
.edit_mode .modal_indicator:before.pull-right {
  margin-left: .3em;
}
.command_mode .modal_indicator:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: ' ';
}
.command_mode .modal_indicator:before.fa-pull-left {
  margin-right: .3em;
}
.command_mode .modal_indicator:before.fa-pull-right {
  margin-left: .3em;
}
.command_mode .modal_indicator:before.pull-left {
  margin-right: .3em;
}
.command_mode .modal_indicator:before.pull-right {
  margin-left: .3em;
}
.kernel_idle_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f10c";
}
.kernel_idle_icon:before.fa-pull-left {
  margin-right: .3em;
}
.kernel_idle_icon:before.fa-pull-right {
  margin-left: .3em;
}
.kernel_idle_icon:before.pull-left {
  margin-right: .3em;
}
.kernel_idle_icon:before.pull-right {
  margin-left: .3em;
}
.kernel_busy_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f111";
}
.kernel_busy_icon:before.fa-pull-left {
  margin-right: .3em;
}
.kernel_busy_icon:before.fa-pull-right {
  margin-left: .3em;
}
.kernel_busy_icon:before.pull-left {
  margin-right: .3em;
}
.kernel_busy_icon:before.pull-right {
  margin-left: .3em;
}
.kernel_dead_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f1e2";
}
.kernel_dead_icon:before.fa-pull-left {
  margin-right: .3em;
}
.kernel_dead_icon:before.fa-pull-right {
  margin-left: .3em;
}
.kernel_dead_icon:before.pull-left {
  margin-right: .3em;
}
.kernel_dead_icon:before.pull-right {
  margin-left: .3em;
}
.kernel_disconnected_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f127";
}
.kernel_disconnected_icon:before.fa-pull-left {
  margin-right: .3em;
}
.kernel_disconnected_icon:before.fa-pull-right {
  margin-left: .3em;
}
.kernel_disconnected_icon:before.pull-left {
  margin-right: .3em;
}
.kernel_disconnected_icon:before.pull-right {
  margin-left: .3em;
}
.notification_widget {
  color: #777;
  z-index: 10;
  background: rgba(240, 240, 240, 0.5);
  margin-right: 4px;
  color: #333;
  background-color: #fff;
  border-color: #ccc;
}
.notification_widget:focus,
.notification_widget.focus {
  color: #333;
  background-color: #e6e6e6;
  border-color: #8c8c8c;
}
.notification_widget:hover {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
.notification_widget:active,
.notification_widget.active,
.open > .dropdown-toggle.notification_widget {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
.notification_widget:active:hover,
.notification_widget.active:hover,
.open > .dropdown-toggle.notification_widget:hover,
.notification_widget:active:focus,
.notification_widget.active:focus,
.open > .dropdown-toggle.notification_widget:focus,
.notification_widget:active.focus,
.notification_widget.active.focus,
.open > .dropdown-toggle.notification_widget.focus {
  color: #333;
  background-color: #d4d4d4;
  border-color: #8c8c8c;
}
.notification_widget:active,
.notification_widget.active,
.open > .dropdown-toggle.notification_widget {
  background-image: none;
}
.notification_widget.disabled:hover,
.notification_widget[disabled]:hover,
fieldset[disabled] .notification_widget:hover,
.notification_widget.disabled:focus,
.notification_widget[disabled]:focus,
fieldset[disabled] .notification_widget:focus,
.notification_widget.disabled.focus,
.notification_widget[disabled].focus,
fieldset[disabled] .notification_widget.focus {
  background-color: #fff;
  border-color: #ccc;
}
.notification_widget .badge {
  color: #fff;
  background-color: #333;
}
.notification_widget.warning {
  color: #fff;
  background-color: #f0ad4e;
  border-color: #eea236;
}
.notification_widget.warning:focus,
.notification_widget.warning.focus {
  color: #fff;
  background-color: #ec971f;
  border-color: #985f0d;
}
.notification_widget.warning:hover {
  color: #fff;
  background-color: #ec971f;
  border-color: #d58512;
}
.notification_widget.warning:active,
.notification_widget.warning.active,
.open > .dropdown-toggle.notification_widget.warning {
  color: #fff;
  background-color: #ec971f;
  border-color: #d58512;
}
.notification_widget.warning:active:hover,
.notification_widget.warning.active:hover,
.open > .dropdown-toggle.notification_widget.warning:hover,
.notification_widget.warning:active:focus,
.notification_widget.warning.active:focus,
.open > .dropdown-toggle.notification_widget.warning:focus,
.notification_widget.warning:active.focus,
.notification_widget.warning.active.focus,
.open > .dropdown-toggle.notification_widget.warning.focus {
  color: #fff;
  background-color: #d58512;
  border-color: #985f0d;
}
.notification_widget.warning:active,
.notification_widget.warning.active,
.open > .dropdown-toggle.notification_widget.warning {
  background-image: none;
}
.notification_widget.warning.disabled:hover,
.notification_widget.warning[disabled]:hover,
fieldset[disabled] .notification_widget.warning:hover,
.notification_widget.warning.disabled:focus,
.notification_widget.warning[disabled]:focus,
fieldset[disabled] .notification_widget.warning:focus,
.notification_widget.warning.disabled.focus,
.notification_widget.warning[disabled].focus,
fieldset[disabled] .notification_widget.warning.focus {
  background-color: #f0ad4e;
  border-color: #eea236;
}
.notification_widget.warning .badge {
  color: #f0ad4e;
  background-color: #fff;
}
.notification_widget.success {
  color: #fff;
  background-color: #5cb85c;
  border-color: #4cae4c;
}
.notification_widget.success:focus,
.notification_widget.success.focus {
  color: #fff;
  background-color: #449d44;
  border-color: #255625;
}
.notification_widget.success:hover {
  color: #fff;
  background-color: #449d44;
  border-color: #398439;
}
.notification_widget.success:active,
.notification_widget.success.active,
.open > .dropdown-toggle.notification_widget.success {
  color: #fff;
  background-color: #449d44;
  border-color: #398439;
}
.notification_widget.success:active:hover,
.notification_widget.success.active:hover,
.open > .dropdown-toggle.notification_widget.success:hover,
.notification_widget.success:active:focus,
.notification_widget.success.active:focus,
.open > .dropdown-toggle.notification_widget.success:focus,
.notification_widget.success:active.focus,
.notification_widget.success.active.focus,
.open > .dropdown-toggle.notification_widget.success.focus {
  color: #fff;
  background-color: #398439;
  border-color: #255625;
}
.notification_widget.success:active,
.notification_widget.success.active,
.open > .dropdown-toggle.notification_widget.success {
  background-image: none;
}
.notification_widget.success.disabled:hover,
.notification_widget.success[disabled]:hover,
fieldset[disabled] .notification_widget.success:hover,
.notification_widget.success.disabled:focus,
.notification_widget.success[disabled]:focus,
fieldset[disabled] .notification_widget.success:focus,
.notification_widget.success.disabled.focus,
.notification_widget.success[disabled].focus,
fieldset[disabled] .notification_widget.success.focus {
  background-color: #5cb85c;
  border-color: #4cae4c;
}
.notification_widget.success .badge {
  color: #5cb85c;
  background-color: #fff;
}
.notification_widget.info {
  color: #fff;
  background-color: #5bc0de;
  border-color: #46b8da;
}
.notification_widget.info:focus,
.notification_widget.info.focus {
  color: #fff;
  background-color: #31b0d5;
  border-color: #1b6d85;
}
.notification_widget.info:hover {
  color: #fff;
  background-color: #31b0d5;
  border-color: #269abc;
}
.notification_widget.info:active,
.notification_widget.info.active,
.open > .dropdown-toggle.notification_widget.info {
  color: #fff;
  background-color: #31b0d5;
  border-color: #269abc;
}
.notification_widget.info:active:hover,
.notification_widget.info.active:hover,
.open > .dropdown-toggle.notification_widget.info:hover,
.notification_widget.info:active:focus,
.notification_widget.info.active:focus,
.open > .dropdown-toggle.notification_widget.info:focus,
.notification_widget.info:active.focus,
.notification_widget.info.active.focus,
.open > .dropdown-toggle.notification_widget.info.focus {
  color: #fff;
  background-color: #269abc;
  border-color: #1b6d85;
}
.notification_widget.info:active,
.notification_widget.info.active,
.open > .dropdown-toggle.notification_widget.info {
  background-image: none;
}
.notification_widget.info.disabled:hover,
.notification_widget.info[disabled]:hover,
fieldset[disabled] .notification_widget.info:hover,
.notification_widget.info.disabled:focus,
.notification_widget.info[disabled]:focus,
fieldset[disabled] .notification_widget.info:focus,
.notification_widget.info.disabled.focus,
.notification_widget.info[disabled].focus,
fieldset[disabled] .notification_widget.info.focus {
  background-color: #5bc0de;
  border-color: #46b8da;
}
.notification_widget.info .badge {
  color: #5bc0de;
  background-color: #fff;
}
.notification_widget.danger {
  color: #fff;
  background-color: #d9534f;
  border-color: #d43f3a;
}
.notification_widget.danger:focus,
.notification_widget.danger.focus {
  color: #fff;
  background-color: #c9302c;
  border-color: #761c19;
}
.notification_widget.danger:hover {
  color: #fff;
  background-color: #c9302c;
  border-color: #ac2925;
}
.notification_widget.danger:active,
.notification_widget.danger.active,
.open > .dropdown-toggle.notification_widget.danger {
  color: #fff;
  background-color: #c9302c;
  border-color: #ac2925;
}
.notification_widget.danger:active:hover,
.notification_widget.danger.active:hover,
.open > .dropdown-toggle.notification_widget.danger:hover,
.notification_widget.danger:active:focus,
.notification_widget.danger.active:focus,
.open > .dropdown-toggle.notification_widget.danger:focus,
.notification_widget.danger:active.focus,
.notification_widget.danger.active.focus,
.open > .dropdown-toggle.notification_widget.danger.focus {
  color: #fff;
  background-color: #ac2925;
  border-color: #761c19;
}
.notification_widget.danger:active,
.notification_widget.danger.active,
.open > .dropdown-toggle.notification_widget.danger {
  background-image: none;
}
.notification_widget.danger.disabled:hover,
.notification_widget.danger[disabled]:hover,
fieldset[disabled] .notification_widget.danger:hover,
.notification_widget.danger.disabled:focus,
.notification_widget.danger[disabled]:focus,
fieldset[disabled] .notification_widget.danger:focus,
.notification_widget.danger.disabled.focus,
.notification_widget.danger[disabled].focus,
fieldset[disabled] .notification_widget.danger.focus {
  background-color: #d9534f;
  border-color: #d43f3a;
}
.notification_widget.danger .badge {
  color: #d9534f;
  background-color: #fff;
}
div#pager {
  background-color: #fff;
  font-size: 14px;
  line-height: 20px;
  overflow: hidden;
  display: none;
  position: fixed;
  bottom: 0px;
  width: 100%;
  max-height: 50%;
  padding-top: 8px;
  -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  /* Display over codemirror */
  z-index: 100;
  /* Hack which prevents jquery ui resizable from changing top. */
  top: auto !important;
}
div#pager pre {
  line-height: 1.21429em;
  color: #000;
  background-color: #f7f7f7;
  padding: 0.4em;
}
div#pager #pager-button-area {
  position: absolute;
  top: 8px;
  right: 20px;
}
div#pager #pager-contents {
  position: relative;
  overflow: auto;
  width: 100%;
  height: 100%;
}
div#pager #pager-contents #pager-container {
  position: relative;
  padding: 15px 0px;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
}
div#pager .ui-resizable-handle {
  top: 0px;
  height: 8px;
  background: #f7f7f7;
  border-top: 1px solid #cfcfcf;
  border-bottom: 1px solid #cfcfcf;
  /* This injects handle bars (a short, wide = symbol) for 
        the resize handle. */
}
div#pager .ui-resizable-handle::after {
  content: '';
  top: 2px;
  left: 50%;
  height: 3px;
  width: 30px;
  margin-left: -15px;
  position: absolute;
  border-top: 1px solid #cfcfcf;
}
.quickhelp {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
  line-height: 1.8em;
}
.shortcut_key {
  display: inline-block;
  width: 21ex;
  text-align: right;
  font-family: monospace;
}
.shortcut_descr {
  display: inline-block;
  /* Old browsers */
  -webkit-box-flex: 1;
  -moz-box-flex: 1;
  box-flex: 1;
  /* Modern browsers */
  flex: 1;
}
span.save_widget {
  height: 30px;
  margin-top: 4px;
  display: flex;
  justify-content: flex-start;
  align-items: baseline;
  width: 50%;
  flex: 1;
}
span.save_widget span.filename {
  height: 100%;
  line-height: 1em;
  margin-left: 16px;
  border: none;
  font-size: 146.5%;
  text-overflow: ellipsis;
  overflow: hidden;
  white-space: nowrap;
  border-radius: 2px;
}
span.save_widget span.filename:hover {
  background-color: #e6e6e6;
}
[dir="rtl"] span.save_widget.pull-left {
  float: right !important;
  float: right;
}
[dir="rtl"] span.save_widget span.filename {
  margin-left: 0;
  margin-right: 16px;
}
span.checkpoint_status,
span.autosave_status {
  font-size: small;
  white-space: nowrap;
  padding: 0 5px;
}
@media (max-width: 767px) {
  span.save_widget {
    font-size: small;
    padding: 0 0 0 5px;
  }
  span.checkpoint_status,
  span.autosave_status {
    display: none;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  span.checkpoint_status {
    display: none;
  }
  span.autosave_status {
    font-size: x-small;
  }
}
.toolbar {
  padding: 0px;
  margin-left: -5px;
  margin-top: 2px;
  margin-bottom: 5px;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
}
.toolbar select,
.toolbar label {
  width: auto;
  vertical-align: middle;
  margin-right: 2px;
  margin-bottom: 0px;
  display: inline;
  font-size: 92%;
  margin-left: 0.3em;
  margin-right: 0.3em;
  padding: 0px;
  padding-top: 3px;
}
.toolbar .btn {
  padding: 2px 8px;
}
.toolbar .btn-group {
  margin-top: 0px;
  margin-left: 5px;
}
.toolbar-btn-label {
  margin-left: 6px;
}
#maintoolbar {
  margin-bottom: -3px;
  margin-top: -8px;
  border: 0px;
  min-height: 27px;
  margin-left: 0px;
  padding-top: 11px;
  padding-bottom: 3px;
}
#maintoolbar .navbar-text {
  float: none;
  vertical-align: middle;
  text-align: right;
  margin-left: 5px;
  margin-right: 0px;
  margin-top: 0px;
}
.select-xs {
  height: 24px;
}
[dir="rtl"] .btn-group > .btn,
.btn-group-vertical > .btn {
  float: right;
}
.pulse,
.dropdown-menu > li > a.pulse,
li.pulse > a.dropdown-toggle,
li.pulse.open > a.dropdown-toggle {
  background-color: #F37626;
  color: white;
}
/**
 * Primary styles
 *
 * Author: Jupyter Development Team
 */
/** WARNING IF YOU ARE EDITTING THIS FILE, if this is a .css file, It has a lot
 * of chance of beeing generated from the ../less/[samename].less file, you can
 * try to get back the less file by reverting somme commit in history
 **/
/*
 * We'll try to get something pretty, so we
 * have some strange css to have the scroll bar on
 * the left with fix button on the top right of the tooltip
 */
@-moz-keyframes fadeOut {
  from {
    opacity: 1;
  }
  to {
    opacity: 0;
  }
}
@-webkit-keyframes fadeOut {
  from {
    opacity: 1;
  }
  to {
    opacity: 0;
  }
}
@-moz-keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
@-webkit-keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
/*properties of tooltip after "expand"*/
.bigtooltip {
  overflow: auto;
  height: 200px;
  -webkit-transition-property: height;
  -webkit-transition-duration: 500ms;
  -moz-transition-property: height;
  -moz-transition-duration: 500ms;
  transition-property: height;
  transition-duration: 500ms;
}
/*properties of tooltip before "expand"*/
.smalltooltip {
  -webkit-transition-property: height;
  -webkit-transition-duration: 500ms;
  -moz-transition-property: height;
  -moz-transition-duration: 500ms;
  transition-property: height;
  transition-duration: 500ms;
  text-overflow: ellipsis;
  overflow: hidden;
  height: 80px;
}
.tooltipbuttons {
  position: absolute;
  padding-right: 15px;
  top: 0px;
  right: 0px;
}
.tooltiptext {
  /*avoid the button to overlap on some docstring*/
  padding-right: 30px;
}
.ipython_tooltip {
  max-width: 700px;
  /*fade-in animation when inserted*/
  -webkit-animation: fadeOut 400ms;
  -moz-animation: fadeOut 400ms;
  animation: fadeOut 400ms;
  -webkit-animation: fadeIn 400ms;
  -moz-animation: fadeIn 400ms;
  animation: fadeIn 400ms;
  vertical-align: middle;
  background-color: #f7f7f7;
  overflow: visible;
  border: #ababab 1px solid;
  outline: none;
  padding: 3px;
  margin: 0px;
  padding-left: 7px;
  font-family: monospace;
  min-height: 50px;
  -moz-box-shadow: 0px 6px 10px -1px #adadad;
  -webkit-box-shadow: 0px 6px 10px -1px #adadad;
  box-shadow: 0px 6px 10px -1px #adadad;
  border-radius: 2px;
  position: absolute;
  z-index: 1000;
}
.ipython_tooltip a {
  float: right;
}
.ipython_tooltip .tooltiptext pre {
  border: 0;
  border-radius: 0;
  font-size: 100%;
  background-color: #f7f7f7;
}
.pretooltiparrow {
  left: 0px;
  margin: 0px;
  top: -16px;
  width: 40px;
  height: 16px;
  overflow: hidden;
  position: absolute;
}
.pretooltiparrow:before {
  background-color: #f7f7f7;
  border: 1px #ababab solid;
  z-index: 11;
  content: "";
  position: absolute;
  left: 15px;
  top: 10px;
  width: 25px;
  height: 25px;
  -webkit-transform: rotate(45deg);
  -moz-transform: rotate(45deg);
  -ms-transform: rotate(45deg);
  -o-transform: rotate(45deg);
}
ul.typeahead-list i {
  margin-left: -10px;
  width: 18px;
}
[dir="rtl"] ul.typeahead-list i {
  margin-left: 0;
  margin-right: -10px;
}
ul.typeahead-list {
  max-height: 80vh;
  overflow: auto;
}
ul.typeahead-list > li > a {
  /** Firefox bug **/
  /* see https://github.com/jupyter/notebook/issues/559 */
  white-space: normal;
}
ul.typeahead-list  > li > a.pull-right {
  float: left !important;
  float: left;
}
[dir="rtl"] .typeahead-list {
  text-align: right;
}
.cmd-palette .modal-body {
  padding: 7px;
}
.cmd-palette form {
  background: white;
}
.cmd-palette input {
  outline: none;
}
.no-shortcut {
  min-width: 20px;
  color: transparent;
}
[dir="rtl"] .no-shortcut.pull-right {
  float: left !important;
  float: left;
}
[dir="rtl"] .command-shortcut.pull-right {
  float: left !important;
  float: left;
}
.command-shortcut:before {
  content: "(command mode)";
  padding-right: 3px;
  color: #777777;
}
.edit-shortcut:before {
  content: "(edit)";
  padding-right: 3px;
  color: #777777;
}
[dir="rtl"] .edit-shortcut.pull-right {
  float: left !important;
  float: left;
}
#find-and-replace #replace-preview .match,
#find-and-replace #replace-preview .insert {
  background-color: #BBDEFB;
  border-color: #90CAF9;
  border-style: solid;
  border-width: 1px;
  border-radius: 0px;
}
[dir="ltr"] #find-and-replace .input-group-btn + .form-control {
  border-left: none;
}
[dir="rtl"] #find-and-replace .input-group-btn + .form-control {
  border-right: none;
}
#find-and-replace #replace-preview .replace .match {
  background-color: #FFCDD2;
  border-color: #EF9A9A;
  border-radius: 0px;
}
#find-and-replace #replace-preview .replace .insert {
  background-color: #C8E6C9;
  border-color: #A5D6A7;
  border-radius: 0px;
}
#find-and-replace #replace-preview {
  max-height: 60vh;
  overflow: auto;
}
#find-and-replace #replace-preview pre {
  padding: 5px 10px;
}
.terminal-app {
  background: #EEE;
}
.terminal-app #header {
  background: #fff;
  -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
}
.terminal-app .terminal {
  width: 100%;
  float: left;
  font-family: monospace;
  color: white;
  background: black;
  padding: 0.4em;
  border-radius: 2px;
  -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.4);
  box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.4);
}
.terminal-app .terminal,
.terminal-app .terminal dummy-screen {
  line-height: 1em;
  font-size: 14px;
}
.terminal-app .terminal .xterm-rows {
  padding: 10px;
}
.terminal-app .terminal-cursor {
  color: black;
  background: white;
}
.terminal-app #terminado-container {
  margin-top: 20px;
}
/*# sourceMappingURL=style.min.css.map */
    </style>
<style type="text/css">
    .highlight .hll { background-color: #ffffcc }
.highlight  { background: #f8f8f8; }
.highlight .c { color: #408080; font-style: italic } /* Comment */
.highlight .err { border: 1px solid #FF0000 } /* Error */
.highlight .k { color: #008000; font-weight: bold } /* Keyword */
.highlight .o { color: #666666 } /* Operator */
.highlight .ch { color: #408080; font-style: italic } /* Comment.Hashbang */
.highlight .cm { color: #408080; font-style: italic } /* Comment.Multiline */
.highlight .cp { color: #BC7A00 } /* Comment.Preproc */
.highlight .cpf { color: #408080; font-style: italic } /* Comment.PreprocFile */
.highlight .c1 { color: #408080; font-style: italic } /* Comment.Single */
.highlight .cs { color: #408080; font-style: italic } /* Comment.Special */
.highlight .gd { color: #A00000 } /* Generic.Deleted */
.highlight .ge { font-style: italic } /* Generic.Emph */
.highlight .gr { color: #FF0000 } /* Generic.Error */
.highlight .gh { color: #000080; font-weight: bold } /* Generic.Heading */
.highlight .gi { color: #00A000 } /* Generic.Inserted */
.highlight .go { color: #888888 } /* Generic.Output */
.highlight .gp { color: #000080; font-weight: bold } /* Generic.Prompt */
.highlight .gs { font-weight: bold } /* Generic.Strong */
.highlight .gu { color: #800080; font-weight: bold } /* Generic.Subheading */
.highlight .gt { color: #0044DD } /* Generic.Traceback */
.highlight .kc { color: #008000; font-weight: bold } /* Keyword.Constant */
.highlight .kd { color: #008000; font-weight: bold } /* Keyword.Declaration */
.highlight .kn { color: #008000; font-weight: bold } /* Keyword.Namespace */
.highlight .kp { color: #008000 } /* Keyword.Pseudo */
.highlight .kr { color: #008000; font-weight: bold } /* Keyword.Reserved */
.highlight .kt { color: #B00040 } /* Keyword.Type */
.highlight .m { color: #666666 } /* Literal.Number */
.highlight .s { color: #BA2121 } /* Literal.String */
.highlight .na { color: #7D9029 } /* Name.Attribute */
.highlight .nb { color: #008000 } /* Name.Builtin */
.highlight .nc { color: #0000FF; font-weight: bold } /* Name.Class */
.highlight .no { color: #880000 } /* Name.Constant */
.highlight .nd { color: #AA22FF } /* Name.Decorator */
.highlight .ni { color: #999999; font-weight: bold } /* Name.Entity */
.highlight .ne { color: #D2413A; font-weight: bold } /* Name.Exception */
.highlight .nf { color: #0000FF } /* Name.Function */
.highlight .nl { color: #A0A000 } /* Name.Label */
.highlight .nn { color: #0000FF; font-weight: bold } /* Name.Namespace */
.highlight .nt { color: #008000; font-weight: bold } /* Name.Tag */
.highlight .nv { color: #19177C } /* Name.Variable */
.highlight .ow { color: #AA22FF; font-weight: bold } /* Operator.Word */
.highlight .w { color: #bbbbbb } /* Text.Whitespace */
.highlight .mb { color: #666666 } /* Literal.Number.Bin */
.highlight .mf { color: #666666 } /* Literal.Number.Float */
.highlight .mh { color: #666666 } /* Literal.Number.Hex */
.highlight .mi { color: #666666 } /* Literal.Number.Integer */
.highlight .mo { color: #666666 } /* Literal.Number.Oct */
.highlight .sa { color: #BA2121 } /* Literal.String.Affix */
.highlight .sb { color: #BA2121 } /* Literal.String.Backtick */
.highlight .sc { color: #BA2121 } /* Literal.String.Char */
.highlight .dl { color: #BA2121 } /* Literal.String.Delimiter */
.highlight .sd { color: #BA2121; font-style: italic } /* Literal.String.Doc */
.highlight .s2 { color: #BA2121 } /* Literal.String.Double */
.highlight .se { color: #BB6622; font-weight: bold } /* Literal.String.Escape */
.highlight .sh { color: #BA2121 } /* Literal.String.Heredoc */
.highlight .si { color: #BB6688; font-weight: bold } /* Literal.String.Interpol */
.highlight .sx { color: #008000 } /* Literal.String.Other */
.highlight .sr { color: #BB6688 } /* Literal.String.Regex */
.highlight .s1 { color: #BA2121 } /* Literal.String.Single */
.highlight .ss { color: #19177C } /* Literal.String.Symbol */
.highlight .bp { color: #008000 } /* Name.Builtin.Pseudo */
.highlight .fm { color: #0000FF } /* Name.Function.Magic */
.highlight .vc { color: #19177C } /* Name.Variable.Class */
.highlight .vg { color: #19177C } /* Name.Variable.Global */
.highlight .vi { color: #19177C } /* Name.Variable.Instance */
.highlight .vm { color: #19177C } /* Name.Variable.Magic */
.highlight .il { color: #666666 } /* Literal.Number.Integer.Long */
    </style>


<style type="text/css">
/* Overrides of notebook CSS for static HTML export */
body {
  overflow: visible;
  padding: 8px;
}

div#notebook {
  overflow: visible;
  border-top: none;
}@media print {
  div.cell {
    display: block;
    page-break-inside: avoid;
  } 
  div.output_wrapper { 
    display: block;
    page-break-inside: avoid; 
  }
  div.output { 
    display: block;
    page-break-inside: avoid; 
  }
}
</style>

<!-- Custom stylesheet, it must be in the same directory as the html file -->
<link rel="stylesheet" href="custom.css">

<!-- Loading mathjax macro -->
<!-- Load mathjax -->
    <script src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.5/latest.js?config=TeX-AMS_HTML"></script>
    <!-- MathJax configuration -->
    <script type="text/x-mathjax-config">
    MathJax.Hub.Config({
        tex2jax: {
            inlineMath: [ ['$','$'], ["\\(","\\)"] ],
            displayMath: [ ['$$','$$'], ["\\[","\\]"] ],
            processEscapes: true,
            processEnvironments: true
        },
        // Center justify equations in code and markdown cells. Elsewhere
        // we use CSS to left justify single line equations in code cells.
        displayAlign: 'center',
        "HTML-CSS": {
            styles: {'.MathJax_Display': {"margin": 0}},
            linebreaks: { automatic: true }
        }
    });
    </script>
    <!-- End of mathjax configuration --></head>
<body>
  <div tabindex="-1" id="notebook" class="border-box-sizing">
    <div class="container" id="notebook-container">

<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[74]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="kn">import</span> <span class="nn">matplotlib.pyplot</span> <span class="k">as</span> <span class="nn">plt</span>
<span class="kn">import</span> <span class="nn">pandas</span> <span class="k">as</span> <span class="nn">pd</span>
<span class="kn">import</span> <span class="nn">statsmodels.tsa.seasonal</span> <span class="k">as</span> <span class="nn">seasonal</span>
<span class="kn">import</span> <span class="nn">statsmodels.tsa.holtwinters</span> <span class="k">as</span> <span class="nn">hw</span>
<span class="kn">import</span> <span class="nn">locale</span>
<span class="kn">import</span> <span class="nn">matplotlib.patches</span> <span class="k">as</span> <span class="nn">mpatches</span>
<span class="kn">import</span> <span class="nn">requests</span>
<span class="kn">import</span> <span class="nn">io</span>
<span class="kn">import</span> <span class="nn">datetime</span> <span class="k">as</span> <span class="nn">dt</span>
<span class="kn">import</span> <span class="nn">numpy</span> <span class="k">as</span> <span class="nn">np</span>
</pre></div>

    </div>
</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[75]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="k">def</span> <span class="nf">char_range</span><span class="p">(</span><span class="n">c1</span><span class="p">,</span> <span class="n">n</span><span class="p">):</span>
    <span class="sd">&quot;&quot;&quot;Generates the characters from `c1` to `c2`, inclusive.&quot;&quot;&quot;</span>
    <span class="k">for</span> <span class="n">c</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="nb">ord</span><span class="p">(</span><span class="n">c1</span><span class="p">),</span> <span class="nb">ord</span><span class="p">(</span><span class="n">c1</span><span class="p">)</span><span class="o">+</span><span class="n">n</span><span class="p">):</span>
        <span class="k">yield</span> <span class="nb">chr</span><span class="p">(</span><span class="n">c</span><span class="p">)</span>
<span class="nb">list</span><span class="p">(</span><span class="n">char_range</span><span class="p">(</span><span class="s1">&#39;a&#39;</span><span class="p">,</span><span class="mi">5</span><span class="p">))</span>
<span class="n">locale</span><span class="o">.</span><span class="n">setlocale</span><span class="p">(</span><span class="n">locale</span><span class="o">.</span><span class="n">LC_ALL</span><span class="p">,</span> <span class="s1">&#39;de_DE&#39;</span><span class="p">)</span>
<span class="n">today</span> <span class="o">=</span> <span class="n">dt</span><span class="o">.</span><span class="n">datetime</span><span class="o">.</span><span class="n">today</span><span class="p">()</span><span class="o">.</span><span class="n">strftime</span><span class="p">(</span><span class="s2">&quot;</span><span class="si">%-d</span><span class="s2">. %B 2020&quot;</span><span class="p">)</span>
<span class="n">today</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[75]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>&#39;2. August 2020&#39;</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[76]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">r</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="sa">r</span><span class="s1">&#39;https://www.rki.de/DE/Content/InfAZ/N/Neuartiges_Coronavirus/Projekte_RKI/Nowcasting_Zahlen.xlsx?__blob=publicationFile&#39;</span><span class="p">)</span>
<span class="n">test</span> <span class="o">=</span> <span class="n">pd</span><span class="o">.</span><span class="n">read_excel</span><span class="p">(</span><span class="n">io</span><span class="o">.</span><span class="n">BytesIO</span><span class="p">(</span><span class="n">r</span><span class="o">.</span><span class="n">content</span><span class="p">),</span><span class="mi">1</span><span class="p">,</span><span class="n">columns</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="s1">&#39;abcdefghijk&#39;</span><span class="p">))</span>
</pre></div>

    </div>
</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[77]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">nowcast</span> <span class="o">=</span> <span class="n">test</span> <span class="c1">#pd.read_excel(&#39;nowcast.xlsx&#39;,1,columns = list(&#39;abcdefghijk&#39;))</span>
<span class="n">nowcast</span><span class="o">.</span><span class="n">columns</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">char_range</span><span class="p">(</span><span class="s1">&#39;a&#39;</span><span class="p">,</span><span class="nb">len</span><span class="p">(</span><span class="n">nowcast</span><span class="o">.</span><span class="n">columns</span><span class="p">)))</span>
<span class="n">nowcast</span><span class="o">.</span><span class="n">index</span> <span class="o">=</span> <span class="n">nowcast</span><span class="o">.</span><span class="n">a</span>
<span class="n">pd</span><span class="o">.</span><span class="n">set_option</span><span class="p">(</span><span class="s2">&quot;display.max_rows&quot;</span><span class="p">,</span> <span class="mi">20</span><span class="p">,</span> <span class="s2">&quot;display.max_columns&quot;</span><span class="p">,</span> <span class="kc">None</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Last update:&quot;</span><span class="p">,</span><span class="n">nowcast</span><span class="o">.</span><span class="n">index</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span><span class="o">+</span><span class="n">dt</span><span class="o">.</span><span class="n">timedelta</span><span class="p">(</span><span class="mi">4</span><span class="p">))</span>
<span class="n">today</span> <span class="o">=</span> <span class="p">(</span><span class="n">nowcast</span><span class="o">.</span><span class="n">index</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span><span class="o">+</span><span class="n">dt</span><span class="o">.</span><span class="n">timedelta</span><span class="p">(</span><span class="mi">4</span><span class="p">))</span><span class="o">.</span><span class="n">strftime</span><span class="p">(</span><span class="s2">&quot;</span><span class="si">%-d</span><span class="s2">. %B 2020&quot;</span><span class="p">)</span>
<span class="n">nowcast</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt"></div>


<div class="output_subarea output_stream output_stdout output_text">
<pre>Last update: 2020-08-01 00:00:00
</pre>
</div>
</div>

<div class="output_area">

    <div class="prompt output_prompt">Out[77]:</div>



<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>a</th>
      <th>b</th>
      <th>c</th>
      <th>d</th>
      <th>e</th>
      <th>f</th>
      <th>g</th>
      <th>h</th>
      <th>i</th>
      <th>j</th>
      <th>k</th>
      <th>l</th>
      <th>m</th>
    </tr>
    <tr>
      <th>a</th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>2020-03-02</td>
      <td>2020-03-02</td>
      <td>303</td>
      <td>288</td>
      <td>320</td>
      <td>225</td>
      <td>212</td>
      <td>238</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <td>2020-03-03</td>
      <td>2020-03-03</td>
      <td>320</td>
      <td>305</td>
      <td>336</td>
      <td>260</td>
      <td>246</td>
      <td>275</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <td>2020-03-04</td>
      <td>2020-03-04</td>
      <td>448</td>
      <td>430</td>
      <td>465</td>
      <td>325</td>
      <td>309</td>
      <td>341</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <td>2020-03-05</td>
      <td>2020-03-05</td>
      <td>505</td>
      <td>483</td>
      <td>524</td>
      <td>394</td>
      <td>376</td>
      <td>411</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <td>2020-03-06</td>
      <td>2020-03-06</td>
      <td>758</td>
      <td>736</td>
      <td>787</td>
      <td>508</td>
      <td>488</td>
      <td>528</td>
      <td>2.26</td>
      <td>2.18</td>
      <td>2.34</td>
      <td>2.34</td>
      <td>2.30</td>
      <td>2.40</td>
    </tr>
    <tr>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <td>2020-07-24</td>
      <td>2020-07-24</td>
      <td>711</td>
      <td>554</td>
      <td>855</td>
      <td>706</td>
      <td>594</td>
      <td>821</td>
      <td>1.32</td>
      <td>1.18</td>
      <td>1.44</td>
      <td>1.19</td>
      <td>1.12</td>
      <td>1.27</td>
    </tr>
    <tr>
      <td>2020-07-25</td>
      <td>2020-07-25</td>
      <td>630</td>
      <td>445</td>
      <td>794</td>
      <td>688</td>
      <td>551</td>
      <td>819</td>
      <td>1.19</td>
      <td>1.04</td>
      <td>1.32</td>
      <td>1.18</td>
      <td>1.09</td>
      <td>1.27</td>
    </tr>
    <tr>
      <td>2020-07-26</td>
      <td>2020-07-26</td>
      <td>699</td>
      <td>524</td>
      <td>893</td>
      <td>679</td>
      <td>524</td>
      <td>833</td>
      <td>1.05</td>
      <td>0.90</td>
      <td>1.21</td>
      <td>1.21</td>
      <td>1.09</td>
      <td>1.32</td>
    </tr>
    <tr>
      <td>2020-07-27</td>
      <td>2020-07-27</td>
      <td>1001</td>
      <td>630</td>
      <td>1393</td>
      <td>760</td>
      <td>538</td>
      <td>984</td>
      <td>1.11</td>
      <td>0.92</td>
      <td>1.29</td>
      <td>1.20</td>
      <td>1.07</td>
      <td>1.34</td>
    </tr>
    <tr>
      <td>2020-07-28</td>
      <td>2020-07-28</td>
      <td>858</td>
      <td>459</td>
      <td>1240</td>
      <td>797</td>
      <td>515</td>
      <td>1080</td>
      <td>1.13</td>
      <td>0.93</td>
      <td>1.41</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
  </tbody>
</table>
<p>149 rows × 13 columns</p>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[78]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># #Seasonal decomposition of Nowcast values not smoothed</span>
<span class="c1"># import statsmodels.tsa.seasonal as seasonal</span>
<span class="c1"># result_b = seasonal.seasonal_decompose(nowcast.b,model=&quot;multiplicative&quot;)</span>
<span class="c1"># plot = result_b.plot()</span>
</pre></div>

    </div>
</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[79]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1">#Seasonal decomposition of Nowcast values not smoothed</span>
<span class="kn">import</span> <span class="nn">statsmodels.tsa.seasonal</span> <span class="k">as</span> <span class="nn">seasonal</span>
<span class="n">nowcast</span><span class="o">.</span><span class="n">b</span><span class="p">[</span><span class="n">nowcast</span><span class="o">.</span><span class="n">index</span> <span class="o">==</span> <span class="n">dt</span><span class="o">.</span><span class="n">datetime</span><span class="p">(</span><span class="mi">2020</span><span class="p">,</span><span class="mi">6</span><span class="p">,</span><span class="mi">15</span><span class="p">)]</span> <span class="o">=</span> <span class="mi">500</span>
<span class="n">nowcast</span><span class="o">.</span><span class="n">b</span><span class="p">[</span><span class="n">nowcast</span><span class="o">.</span><span class="n">index</span> <span class="o">==</span> <span class="n">dt</span><span class="o">.</span><span class="n">datetime</span><span class="p">(</span><span class="mi">2020</span><span class="p">,</span><span class="mi">6</span><span class="p">,</span><span class="mi">16</span><span class="p">)]</span> <span class="o">=</span> <span class="mi">500</span>
<span class="n">nowcast</span><span class="o">.</span><span class="n">b</span><span class="p">[</span><span class="n">nowcast</span><span class="o">.</span><span class="n">index</span> <span class="o">==</span> <span class="n">dt</span><span class="o">.</span><span class="n">datetime</span><span class="p">(</span><span class="mi">2020</span><span class="p">,</span><span class="mi">6</span><span class="p">,</span><span class="mi">17</span><span class="p">)]</span> <span class="o">=</span> <span class="mi">500</span>
<span class="n">result_b</span> <span class="o">=</span> <span class="n">seasonal</span><span class="o">.</span><span class="n">seasonal_decompose</span><span class="p">(</span><span class="n">nowcast</span><span class="o">.</span><span class="n">b</span><span class="p">,</span><span class="n">model</span><span class="o">=</span><span class="s2">&quot;multiplicative&quot;</span><span class="p">)</span>
<span class="n">result_b</span><span class="o">.</span><span class="n">observed</span><span class="p">[</span><span class="n">result_b</span><span class="o">.</span><span class="n">observed</span><span class="o">.</span><span class="n">index</span> <span class="o">==</span> <span class="n">dt</span><span class="o">.</span><span class="n">datetime</span><span class="p">(</span><span class="mi">2020</span><span class="p">,</span><span class="mi">6</span><span class="p">,</span><span class="mi">15</span><span class="p">)]</span> <span class="o">=</span> <span class="mi">645</span>
<span class="n">result_b</span><span class="o">.</span><span class="n">observed</span><span class="p">[</span><span class="n">result_b</span><span class="o">.</span><span class="n">observed</span><span class="o">.</span><span class="n">index</span> <span class="o">==</span> <span class="n">dt</span><span class="o">.</span><span class="n">datetime</span><span class="p">(</span><span class="mi">2020</span><span class="p">,</span><span class="mi">6</span><span class="p">,</span><span class="mi">16</span><span class="p">)]</span> <span class="o">=</span> <span class="mi">1123</span>
<span class="n">result_b</span><span class="o">.</span><span class="n">observed</span><span class="p">[</span><span class="n">result_b</span><span class="o">.</span><span class="n">observed</span><span class="o">.</span><span class="n">index</span> <span class="o">==</span> <span class="n">dt</span><span class="o">.</span><span class="n">datetime</span><span class="p">(</span><span class="mi">2020</span><span class="p">,</span><span class="mi">6</span><span class="p">,</span><span class="mi">17</span><span class="p">)]</span> <span class="o">=</span> <span class="mi">669</span>
<span class="n">nowcast</span><span class="o">.</span><span class="n">b</span><span class="p">[</span><span class="n">nowcast</span><span class="o">.</span><span class="n">index</span> <span class="o">==</span> <span class="n">dt</span><span class="o">.</span><span class="n">datetime</span><span class="p">(</span><span class="mi">2020</span><span class="p">,</span><span class="mi">6</span><span class="p">,</span><span class="mi">15</span><span class="p">)]</span> <span class="o">=</span> <span class="mi">645</span>
<span class="n">nowcast</span><span class="o">.</span><span class="n">b</span><span class="p">[</span><span class="n">nowcast</span><span class="o">.</span><span class="n">index</span> <span class="o">==</span> <span class="n">dt</span><span class="o">.</span><span class="n">datetime</span><span class="p">(</span><span class="mi">2020</span><span class="p">,</span><span class="mi">6</span><span class="p">,</span><span class="mi">16</span><span class="p">)]</span> <span class="o">=</span> <span class="mi">1123</span>
<span class="n">nowcast</span><span class="o">.</span><span class="n">b</span><span class="p">[</span><span class="n">nowcast</span><span class="o">.</span><span class="n">index</span> <span class="o">==</span> <span class="n">dt</span><span class="o">.</span><span class="n">datetime</span><span class="p">(</span><span class="mi">2020</span><span class="p">,</span><span class="mi">6</span><span class="p">,</span><span class="mi">17</span><span class="p">)]</span> <span class="o">=</span> <span class="mi">669</span>
<span class="n">plot</span> <span class="o">=</span> <span class="n">result_b</span><span class="o">.</span><span class="n">plot</span><span class="p">()</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt"></div>



<div class="output_svg output_subarea ">
<?xml version="1.0" encoding="utf-8" standalone="no"?>
<!DOCTYPE svg PUBLIC "-//W3C//DTD SVG 1.1//EN"
  "http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd">
<!-- Created with matplotlib (https://matplotlib.org/) -->
<svg height="279.59625pt" version="1.1" viewBox="0 0 424.231459 279.59625" width="424.231459pt" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
 <defs>
  <style type="text/css">
*{stroke-linecap:butt;stroke-linejoin:round;}
  </style>
 </defs>
 <g id="figure_1">
  <g id="patch_1">
   <path d="M 0 279.59625 
L 424.231459 279.59625 
L 424.231459 0 
L 0 0 
z
" style="fill:none;"/>
  </g>
  <g id="axes_1">
   <g id="patch_2">
    <path d="M 53.328125 59.005985 
L 402.113598 59.005985 
L 402.113598 22.318125 
L 53.328125 22.318125 
z
" style="fill:#ffffff;"/>
   </g>
   <g id="matplotlib.axis_1">
    <g id="xtick_1">
     <g id="line2d_1">
      <defs>
       <path d="M 0 0 
L 0 3.5 
" id="m4ab79eac75" style="stroke:#000000;stroke-width:0.8;"/>
      </defs>
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="100.461297" xlink:href="#m4ab79eac75" y="59.005985"/>
      </g>
     </g>
     <g id="text_1">
      <!-- 2020-03-22 -->
      <defs>
       <path d="M 19.1875 8.296875 
L 53.609375 8.296875 
L 53.609375 0 
L 7.328125 0 
L 7.328125 8.296875 
Q 12.9375 14.109375 22.625 23.890625 
Q 32.328125 33.6875 34.8125 36.53125 
Q 39.546875 41.84375 41.421875 45.53125 
Q 43.3125 49.21875 43.3125 52.78125 
Q 43.3125 58.59375 39.234375 62.25 
Q 35.15625 65.921875 28.609375 65.921875 
Q 23.96875 65.921875 18.8125 64.3125 
Q 13.671875 62.703125 7.8125 59.421875 
L 7.8125 69.390625 
Q 13.765625 71.78125 18.9375 73 
Q 24.125 74.21875 28.421875 74.21875 
Q 39.75 74.21875 46.484375 68.546875 
Q 53.21875 62.890625 53.21875 53.421875 
Q 53.21875 48.921875 51.53125 44.890625 
Q 49.859375 40.875 45.40625 35.40625 
Q 44.1875 33.984375 37.640625 27.21875 
Q 31.109375 20.453125 19.1875 8.296875 
z
" id="DejaVuSans-50"/>
       <path d="M 31.78125 66.40625 
Q 24.171875 66.40625 20.328125 58.90625 
Q 16.5 51.421875 16.5 36.375 
Q 16.5 21.390625 20.328125 13.890625 
Q 24.171875 6.390625 31.78125 6.390625 
Q 39.453125 6.390625 43.28125 13.890625 
Q 47.125 21.390625 47.125 36.375 
Q 47.125 51.421875 43.28125 58.90625 
Q 39.453125 66.40625 31.78125 66.40625 
z
M 31.78125 74.21875 
Q 44.046875 74.21875 50.515625 64.515625 
Q 56.984375 54.828125 56.984375 36.375 
Q 56.984375 17.96875 50.515625 8.265625 
Q 44.046875 -1.421875 31.78125 -1.421875 
Q 19.53125 -1.421875 13.0625 8.265625 
Q 6.59375 17.96875 6.59375 36.375 
Q 6.59375 54.828125 13.0625 64.515625 
Q 19.53125 74.21875 31.78125 74.21875 
z
" id="DejaVuSans-48"/>
       <path d="M 4.890625 31.390625 
L 31.203125 31.390625 
L 31.203125 23.390625 
L 4.890625 23.390625 
z
" id="DejaVuSans-45"/>
       <path d="M 40.578125 39.3125 
Q 47.65625 37.796875 51.625 33 
Q 55.609375 28.21875 55.609375 21.1875 
Q 55.609375 10.40625 48.1875 4.484375 
Q 40.765625 -1.421875 27.09375 -1.421875 
Q 22.515625 -1.421875 17.65625 -0.515625 
Q 12.796875 0.390625 7.625 2.203125 
L 7.625 11.71875 
Q 11.71875 9.328125 16.59375 8.109375 
Q 21.484375 6.890625 26.8125 6.890625 
Q 36.078125 6.890625 40.9375 10.546875 
Q 45.796875 14.203125 45.796875 21.1875 
Q 45.796875 27.640625 41.28125 31.265625 
Q 36.765625 34.90625 28.71875 34.90625 
L 20.21875 34.90625 
L 20.21875 43.015625 
L 29.109375 43.015625 
Q 36.375 43.015625 40.234375 45.921875 
Q 44.09375 48.828125 44.09375 54.296875 
Q 44.09375 59.90625 40.109375 62.90625 
Q 36.140625 65.921875 28.71875 65.921875 
Q 24.65625 65.921875 20.015625 65.03125 
Q 15.375 64.15625 9.8125 62.3125 
L 9.8125 71.09375 
Q 15.4375 72.65625 20.34375 73.4375 
Q 25.25 74.21875 29.59375 74.21875 
Q 40.828125 74.21875 47.359375 69.109375 
Q 53.90625 64.015625 53.90625 55.328125 
Q 53.90625 49.265625 50.4375 45.09375 
Q 46.96875 40.921875 40.578125 39.3125 
z
" id="DejaVuSans-51"/>
      </defs>
      <g transform="translate(71.403485 73.604422)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-51"/>
       <use x="417.822266" xlink:href="#DejaVuSans-45"/>
       <use x="453.90625" xlink:href="#DejaVuSans-50"/>
       <use x="517.529297" xlink:href="#DejaVuSans-50"/>
      </g>
     </g>
    </g>
    <g id="xtick_2">
     <g id="line2d_2">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="124.027883" xlink:href="#m4ab79eac75" y="59.005985"/>
      </g>
     </g>
     <g id="text_2">
      <!-- 2020-04-01 -->
      <defs>
       <path d="M 37.796875 64.3125 
L 12.890625 25.390625 
L 37.796875 25.390625 
z
M 35.203125 72.90625 
L 47.609375 72.90625 
L 47.609375 25.390625 
L 58.015625 25.390625 
L 58.015625 17.1875 
L 47.609375 17.1875 
L 47.609375 0 
L 37.796875 0 
L 37.796875 17.1875 
L 4.890625 17.1875 
L 4.890625 26.703125 
z
" id="DejaVuSans-52"/>
       <path d="M 12.40625 8.296875 
L 28.515625 8.296875 
L 28.515625 63.921875 
L 10.984375 60.40625 
L 10.984375 69.390625 
L 28.421875 72.90625 
L 38.28125 72.90625 
L 38.28125 8.296875 
L 54.390625 8.296875 
L 54.390625 0 
L 12.40625 0 
z
" id="DejaVuSans-49"/>
      </defs>
      <g transform="translate(94.970071 73.604422)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-52"/>
       <use x="417.822266" xlink:href="#DejaVuSans-45"/>
       <use x="453.90625" xlink:href="#DejaVuSans-48"/>
       <use x="517.529297" xlink:href="#DejaVuSans-49"/>
      </g>
     </g>
    </g>
    <g id="xtick_3">
     <g id="line2d_3">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="173.517714" xlink:href="#m4ab79eac75" y="59.005985"/>
      </g>
     </g>
     <g id="text_3">
      <!-- 2020-04-22 -->
      <g transform="translate(144.459901 73.604422)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-52"/>
       <use x="417.822266" xlink:href="#DejaVuSans-45"/>
       <use x="453.90625" xlink:href="#DejaVuSans-50"/>
       <use x="517.529297" xlink:href="#DejaVuSans-50"/>
      </g>
     </g>
    </g>
    <g id="xtick_4">
     <g id="line2d_4">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="194.727641" xlink:href="#m4ab79eac75" y="59.005985"/>
      </g>
     </g>
     <g id="text_4">
      <!-- 2020-05-01 -->
      <defs>
       <path d="M 10.796875 72.90625 
L 49.515625 72.90625 
L 49.515625 64.59375 
L 19.828125 64.59375 
L 19.828125 46.734375 
Q 21.96875 47.46875 24.109375 47.828125 
Q 26.265625 48.1875 28.421875 48.1875 
Q 40.625 48.1875 47.75 41.5 
Q 54.890625 34.8125 54.890625 23.390625 
Q 54.890625 11.625 47.5625 5.09375 
Q 40.234375 -1.421875 26.90625 -1.421875 
Q 22.3125 -1.421875 17.546875 -0.640625 
Q 12.796875 0.140625 7.71875 1.703125 
L 7.71875 11.625 
Q 12.109375 9.234375 16.796875 8.0625 
Q 21.484375 6.890625 26.703125 6.890625 
Q 35.15625 6.890625 40.078125 11.328125 
Q 45.015625 15.765625 45.015625 23.390625 
Q 45.015625 31 40.078125 35.4375 
Q 35.15625 39.890625 26.703125 39.890625 
Q 22.75 39.890625 18.8125 39.015625 
Q 14.890625 38.140625 10.796875 36.28125 
z
" id="DejaVuSans-53"/>
      </defs>
      <g transform="translate(165.669829 73.604422)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-53"/>
       <use x="417.822266" xlink:href="#DejaVuSans-45"/>
       <use x="453.90625" xlink:href="#DejaVuSans-48"/>
       <use x="517.529297" xlink:href="#DejaVuSans-49"/>
      </g>
     </g>
    </g>
    <g id="xtick_5">
     <g id="line2d_5">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="244.217472" xlink:href="#m4ab79eac75" y="59.005985"/>
      </g>
     </g>
     <g id="text_5">
      <!-- 2020-05-22 -->
      <g transform="translate(215.159659 73.604422)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-53"/>
       <use x="417.822266" xlink:href="#DejaVuSans-45"/>
       <use x="453.90625" xlink:href="#DejaVuSans-50"/>
       <use x="517.529297" xlink:href="#DejaVuSans-50"/>
      </g>
     </g>
    </g>
    <g id="xtick_6">
     <g id="line2d_6">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="267.784058" xlink:href="#m4ab79eac75" y="59.005985"/>
      </g>
     </g>
     <g id="text_6">
      <!-- 2020-06-01 -->
      <defs>
       <path d="M 33.015625 40.375 
Q 26.375 40.375 22.484375 35.828125 
Q 18.609375 31.296875 18.609375 23.390625 
Q 18.609375 15.53125 22.484375 10.953125 
Q 26.375 6.390625 33.015625 6.390625 
Q 39.65625 6.390625 43.53125 10.953125 
Q 47.40625 15.53125 47.40625 23.390625 
Q 47.40625 31.296875 43.53125 35.828125 
Q 39.65625 40.375 33.015625 40.375 
z
M 52.59375 71.296875 
L 52.59375 62.3125 
Q 48.875 64.0625 45.09375 64.984375 
Q 41.3125 65.921875 37.59375 65.921875 
Q 27.828125 65.921875 22.671875 59.328125 
Q 17.53125 52.734375 16.796875 39.40625 
Q 19.671875 43.65625 24.015625 45.921875 
Q 28.375 48.1875 33.59375 48.1875 
Q 44.578125 48.1875 50.953125 41.515625 
Q 57.328125 34.859375 57.328125 23.390625 
Q 57.328125 12.15625 50.6875 5.359375 
Q 44.046875 -1.421875 33.015625 -1.421875 
Q 20.359375 -1.421875 13.671875 8.265625 
Q 6.984375 17.96875 6.984375 36.375 
Q 6.984375 53.65625 15.1875 63.9375 
Q 23.390625 74.21875 37.203125 74.21875 
Q 40.921875 74.21875 44.703125 73.484375 
Q 48.484375 72.75 52.59375 71.296875 
z
" id="DejaVuSans-54"/>
      </defs>
      <g transform="translate(238.726245 73.604422)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-54"/>
       <use x="417.822266" xlink:href="#DejaVuSans-45"/>
       <use x="453.90625" xlink:href="#DejaVuSans-48"/>
       <use x="517.529297" xlink:href="#DejaVuSans-49"/>
      </g>
     </g>
    </g>
    <g id="xtick_7">
     <g id="line2d_7">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="317.273888" xlink:href="#m4ab79eac75" y="59.005985"/>
      </g>
     </g>
     <g id="text_7">
      <!-- 2020-06-22 -->
      <g transform="translate(288.216076 73.604422)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-54"/>
       <use x="417.822266" xlink:href="#DejaVuSans-45"/>
       <use x="453.90625" xlink:href="#DejaVuSans-50"/>
       <use x="517.529297" xlink:href="#DejaVuSans-50"/>
      </g>
     </g>
    </g>
    <g id="xtick_8">
     <g id="line2d_8">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="338.483816" xlink:href="#m4ab79eac75" y="59.005985"/>
      </g>
     </g>
     <g id="text_8">
      <!-- 2020-07-01 -->
      <defs>
       <path d="M 8.203125 72.90625 
L 55.078125 72.90625 
L 55.078125 68.703125 
L 28.609375 0 
L 18.3125 0 
L 43.21875 64.59375 
L 8.203125 64.59375 
z
" id="DejaVuSans-55"/>
      </defs>
      <g transform="translate(309.426003 73.604422)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-55"/>
       <use x="417.822266" xlink:href="#DejaVuSans-45"/>
       <use x="453.90625" xlink:href="#DejaVuSans-48"/>
       <use x="517.529297" xlink:href="#DejaVuSans-49"/>
      </g>
     </g>
    </g>
    <g id="xtick_9">
     <g id="line2d_9">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="387.973646" xlink:href="#m4ab79eac75" y="59.005985"/>
      </g>
     </g>
     <g id="text_9">
      <!-- 2020-07-22 -->
      <g transform="translate(358.915834 73.604422)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-55"/>
       <use x="417.822266" xlink:href="#DejaVuSans-45"/>
       <use x="453.90625" xlink:href="#DejaVuSans-50"/>
       <use x="517.529297" xlink:href="#DejaVuSans-50"/>
      </g>
     </g>
    </g>
   </g>
   <g id="matplotlib.axis_2">
    <g id="ytick_1">
     <g id="line2d_10">
      <defs>
       <path d="M 0 0 
L -3.5 0 
" id="mb7d6af1451" style="stroke:#000000;stroke-width:0.8;"/>
      </defs>
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="53.328125" xlink:href="#mb7d6af1451" y="58.692044"/>
      </g>
     </g>
     <g id="text_10">
      <!-- 0 -->
      <g transform="translate(39.965625 62.491263)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-48"/>
      </g>
     </g>
    </g>
    <g id="ytick_2">
     <g id="line2d_11">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="53.328125" xlink:href="#mb7d6af1451" y="29.890144"/>
      </g>
     </g>
     <g id="text_11">
      <!-- 5000 -->
      <g transform="translate(20.878125 33.689363)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-53"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-48"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
      </g>
     </g>
    </g>
   </g>
   <g id="line2d_12">
    <path clip-path="url(#p98d895b6a3)" d="M 53.328125 56.946649 
L 55.684784 56.848723 
L 58.041442 56.111394 
L 60.398101 55.783052 
L 62.754759 54.325676 
L 65.111418 53.006549 
L 67.468077 50.978895 
L 69.824735 47.009994 
L 72.181394 43.853305 
L 74.538052 40.045694 
L 76.894711 37.914354 
L 79.25137 33.507663 
L 81.608028 33.081395 
L 83.964687 31.762268 
L 86.321345 23.985755 
L 88.678004 28.507653 
L 91.034663 28.173551 
L 93.391321 31.428166 
L 95.74798 27.960417 
L 98.104638 33.092916 
L 100.461297 36.710434 
L 102.817956 28.980004 
L 105.174614 35.160892 
L 107.531273 33.196603 
L 109.887931 35.604441 
L 112.24459 34.924717 
L 114.601249 36.324489 
L 116.957907 39.878643 
L 119.314566 33.380935 
L 121.671224 38.023801 
L 124.027883 35.333703 
L 126.384542 37.182785 
L 128.7412 37.159744 
L 131.097859 41.324499 
L 133.454517 43.156299 
L 135.811176 39.400532 
L 138.167835 41.134406 
L 142.881152 43.133258 
L 145.23781 45.28764 
L 147.594469 47.096399 
L 152.307786 47.781885 
L 154.664445 47.476584 
L 157.021103 47.586032 
L 159.377762 48.582577 
L 161.734421 49.175897 
L 164.091079 50.414378 
L 166.447738 51.163228 
L 168.804396 49.596404 
L 171.161055 50.89249 
L 173.517714 51.186269 
L 175.874372 51.35332 
L 182.944348 53.484661 
L 185.301007 52.338345 
L 187.657665 53.236964 
L 190.014324 53.703555 
L 192.370982 53.271527 
L 194.727641 53.962772 
L 197.0843 54.406321 
L 199.440958 54.314155 
L 201.797617 53.536504 
L 206.510934 54.371759 
L 211.224251 54.769225 
L 213.58091 55.310701 
L 215.937568 55.495033 
L 218.294227 54.884433 
L 223.007544 55.304941 
L 225.364203 55.673605 
L 227.720861 54.780746 
L 232.434179 56.145956 
L 234.790837 55.132129 
L 237.147496 55.978905 
L 239.504154 55.43743 
L 241.860813 56.445496 
L 248.930789 56.549183 
L 251.287447 56.007707 
L 253.644106 56.186279 
L 256.000765 56.065311 
L 258.357423 56.491579 
L 260.714082 56.670151 
L 263.070741 57.010013 
L 265.427399 57.165543 
L 267.784058 56.791119 
L 270.140716 56.163237 
L 277.210692 56.877524 
L 279.567351 56.981211 
L 281.924009 57.338355 
L 284.280668 56.307247 
L 286.637327 56.122915 
L 288.993985 56.220841 
L 291.350644 56.554943 
L 298.42062 56.629828 
L 300.777278 54.976599 
L 303.133937 52.223137 
L 305.490595 54.83835 
L 307.847254 55.587199 
L 310.203913 55.385586 
L 314.91723 56.537662 
L 317.273888 55.944343 
L 319.630547 56.226602 
L 321.987206 56.001947 
L 324.343864 56.364851 
L 326.700523 56.20356 
L 329.057181 56.65863 
L 331.41384 56.871764 
L 333.770499 56.238122 
L 336.127157 56.140196 
L 340.840474 56.710473 
L 343.197133 56.687432 
L 345.553792 56.986972 
L 347.91045 56.96393 
L 350.267109 56.618307 
L 354.980426 56.762317 
L 359.693743 56.157477 
L 362.050402 56.422454 
L 364.40706 56.572224 
L 366.763719 55.581439 
L 369.120378 55.650564 
L 371.477036 55.512314 
L 373.833695 55.978905 
L 376.190353 55.679365 
L 378.547012 55.978905 
L 380.903671 55.74273 
L 383.260329 55.022682 
L 385.616988 54.654018 
L 387.973646 54.452405 
L 390.330305 54.798027 
L 392.686964 54.596414 
L 395.043622 55.063005 
L 397.400281 54.665539 
L 399.756939 52.925904 
L 402.113598 53.749638 
L 402.113598 53.749638 
" style="fill:none;stroke:#1f77b4;stroke-linecap:square;stroke-width:1.5;"/>
   </g>
   <g id="patch_3">
    <path d="M 53.328125 59.005985 
L 53.328125 22.318125 
" style="fill:none;stroke:#000000;stroke-linecap:square;stroke-linejoin:miter;stroke-width:0.8;"/>
   </g>
   <g id="patch_4">
    <path d="M 402.113598 59.005985 
L 402.113598 22.318125 
" style="fill:none;stroke:#000000;stroke-linecap:square;stroke-linejoin:miter;stroke-width:0.8;"/>
   </g>
   <g id="patch_5">
    <path d="M 53.328125 59.005985 
L 402.113598 59.005985 
" style="fill:none;stroke:#000000;stroke-linecap:square;stroke-linejoin:miter;stroke-width:0.8;"/>
   </g>
   <g id="patch_6">
    <path d="M 53.328125 22.318125 
L 402.113598 22.318125 
" style="fill:none;stroke:#000000;stroke-linecap:square;stroke-linejoin:miter;stroke-width:0.8;"/>
   </g>
   <g id="text_12">
    <!-- b -->
    <defs>
     <path d="M 48.6875 27.296875 
Q 48.6875 37.203125 44.609375 42.84375 
Q 40.53125 48.484375 33.40625 48.484375 
Q 26.265625 48.484375 22.1875 42.84375 
Q 18.109375 37.203125 18.109375 27.296875 
Q 18.109375 17.390625 22.1875 11.75 
Q 26.265625 6.109375 33.40625 6.109375 
Q 40.53125 6.109375 44.609375 11.75 
Q 48.6875 17.390625 48.6875 27.296875 
z
M 18.109375 46.390625 
Q 20.953125 51.265625 25.265625 53.625 
Q 29.59375 56 35.59375 56 
Q 45.5625 56 51.78125 48.09375 
Q 58.015625 40.1875 58.015625 27.296875 
Q 58.015625 14.40625 51.78125 6.484375 
Q 45.5625 -1.421875 35.59375 -1.421875 
Q 29.59375 -1.421875 25.265625 0.953125 
Q 20.953125 3.328125 18.109375 8.203125 
L 18.109375 0 
L 9.078125 0 
L 9.078125 75.984375 
L 18.109375 75.984375 
z
" id="DejaVuSans-98"/>
    </defs>
    <g transform="translate(223.911799 16.318125)scale(0.12 -0.12)">
     <use xlink:href="#DejaVuSans-98"/>
    </g>
   </g>
  </g>
  <g id="axes_2">
   <g id="patch_7">
    <path d="M 53.328125 124.576698 
L 402.113598 124.576698 
L 402.113598 87.888838 
L 53.328125 87.888838 
z
" style="fill:#ffffff;"/>
   </g>
   <g id="matplotlib.axis_3">
    <g id="xtick_10">
     <g id="line2d_13">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="100.461297" xlink:href="#m4ab79eac75" y="124.576698"/>
      </g>
     </g>
     <g id="text_13">
      <!-- 2020-03-22 -->
      <g transform="translate(71.403485 139.175136)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-51"/>
       <use x="417.822266" xlink:href="#DejaVuSans-45"/>
       <use x="453.90625" xlink:href="#DejaVuSans-50"/>
       <use x="517.529297" xlink:href="#DejaVuSans-50"/>
      </g>
     </g>
    </g>
    <g id="xtick_11">
     <g id="line2d_14">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="124.027883" xlink:href="#m4ab79eac75" y="124.576698"/>
      </g>
     </g>
     <g id="text_14">
      <!-- 2020-04-01 -->
      <g transform="translate(94.970071 139.175136)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-52"/>
       <use x="417.822266" xlink:href="#DejaVuSans-45"/>
       <use x="453.90625" xlink:href="#DejaVuSans-48"/>
       <use x="517.529297" xlink:href="#DejaVuSans-49"/>
      </g>
     </g>
    </g>
    <g id="xtick_12">
     <g id="line2d_15">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="173.517714" xlink:href="#m4ab79eac75" y="124.576698"/>
      </g>
     </g>
     <g id="text_15">
      <!-- 2020-04-22 -->
      <g transform="translate(144.459901 139.175136)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-52"/>
       <use x="417.822266" xlink:href="#DejaVuSans-45"/>
       <use x="453.90625" xlink:href="#DejaVuSans-50"/>
       <use x="517.529297" xlink:href="#DejaVuSans-50"/>
      </g>
     </g>
    </g>
    <g id="xtick_13">
     <g id="line2d_16">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="194.727641" xlink:href="#m4ab79eac75" y="124.576698"/>
      </g>
     </g>
     <g id="text_16">
      <!-- 2020-05-01 -->
      <g transform="translate(165.669829 139.175136)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-53"/>
       <use x="417.822266" xlink:href="#DejaVuSans-45"/>
       <use x="453.90625" xlink:href="#DejaVuSans-48"/>
       <use x="517.529297" xlink:href="#DejaVuSans-49"/>
      </g>
     </g>
    </g>
    <g id="xtick_14">
     <g id="line2d_17">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="244.217472" xlink:href="#m4ab79eac75" y="124.576698"/>
      </g>
     </g>
     <g id="text_17">
      <!-- 2020-05-22 -->
      <g transform="translate(215.159659 139.175136)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-53"/>
       <use x="417.822266" xlink:href="#DejaVuSans-45"/>
       <use x="453.90625" xlink:href="#DejaVuSans-50"/>
       <use x="517.529297" xlink:href="#DejaVuSans-50"/>
      </g>
     </g>
    </g>
    <g id="xtick_15">
     <g id="line2d_18">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="267.784058" xlink:href="#m4ab79eac75" y="124.576698"/>
      </g>
     </g>
     <g id="text_18">
      <!-- 2020-06-01 -->
      <g transform="translate(238.726245 139.175136)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-54"/>
       <use x="417.822266" xlink:href="#DejaVuSans-45"/>
       <use x="453.90625" xlink:href="#DejaVuSans-48"/>
       <use x="517.529297" xlink:href="#DejaVuSans-49"/>
      </g>
     </g>
    </g>
    <g id="xtick_16">
     <g id="line2d_19">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="317.273888" xlink:href="#m4ab79eac75" y="124.576698"/>
      </g>
     </g>
     <g id="text_19">
      <!-- 2020-06-22 -->
      <g transform="translate(288.216076 139.175136)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-54"/>
       <use x="417.822266" xlink:href="#DejaVuSans-45"/>
       <use x="453.90625" xlink:href="#DejaVuSans-50"/>
       <use x="517.529297" xlink:href="#DejaVuSans-50"/>
      </g>
     </g>
    </g>
    <g id="xtick_17">
     <g id="line2d_20">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="338.483816" xlink:href="#m4ab79eac75" y="124.576698"/>
      </g>
     </g>
     <g id="text_20">
      <!-- 2020-07-01 -->
      <g transform="translate(309.426003 139.175136)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-55"/>
       <use x="417.822266" xlink:href="#DejaVuSans-45"/>
       <use x="453.90625" xlink:href="#DejaVuSans-48"/>
       <use x="517.529297" xlink:href="#DejaVuSans-49"/>
      </g>
     </g>
    </g>
    <g id="xtick_18">
     <g id="line2d_21">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="387.973646" xlink:href="#m4ab79eac75" y="124.576698"/>
      </g>
     </g>
     <g id="text_21">
      <!-- 2020-07-22 -->
      <g transform="translate(358.915834 139.175136)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-55"/>
       <use x="417.822266" xlink:href="#DejaVuSans-45"/>
       <use x="453.90625" xlink:href="#DejaVuSans-50"/>
       <use x="517.529297" xlink:href="#DejaVuSans-50"/>
      </g>
     </g>
    </g>
   </g>
   <g id="matplotlib.axis_4">
    <g id="ytick_3">
     <g id="line2d_22">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="53.328125" xlink:href="#mb7d6af1451" y="107.773839"/>
      </g>
     </g>
     <g id="text_22">
      <!-- 2500 -->
      <g transform="translate(20.878125 111.573058)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-53"/>
       <use x="127.246094" xlink:href="#DejaVuSans-48"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
      </g>
     </g>
    </g>
    <g id="ytick_4">
     <g id="line2d_23">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="53.328125" xlink:href="#mb7d6af1451" y="90.307042"/>
      </g>
     </g>
     <g id="text_23">
      <!-- 5000 -->
      <g transform="translate(20.878125 94.10626)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-53"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-48"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
      </g>
     </g>
    </g>
    <g id="text_24">
     <!-- Trend -->
     <defs>
      <path d="M -0.296875 72.90625 
L 61.375 72.90625 
L 61.375 64.59375 
L 35.5 64.59375 
L 35.5 0 
L 25.59375 0 
L 25.59375 64.59375 
L -0.296875 64.59375 
z
" id="DejaVuSans-84"/>
      <path d="M 41.109375 46.296875 
Q 39.59375 47.171875 37.8125 47.578125 
Q 36.03125 48 33.890625 48 
Q 26.265625 48 22.1875 43.046875 
Q 18.109375 38.09375 18.109375 28.8125 
L 18.109375 0 
L 9.078125 0 
L 9.078125 54.6875 
L 18.109375 54.6875 
L 18.109375 46.1875 
Q 20.953125 51.171875 25.484375 53.578125 
Q 30.03125 56 36.53125 56 
Q 37.453125 56 38.578125 55.875 
Q 39.703125 55.765625 41.0625 55.515625 
z
" id="DejaVuSans-114"/>
      <path d="M 56.203125 29.59375 
L 56.203125 25.203125 
L 14.890625 25.203125 
Q 15.484375 15.921875 20.484375 11.0625 
Q 25.484375 6.203125 34.421875 6.203125 
Q 39.59375 6.203125 44.453125 7.46875 
Q 49.3125 8.734375 54.109375 11.28125 
L 54.109375 2.78125 
Q 49.265625 0.734375 44.1875 -0.34375 
Q 39.109375 -1.421875 33.890625 -1.421875 
Q 20.796875 -1.421875 13.15625 6.1875 
Q 5.515625 13.8125 5.515625 26.8125 
Q 5.515625 40.234375 12.765625 48.109375 
Q 20.015625 56 32.328125 56 
Q 43.359375 56 49.78125 48.890625 
Q 56.203125 41.796875 56.203125 29.59375 
z
M 47.21875 32.234375 
Q 47.125 39.59375 43.09375 43.984375 
Q 39.0625 48.390625 32.421875 48.390625 
Q 24.90625 48.390625 20.390625 44.140625 
Q 15.875 39.890625 15.1875 32.171875 
z
" id="DejaVuSans-101"/>
      <path d="M 54.890625 33.015625 
L 54.890625 0 
L 45.90625 0 
L 45.90625 32.71875 
Q 45.90625 40.484375 42.875 44.328125 
Q 39.84375 48.1875 33.796875 48.1875 
Q 26.515625 48.1875 22.3125 43.546875 
Q 18.109375 38.921875 18.109375 30.90625 
L 18.109375 0 
L 9.078125 0 
L 9.078125 54.6875 
L 18.109375 54.6875 
L 18.109375 46.1875 
Q 21.34375 51.125 25.703125 53.5625 
Q 30.078125 56 35.796875 56 
Q 45.21875 56 50.046875 50.171875 
Q 54.890625 44.34375 54.890625 33.015625 
z
" id="DejaVuSans-110"/>
      <path d="M 45.40625 46.390625 
L 45.40625 75.984375 
L 54.390625 75.984375 
L 54.390625 0 
L 45.40625 0 
L 45.40625 8.203125 
Q 42.578125 3.328125 38.25 0.953125 
Q 33.9375 -1.421875 27.875 -1.421875 
Q 17.96875 -1.421875 11.734375 6.484375 
Q 5.515625 14.40625 5.515625 27.296875 
Q 5.515625 40.1875 11.734375 48.09375 
Q 17.96875 56 27.875 56 
Q 33.9375 56 38.25 53.625 
Q 42.578125 51.265625 45.40625 46.390625 
z
M 14.796875 27.296875 
Q 14.796875 17.390625 18.875 11.75 
Q 22.953125 6.109375 30.078125 6.109375 
Q 37.203125 6.109375 41.296875 11.75 
Q 45.40625 17.390625 45.40625 27.296875 
Q 45.40625 37.203125 41.296875 42.84375 
Q 37.203125 48.484375 30.078125 48.484375 
Q 22.953125 48.484375 18.875 42.84375 
Q 14.796875 37.203125 14.796875 27.296875 
z
" id="DejaVuSans-100"/>
     </defs>
     <g transform="translate(14.798438 120.749175)rotate(-90)scale(0.1 -0.1)">
      <use xlink:href="#DejaVuSans-84"/>
      <use x="60.865234" xlink:href="#DejaVuSans-114"/>
      <use x="101.947266" xlink:href="#DejaVuSans-101"/>
      <use x="163.470703" xlink:href="#DejaVuSans-110"/>
      <use x="226.849609" xlink:href="#DejaVuSans-100"/>
     </g>
    </g>
   </g>
   <g id="line2d_24">
    <path clip-path="url(#pb237cea683)" d="M 60.398101 120.589478 
L 62.754759 118.86775 
L 65.111418 116.616031 
L 67.468077 113.832322 
L 69.824735 110.736208 
L 74.538052 103.676627 
L 76.894711 100.346957 
L 79.25137 96.35754 
L 81.608028 93.698595 
L 83.964687 91.641505 
L 86.321345 90.517641 
L 88.678004 89.556468 
L 91.034663 89.558465 
L 95.74798 91.28119 
L 98.104638 92.433998 
L 100.461297 93.304344 
L 102.817956 94.027968 
L 105.174614 95.234675 
L 109.887931 96.343567 
L 112.24459 97.106117 
L 114.601249 97.602174 
L 121.671224 98.633214 
L 124.027883 99.499567 
L 126.384542 100.067488 
L 128.7412 101.110505 
L 131.097859 101.649481 
L 133.454517 102.830236 
L 135.811176 103.861276 
L 138.167835 105.269599 
L 140.524493 106.269698 
L 142.881152 107.006298 
L 145.23781 108.458537 
L 147.594469 109.557448 
L 152.307786 111.443863 
L 157.021103 112.692489 
L 159.377762 113.343252 
L 161.734421 113.657654 
L 168.804396 115.353431 
L 173.517714 116.283663 
L 187.657665 118.663139 
L 190.014324 118.926638 
L 204.154275 119.8938 
L 208.867593 120.255113 
L 215.937568 120.848984 
L 218.294227 121.030639 
L 223.007544 121.063576 
L 230.07752 121.369994 
L 234.790837 121.526696 
L 239.504154 122.015766 
L 270.140716 122.863156 
L 284.280668 122.738393 
L 291.350644 122.493858 
L 300.777278 122.115577 
L 305.490595 121.804169 
L 310.203913 121.811155 
L 319.630547 122.192431 
L 324.343864 122.369095 
L 350.267109 122.875133 
L 359.693743 122.437964 
L 366.763719 121.953884 
L 376.190353 121.553645 
L 390.330305 120.459724 
L 392.686964 120.096415 
L 395.043622 119.939713 
L 395.043622 119.939713 
" style="fill:none;stroke:#1f77b4;stroke-linecap:square;stroke-width:1.5;"/>
   </g>
   <g id="patch_8">
    <path d="M 53.328125 124.576698 
L 53.328125 87.888838 
" style="fill:none;stroke:#000000;stroke-linecap:square;stroke-linejoin:miter;stroke-width:0.8;"/>
   </g>
   <g id="patch_9">
    <path d="M 402.113598 124.576698 
L 402.113598 87.888838 
" style="fill:none;stroke:#000000;stroke-linecap:square;stroke-linejoin:miter;stroke-width:0.8;"/>
   </g>
   <g id="patch_10">
    <path d="M 53.328125 124.576698 
L 402.113598 124.576698 
" style="fill:none;stroke:#000000;stroke-linecap:square;stroke-linejoin:miter;stroke-width:0.8;"/>
   </g>
   <g id="patch_11">
    <path d="M 53.328125 87.888838 
L 402.113598 87.888838 
" style="fill:none;stroke:#000000;stroke-linecap:square;stroke-linejoin:miter;stroke-width:0.8;"/>
   </g>
  </g>
  <g id="axes_3">
   <g id="patch_12">
    <path d="M 53.328125 190.147412 
L 402.113598 190.147412 
L 402.113598 153.459552 
L 53.328125 153.459552 
z
" style="fill:#ffffff;"/>
   </g>
   <g id="matplotlib.axis_5">
    <g id="xtick_19">
     <g id="line2d_25">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="100.461297" xlink:href="#m4ab79eac75" y="190.147412"/>
      </g>
     </g>
     <g id="text_25">
      <!-- 2020-03-22 -->
      <g transform="translate(71.403485 204.745849)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-51"/>
       <use x="417.822266" xlink:href="#DejaVuSans-45"/>
       <use x="453.90625" xlink:href="#DejaVuSans-50"/>
       <use x="517.529297" xlink:href="#DejaVuSans-50"/>
      </g>
     </g>
    </g>
    <g id="xtick_20">
     <g id="line2d_26">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="124.027883" xlink:href="#m4ab79eac75" y="190.147412"/>
      </g>
     </g>
     <g id="text_26">
      <!-- 2020-04-01 -->
      <g transform="translate(94.970071 204.745849)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-52"/>
       <use x="417.822266" xlink:href="#DejaVuSans-45"/>
       <use x="453.90625" xlink:href="#DejaVuSans-48"/>
       <use x="517.529297" xlink:href="#DejaVuSans-49"/>
      </g>
     </g>
    </g>
    <g id="xtick_21">
     <g id="line2d_27">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="173.517714" xlink:href="#m4ab79eac75" y="190.147412"/>
      </g>
     </g>
     <g id="text_27">
      <!-- 2020-04-22 -->
      <g transform="translate(144.459901 204.745849)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-52"/>
       <use x="417.822266" xlink:href="#DejaVuSans-45"/>
       <use x="453.90625" xlink:href="#DejaVuSans-50"/>
       <use x="517.529297" xlink:href="#DejaVuSans-50"/>
      </g>
     </g>
    </g>
    <g id="xtick_22">
     <g id="line2d_28">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="194.727641" xlink:href="#m4ab79eac75" y="190.147412"/>
      </g>
     </g>
     <g id="text_28">
      <!-- 2020-05-01 -->
      <g transform="translate(165.669829 204.745849)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-53"/>
       <use x="417.822266" xlink:href="#DejaVuSans-45"/>
       <use x="453.90625" xlink:href="#DejaVuSans-48"/>
       <use x="517.529297" xlink:href="#DejaVuSans-49"/>
      </g>
     </g>
    </g>
    <g id="xtick_23">
     <g id="line2d_29">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="244.217472" xlink:href="#m4ab79eac75" y="190.147412"/>
      </g>
     </g>
     <g id="text_29">
      <!-- 2020-05-22 -->
      <g transform="translate(215.159659 204.745849)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-53"/>
       <use x="417.822266" xlink:href="#DejaVuSans-45"/>
       <use x="453.90625" xlink:href="#DejaVuSans-50"/>
       <use x="517.529297" xlink:href="#DejaVuSans-50"/>
      </g>
     </g>
    </g>
    <g id="xtick_24">
     <g id="line2d_30">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="267.784058" xlink:href="#m4ab79eac75" y="190.147412"/>
      </g>
     </g>
     <g id="text_30">
      <!-- 2020-06-01 -->
      <g transform="translate(238.726245 204.745849)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-54"/>
       <use x="417.822266" xlink:href="#DejaVuSans-45"/>
       <use x="453.90625" xlink:href="#DejaVuSans-48"/>
       <use x="517.529297" xlink:href="#DejaVuSans-49"/>
      </g>
     </g>
    </g>
    <g id="xtick_25">
     <g id="line2d_31">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="317.273888" xlink:href="#m4ab79eac75" y="190.147412"/>
      </g>
     </g>
     <g id="text_31">
      <!-- 2020-06-22 -->
      <g transform="translate(288.216076 204.745849)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-54"/>
       <use x="417.822266" xlink:href="#DejaVuSans-45"/>
       <use x="453.90625" xlink:href="#DejaVuSans-50"/>
       <use x="517.529297" xlink:href="#DejaVuSans-50"/>
      </g>
     </g>
    </g>
    <g id="xtick_26">
     <g id="line2d_32">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="338.483816" xlink:href="#m4ab79eac75" y="190.147412"/>
      </g>
     </g>
     <g id="text_32">
      <!-- 2020-07-01 -->
      <g transform="translate(309.426003 204.745849)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-55"/>
       <use x="417.822266" xlink:href="#DejaVuSans-45"/>
       <use x="453.90625" xlink:href="#DejaVuSans-48"/>
       <use x="517.529297" xlink:href="#DejaVuSans-49"/>
      </g>
     </g>
    </g>
    <g id="xtick_27">
     <g id="line2d_33">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="387.973646" xlink:href="#m4ab79eac75" y="190.147412"/>
      </g>
     </g>
     <g id="text_33">
      <!-- 2020-07-22 -->
      <g transform="translate(358.915834 204.745849)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-55"/>
       <use x="417.822266" xlink:href="#DejaVuSans-45"/>
       <use x="453.90625" xlink:href="#DejaVuSans-50"/>
       <use x="517.529297" xlink:href="#DejaVuSans-50"/>
      </g>
     </g>
    </g>
   </g>
   <g id="matplotlib.axis_6">
    <g id="ytick_5">
     <g id="line2d_34">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="53.328125" xlink:href="#mb7d6af1451" y="182.25867"/>
      </g>
     </g>
     <g id="text_34">
      <!-- 0,9 -->
      <defs>
       <path d="M 11.71875 12.40625 
L 22.015625 12.40625 
L 22.015625 4 
L 14.015625 -11.625 
L 7.71875 -11.625 
L 11.71875 4 
z
" id="DejaVuSans-44"/>
       <path d="M 10.984375 1.515625 
L 10.984375 10.5 
Q 14.703125 8.734375 18.5 7.8125 
Q 22.3125 6.890625 25.984375 6.890625 
Q 35.75 6.890625 40.890625 13.453125 
Q 46.046875 20.015625 46.78125 33.40625 
Q 43.953125 29.203125 39.59375 26.953125 
Q 35.25 24.703125 29.984375 24.703125 
Q 19.046875 24.703125 12.671875 31.3125 
Q 6.296875 37.9375 6.296875 49.421875 
Q 6.296875 60.640625 12.9375 67.421875 
Q 19.578125 74.21875 30.609375 74.21875 
Q 43.265625 74.21875 49.921875 64.515625 
Q 56.59375 54.828125 56.59375 36.375 
Q 56.59375 19.140625 48.40625 8.859375 
Q 40.234375 -1.421875 26.421875 -1.421875 
Q 22.703125 -1.421875 18.890625 -0.6875 
Q 15.09375 0.046875 10.984375 1.515625 
z
M 30.609375 32.421875 
Q 37.25 32.421875 41.125 36.953125 
Q 45.015625 41.5 45.015625 49.421875 
Q 45.015625 57.28125 41.125 61.84375 
Q 37.25 66.40625 30.609375 66.40625 
Q 23.96875 66.40625 20.09375 61.84375 
Q 16.21875 57.28125 16.21875 49.421875 
Q 16.21875 41.5 20.09375 36.953125 
Q 23.96875 32.421875 30.609375 32.421875 
z
" id="DejaVuSans-57"/>
      </defs>
      <g transform="translate(30.425 186.057889)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-48"/>
       <use x="63.623047" xlink:href="#DejaVuSans-44"/>
       <use x="95.410156" xlink:href="#DejaVuSans-57"/>
      </g>
     </g>
    </g>
    <g id="ytick_6">
     <g id="line2d_35">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="53.328125" xlink:href="#mb7d6af1451" y="168.99117"/>
      </g>
     </g>
     <g id="text_35">
      <!-- 1,0 -->
      <g transform="translate(30.425 172.790389)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-49"/>
       <use x="63.623047" xlink:href="#DejaVuSans-44"/>
       <use x="95.410156" xlink:href="#DejaVuSans-48"/>
      </g>
     </g>
    </g>
    <g id="ytick_7">
     <g id="line2d_36">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="53.328125" xlink:href="#mb7d6af1451" y="155.72367"/>
      </g>
     </g>
     <g id="text_36">
      <!-- 1,1 -->
      <g transform="translate(30.425 159.522888)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-49"/>
       <use x="63.623047" xlink:href="#DejaVuSans-44"/>
       <use x="95.410156" xlink:href="#DejaVuSans-49"/>
      </g>
     </g>
    </g>
    <g id="text_37">
     <!-- Seasonal -->
     <defs>
      <path d="M 53.515625 70.515625 
L 53.515625 60.890625 
Q 47.90625 63.578125 42.921875 64.890625 
Q 37.9375 66.21875 33.296875 66.21875 
Q 25.25 66.21875 20.875 63.09375 
Q 16.5 59.96875 16.5 54.203125 
Q 16.5 49.359375 19.40625 46.890625 
Q 22.3125 44.4375 30.421875 42.921875 
L 36.375 41.703125 
Q 47.40625 39.59375 52.65625 34.296875 
Q 57.90625 29 57.90625 20.125 
Q 57.90625 9.515625 50.796875 4.046875 
Q 43.703125 -1.421875 29.984375 -1.421875 
Q 24.8125 -1.421875 18.96875 -0.25 
Q 13.140625 0.921875 6.890625 3.21875 
L 6.890625 13.375 
Q 12.890625 10.015625 18.65625 8.296875 
Q 24.421875 6.59375 29.984375 6.59375 
Q 38.421875 6.59375 43.015625 9.90625 
Q 47.609375 13.234375 47.609375 19.390625 
Q 47.609375 24.75 44.3125 27.78125 
Q 41.015625 30.8125 33.5 32.328125 
L 27.484375 33.5 
Q 16.453125 35.6875 11.515625 40.375 
Q 6.59375 45.0625 6.59375 53.421875 
Q 6.59375 63.09375 13.40625 68.65625 
Q 20.21875 74.21875 32.171875 74.21875 
Q 37.3125 74.21875 42.625 73.28125 
Q 47.953125 72.359375 53.515625 70.515625 
z
" id="DejaVuSans-83"/>
      <path d="M 34.28125 27.484375 
Q 23.390625 27.484375 19.1875 25 
Q 14.984375 22.515625 14.984375 16.5 
Q 14.984375 11.71875 18.140625 8.90625 
Q 21.296875 6.109375 26.703125 6.109375 
Q 34.1875 6.109375 38.703125 11.40625 
Q 43.21875 16.703125 43.21875 25.484375 
L 43.21875 27.484375 
z
M 52.203125 31.203125 
L 52.203125 0 
L 43.21875 0 
L 43.21875 8.296875 
Q 40.140625 3.328125 35.546875 0.953125 
Q 30.953125 -1.421875 24.3125 -1.421875 
Q 15.921875 -1.421875 10.953125 3.296875 
Q 6 8.015625 6 15.921875 
Q 6 25.140625 12.171875 29.828125 
Q 18.359375 34.515625 30.609375 34.515625 
L 43.21875 34.515625 
L 43.21875 35.40625 
Q 43.21875 41.609375 39.140625 45 
Q 35.0625 48.390625 27.6875 48.390625 
Q 23 48.390625 18.546875 47.265625 
Q 14.109375 46.140625 10.015625 43.890625 
L 10.015625 52.203125 
Q 14.9375 54.109375 19.578125 55.046875 
Q 24.21875 56 28.609375 56 
Q 40.484375 56 46.34375 49.84375 
Q 52.203125 43.703125 52.203125 31.203125 
z
" id="DejaVuSans-97"/>
      <path d="M 44.28125 53.078125 
L 44.28125 44.578125 
Q 40.484375 46.53125 36.375 47.5 
Q 32.28125 48.484375 27.875 48.484375 
Q 21.1875 48.484375 17.84375 46.4375 
Q 14.5 44.390625 14.5 40.28125 
Q 14.5 37.15625 16.890625 35.375 
Q 19.28125 33.59375 26.515625 31.984375 
L 29.59375 31.296875 
Q 39.15625 29.25 43.1875 25.515625 
Q 47.21875 21.78125 47.21875 15.09375 
Q 47.21875 7.46875 41.1875 3.015625 
Q 35.15625 -1.421875 24.609375 -1.421875 
Q 20.21875 -1.421875 15.453125 -0.5625 
Q 10.6875 0.296875 5.421875 2 
L 5.421875 11.28125 
Q 10.40625 8.6875 15.234375 7.390625 
Q 20.0625 6.109375 24.8125 6.109375 
Q 31.15625 6.109375 34.5625 8.28125 
Q 37.984375 10.453125 37.984375 14.40625 
Q 37.984375 18.0625 35.515625 20.015625 
Q 33.0625 21.96875 24.703125 23.78125 
L 21.578125 24.515625 
Q 13.234375 26.265625 9.515625 29.90625 
Q 5.8125 33.546875 5.8125 39.890625 
Q 5.8125 47.609375 11.28125 51.796875 
Q 16.75 56 26.8125 56 
Q 31.78125 56 36.171875 55.265625 
Q 40.578125 54.546875 44.28125 53.078125 
z
" id="DejaVuSans-115"/>
      <path d="M 30.609375 48.390625 
Q 23.390625 48.390625 19.1875 42.75 
Q 14.984375 37.109375 14.984375 27.296875 
Q 14.984375 17.484375 19.15625 11.84375 
Q 23.34375 6.203125 30.609375 6.203125 
Q 37.796875 6.203125 41.984375 11.859375 
Q 46.1875 17.53125 46.1875 27.296875 
Q 46.1875 37.015625 41.984375 42.703125 
Q 37.796875 48.390625 30.609375 48.390625 
z
M 30.609375 56 
Q 42.328125 56 49.015625 48.375 
Q 55.71875 40.765625 55.71875 27.296875 
Q 55.71875 13.875 49.015625 6.21875 
Q 42.328125 -1.421875 30.609375 -1.421875 
Q 18.84375 -1.421875 12.171875 6.21875 
Q 5.515625 13.875 5.515625 27.296875 
Q 5.515625 40.765625 12.171875 48.375 
Q 18.84375 56 30.609375 56 
z
" id="DejaVuSans-111"/>
      <path d="M 9.421875 75.984375 
L 18.40625 75.984375 
L 18.40625 0 
L 9.421875 0 
z
" id="DejaVuSans-108"/>
     </defs>
     <g transform="translate(24.345313 194.404263)rotate(-90)scale(0.1 -0.1)">
      <use xlink:href="#DejaVuSans-83"/>
      <use x="63.476562" xlink:href="#DejaVuSans-101"/>
      <use x="125" xlink:href="#DejaVuSans-97"/>
      <use x="186.279297" xlink:href="#DejaVuSans-115"/>
      <use x="238.378906" xlink:href="#DejaVuSans-111"/>
      <use x="299.560547" xlink:href="#DejaVuSans-110"/>
      <use x="362.939453" xlink:href="#DejaVuSans-97"/>
      <use x="424.21875" xlink:href="#DejaVuSans-108"/>
     </g>
    </g>
   </g>
   <g id="line2d_37">
    <path clip-path="url(#p1bc6f410b1)" d="M 53.328125 155.127182 
L 55.684784 160.749933 
L 58.041442 158.758447 
L 60.398101 170.920635 
L 62.754759 167.135143 
L 65.111418 181.767068 
L 67.468077 188.479782 
L 69.824735 155.127182 
L 72.181394 160.749933 
L 74.538052 158.758447 
L 76.894711 170.920635 
L 79.25137 167.135143 
L 81.608028 181.767068 
L 83.964687 188.479782 
L 86.321345 155.127182 
L 88.678004 160.749933 
L 91.034663 158.758447 
L 93.391321 170.920635 
L 95.74798 167.135143 
L 98.104638 181.767068 
L 100.461297 188.479782 
L 102.817956 155.127182 
L 105.174614 160.749933 
L 107.531273 158.758447 
L 109.887931 170.920635 
L 112.24459 167.135143 
L 114.601249 181.767068 
L 116.957907 188.479782 
L 119.314566 155.127182 
L 121.671224 160.749933 
L 124.027883 158.758447 
L 126.384542 170.920635 
L 128.7412 167.135143 
L 131.097859 181.767068 
L 133.454517 188.479782 
L 135.811176 155.127182 
L 138.167835 160.749933 
L 140.524493 158.758447 
L 142.881152 170.920635 
L 145.23781 167.135143 
L 147.594469 181.767068 
L 149.951128 188.479782 
L 152.307786 155.127182 
L 154.664445 160.749933 
L 157.021103 158.758447 
L 159.377762 170.920635 
L 161.734421 167.135143 
L 164.091079 181.767068 
L 166.447738 188.479782 
L 168.804396 155.127182 
L 171.161055 160.749933 
L 173.517714 158.758447 
L 175.874372 170.920635 
L 178.231031 167.135143 
L 180.587689 181.767068 
L 182.944348 188.479782 
L 185.301007 155.127182 
L 187.657665 160.749933 
L 190.014324 158.758447 
L 192.370982 170.920635 
L 194.727641 167.135143 
L 197.0843 181.767068 
L 199.440958 188.479782 
L 201.797617 155.127182 
L 204.154275 160.749933 
L 206.510934 158.758447 
L 208.867593 170.920635 
L 211.224251 167.135143 
L 213.58091 181.767068 
L 215.937568 188.479782 
L 218.294227 155.127182 
L 220.650886 160.749933 
L 223.007544 158.758447 
L 225.364203 170.920635 
L 227.720861 167.135143 
L 230.07752 181.767068 
L 232.434179 188.479782 
L 234.790837 155.127182 
L 237.147496 160.749933 
L 239.504154 158.758447 
L 241.860813 170.920635 
L 244.217472 167.135143 
L 246.57413 181.767068 
L 248.930789 188.479782 
L 251.287447 155.127182 
L 253.644106 160.749933 
L 256.000765 158.758447 
L 258.357423 170.920635 
L 260.714082 167.135143 
L 263.070741 181.767068 
L 265.427399 188.479782 
L 267.784058 155.127182 
L 270.140716 160.749933 
L 272.497375 158.758447 
L 274.854034 170.920635 
L 277.210692 167.135143 
L 279.567351 181.767068 
L 281.924009 188.479782 
L 284.280668 155.127182 
L 286.637327 160.749933 
L 288.993985 158.758447 
L 291.350644 170.920635 
L 293.707302 167.135143 
L 296.063961 181.767068 
L 298.42062 188.479782 
L 300.777278 155.127182 
L 303.133937 160.749933 
L 305.490595 158.758447 
L 307.847254 170.920635 
L 310.203913 167.135143 
L 312.560571 181.767068 
L 314.91723 188.479782 
L 317.273888 155.127182 
L 319.630547 160.749933 
L 321.987206 158.758447 
L 324.343864 170.920635 
L 326.700523 167.135143 
L 329.057181 181.767068 
L 331.41384 188.479782 
L 333.770499 155.127182 
L 336.127157 160.749933 
L 338.483816 158.758447 
L 340.840474 170.920635 
L 343.197133 167.135143 
L 345.553792 181.767068 
L 347.91045 188.479782 
L 350.267109 155.127182 
L 352.623767 160.749933 
L 354.980426 158.758447 
L 357.337085 170.920635 
L 359.693743 167.135143 
L 362.050402 181.767068 
L 364.40706 188.479782 
L 366.763719 155.127182 
L 369.120378 160.749933 
L 371.477036 158.758447 
L 373.833695 170.920635 
L 376.190353 167.135143 
L 378.547012 181.767068 
L 380.903671 188.479782 
L 383.260329 155.127182 
L 385.616988 160.749933 
L 387.973646 158.758447 
L 390.330305 170.920635 
L 392.686964 167.135143 
L 395.043622 181.767068 
L 397.400281 188.479782 
L 399.756939 155.127182 
L 402.113598 160.749933 
L 402.113598 160.749933 
" style="fill:none;stroke:#1f77b4;stroke-linecap:square;stroke-width:1.5;"/>
   </g>
   <g id="patch_13">
    <path d="M 53.328125 190.147412 
L 53.328125 153.459552 
" style="fill:none;stroke:#000000;stroke-linecap:square;stroke-linejoin:miter;stroke-width:0.8;"/>
   </g>
   <g id="patch_14">
    <path d="M 402.113598 190.147412 
L 402.113598 153.459552 
" style="fill:none;stroke:#000000;stroke-linecap:square;stroke-linejoin:miter;stroke-width:0.8;"/>
   </g>
   <g id="patch_15">
    <path d="M 53.328125 190.147412 
L 402.113598 190.147412 
" style="fill:none;stroke:#000000;stroke-linecap:square;stroke-linejoin:miter;stroke-width:0.8;"/>
   </g>
   <g id="patch_16">
    <path d="M 53.328125 153.459552 
L 402.113598 153.459552 
" style="fill:none;stroke:#000000;stroke-linecap:square;stroke-linejoin:miter;stroke-width:0.8;"/>
   </g>
  </g>
  <g id="axes_4">
   <g id="patch_17">
    <path d="M 53.328125 255.718125 
L 402.113598 255.718125 
L 402.113598 219.030265 
L 53.328125 219.030265 
z
" style="fill:#ffffff;"/>
   </g>
   <g id="line2d_38">
    <path clip-path="url(#p4da15ee730)" d="M 53.328125 254.050495 
L 402.113598 254.050495 
" style="fill:none;stroke:#000000;stroke-linecap:square;stroke-width:1.5;"/>
   </g>
   <g id="matplotlib.axis_7">
    <g id="xtick_28">
     <g id="line2d_39">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="100.461297" xlink:href="#m4ab79eac75" y="255.718125"/>
      </g>
     </g>
     <g id="text_38">
      <!-- 2020-03-22 -->
      <g transform="translate(71.403485 270.316563)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-51"/>
       <use x="417.822266" xlink:href="#DejaVuSans-45"/>
       <use x="453.90625" xlink:href="#DejaVuSans-50"/>
       <use x="517.529297" xlink:href="#DejaVuSans-50"/>
      </g>
     </g>
    </g>
    <g id="xtick_29">
     <g id="line2d_40">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="124.027883" xlink:href="#m4ab79eac75" y="255.718125"/>
      </g>
     </g>
     <g id="text_39">
      <!-- 2020-04-01 -->
      <g transform="translate(94.970071 270.316563)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-52"/>
       <use x="417.822266" xlink:href="#DejaVuSans-45"/>
       <use x="453.90625" xlink:href="#DejaVuSans-48"/>
       <use x="517.529297" xlink:href="#DejaVuSans-49"/>
      </g>
     </g>
    </g>
    <g id="xtick_30">
     <g id="line2d_41">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="173.517714" xlink:href="#m4ab79eac75" y="255.718125"/>
      </g>
     </g>
     <g id="text_40">
      <!-- 2020-04-22 -->
      <g transform="translate(144.459901 270.316563)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-52"/>
       <use x="417.822266" xlink:href="#DejaVuSans-45"/>
       <use x="453.90625" xlink:href="#DejaVuSans-50"/>
       <use x="517.529297" xlink:href="#DejaVuSans-50"/>
      </g>
     </g>
    </g>
    <g id="xtick_31">
     <g id="line2d_42">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="194.727641" xlink:href="#m4ab79eac75" y="255.718125"/>
      </g>
     </g>
     <g id="text_41">
      <!-- 2020-05-01 -->
      <g transform="translate(165.669829 270.316563)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-53"/>
       <use x="417.822266" xlink:href="#DejaVuSans-45"/>
       <use x="453.90625" xlink:href="#DejaVuSans-48"/>
       <use x="517.529297" xlink:href="#DejaVuSans-49"/>
      </g>
     </g>
    </g>
    <g id="xtick_32">
     <g id="line2d_43">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="244.217472" xlink:href="#m4ab79eac75" y="255.718125"/>
      </g>
     </g>
     <g id="text_42">
      <!-- 2020-05-22 -->
      <g transform="translate(215.159659 270.316563)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-53"/>
       <use x="417.822266" xlink:href="#DejaVuSans-45"/>
       <use x="453.90625" xlink:href="#DejaVuSans-50"/>
       <use x="517.529297" xlink:href="#DejaVuSans-50"/>
      </g>
     </g>
    </g>
    <g id="xtick_33">
     <g id="line2d_44">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="267.784058" xlink:href="#m4ab79eac75" y="255.718125"/>
      </g>
     </g>
     <g id="text_43">
      <!-- 2020-06-01 -->
      <g transform="translate(238.726245 270.316563)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-54"/>
       <use x="417.822266" xlink:href="#DejaVuSans-45"/>
       <use x="453.90625" xlink:href="#DejaVuSans-48"/>
       <use x="517.529297" xlink:href="#DejaVuSans-49"/>
      </g>
     </g>
    </g>
    <g id="xtick_34">
     <g id="line2d_45">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="317.273888" xlink:href="#m4ab79eac75" y="255.718125"/>
      </g>
     </g>
     <g id="text_44">
      <!-- 2020-06-22 -->
      <g transform="translate(288.216076 270.316563)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-54"/>
       <use x="417.822266" xlink:href="#DejaVuSans-45"/>
       <use x="453.90625" xlink:href="#DejaVuSans-50"/>
       <use x="517.529297" xlink:href="#DejaVuSans-50"/>
      </g>
     </g>
    </g>
    <g id="xtick_35">
     <g id="line2d_46">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="338.483816" xlink:href="#m4ab79eac75" y="255.718125"/>
      </g>
     </g>
     <g id="text_45">
      <!-- 2020-07-01 -->
      <g transform="translate(309.426003 270.316563)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-55"/>
       <use x="417.822266" xlink:href="#DejaVuSans-45"/>
       <use x="453.90625" xlink:href="#DejaVuSans-48"/>
       <use x="517.529297" xlink:href="#DejaVuSans-49"/>
      </g>
     </g>
    </g>
    <g id="xtick_36">
     <g id="line2d_47">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="387.973646" xlink:href="#m4ab79eac75" y="255.718125"/>
      </g>
     </g>
     <g id="text_46">
      <!-- 2020-07-22 -->
      <g transform="translate(358.915834 270.316563)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-55"/>
       <use x="417.822266" xlink:href="#DejaVuSans-45"/>
       <use x="453.90625" xlink:href="#DejaVuSans-50"/>
       <use x="517.529297" xlink:href="#DejaVuSans-50"/>
      </g>
     </g>
    </g>
   </g>
   <g id="matplotlib.axis_8">
    <g id="ytick_8">
     <g id="line2d_48">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="53.328125" xlink:href="#mb7d6af1451" y="254.050495"/>
      </g>
     </g>
     <g id="text_47">
      <!-- 0 -->
      <g transform="translate(39.965625 257.849714)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-48"/>
      </g>
     </g>
    </g>
    <g id="ytick_9">
     <g id="line2d_49">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="53.328125" xlink:href="#mb7d6af1451" y="226.591741"/>
      </g>
     </g>
     <g id="text_48">
      <!-- 1 -->
      <g transform="translate(39.965625 230.39096)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-49"/>
      </g>
     </g>
    </g>
    <g id="text_49">
     <!-- Resid -->
     <defs>
      <path d="M 44.390625 34.1875 
Q 47.5625 33.109375 50.5625 29.59375 
Q 53.5625 26.078125 56.59375 19.921875 
L 66.609375 0 
L 56 0 
L 46.6875 18.703125 
Q 43.0625 26.03125 39.671875 28.421875 
Q 36.28125 30.8125 30.421875 30.8125 
L 19.671875 30.8125 
L 19.671875 0 
L 9.8125 0 
L 9.8125 72.90625 
L 32.078125 72.90625 
Q 44.578125 72.90625 50.734375 67.671875 
Q 56.890625 62.453125 56.890625 51.90625 
Q 56.890625 45.015625 53.6875 40.46875 
Q 50.484375 35.9375 44.390625 34.1875 
z
M 19.671875 64.796875 
L 19.671875 38.921875 
L 32.078125 38.921875 
Q 39.203125 38.921875 42.84375 42.21875 
Q 46.484375 45.515625 46.484375 51.90625 
Q 46.484375 58.296875 42.84375 61.546875 
Q 39.203125 64.796875 32.078125 64.796875 
z
" id="DejaVuSans-82"/>
      <path d="M 9.421875 54.6875 
L 18.40625 54.6875 
L 18.40625 0 
L 9.421875 0 
z
M 9.421875 75.984375 
L 18.40625 75.984375 
L 18.40625 64.59375 
L 9.421875 64.59375 
z
" id="DejaVuSans-105"/>
     </defs>
     <g transform="translate(33.885938 251.08982)rotate(-90)scale(0.1 -0.1)">
      <use xlink:href="#DejaVuSans-82"/>
      <use x="69.419922" xlink:href="#DejaVuSans-101"/>
      <use x="130.943359" xlink:href="#DejaVuSans-115"/>
      <use x="183.042969" xlink:href="#DejaVuSans-105"/>
      <use x="210.826172" xlink:href="#DejaVuSans-100"/>
     </g>
    </g>
   </g>
   <g id="line2d_50">
    <defs>
     <path d="M 0 3 
C 0.795609 3 1.55874 2.683901 2.12132 2.12132 
C 2.683901 1.55874 3 0.795609 3 0 
C 3 -0.795609 2.683901 -1.55874 2.12132 -2.12132 
C 1.55874 -2.683901 0.795609 -3 0 -3 
C -0.795609 -3 -1.55874 -2.683901 -2.12132 -2.12132 
C -2.683901 -1.55874 -3 -0.795609 -3 0 
C -3 0.795609 -2.683901 1.55874 -2.12132 2.12132 
C -1.55874 2.683901 -0.795609 3 0 3 
z
" id="mfd83587dd5" style="stroke:#1f77b4;"/>
    </defs>
    <g clip-path="url(#p4da15ee730)">
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="60.398101" xlink:href="#mfd83587dd5" y="232.913339"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="62.754759" xlink:href="#mfd83587dd5" y="231.546801"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="65.111418" xlink:href="#mfd83587dd5" y="229.756151"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="67.468077" xlink:href="#mfd83587dd5" y="227.656319"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="69.824735" xlink:href="#mfd83587dd5" y="229.76442"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="72.181394" xlink:href="#mfd83587dd5" y="228.360035"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="74.538052" xlink:href="#mfd83587dd5" y="227.314233"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="76.894711" xlink:href="#mfd83587dd5" y="225.842424"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="79.25137" xlink:href="#mfd83587dd5" y="225.411541"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="81.608028" xlink:href="#mfd83587dd5" y="224.127371"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="83.964687" xlink:href="#mfd83587dd5" y="222.760711"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="86.321345" xlink:href="#mfd83587dd5" y="223.911422"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="88.678004" xlink:href="#mfd83587dd5" y="227.526565"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="91.034663" xlink:href="#mfd83587dd5" y="227.605215"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="93.391321" xlink:href="#mfd83587dd5" y="227.592058"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="95.74798" xlink:href="#mfd83587dd5" y="224.327364"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="98.104638" xlink:href="#mfd83587dd5" y="225.293759"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="100.461297" xlink:href="#mfd83587dd5" y="227.180173"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="102.817956" xlink:href="#mfd83587dd5" y="225.346625"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="105.174614" xlink:href="#mfd83587dd5" y="229.460034"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="107.531273" xlink:href="#mfd83587dd5" y="227.279025"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="109.887931" xlink:href="#mfd83587dd5" y="227.048849"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="112.24459" xlink:href="#mfd83587dd5" y="226.303851"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="114.601249" xlink:href="#mfd83587dd5" y="224.225472"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="116.957907" xlink:href="#mfd83587dd5" y="227.115975"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="119.314566" xlink:href="#mfd83587dd5" y="225.777502"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="121.671224" xlink:href="#mfd83587dd5" y="229.693046"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="124.027883" xlink:href="#mfd83587dd5" y="225.992813"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="126.384542" xlink:href="#mfd83587dd5" y="225.173426"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="128.7412" xlink:href="#mfd83587dd5" y="224.741538"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="131.097859" xlink:href="#mfd83587dd5" y="226.919522"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="133.454517" xlink:href="#mfd83587dd5" y="226.987221"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="135.811176" xlink:href="#mfd83587dd5" y="226.841628"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="138.167835" xlink:href="#mfd83587dd5" y="226.483051"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="140.524493" xlink:href="#mfd83587dd5" y="227.086569"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="142.881152" xlink:href="#mfd83587dd5" y="225.21344"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="145.23781" xlink:href="#mfd83587dd5" y="227.816112"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="147.594469" xlink:href="#mfd83587dd5" y="226.802365"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="149.951128" xlink:href="#mfd83587dd5" y="224.16523"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="152.307786" xlink:href="#mfd83587dd5" y="230.205763"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="154.664445" xlink:href="#mfd83587dd5" y="227.251828"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="157.021103" xlink:href="#mfd83587dd5" y="226.684268"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="159.377762" xlink:href="#mfd83587dd5" y="225.333303"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="161.734421" xlink:href="#mfd83587dd5" y="227.066242"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="164.091079" xlink:href="#mfd83587dd5" y="226.295407"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="166.447738" xlink:href="#mfd83587dd5" y="225.700093"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="168.804396" xlink:href="#mfd83587dd5" y="226.310998"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="171.161055" xlink:href="#mfd83587dd5" y="227.99141"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="173.517714" xlink:href="#mfd83587dd5" y="228.140304"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="175.874372" xlink:href="#mfd83587dd5" y="225.058438"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="178.231031" xlink:href="#mfd83587dd5" y="227.144523"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="180.587689" xlink:href="#mfd83587dd5" y="226.163662"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="182.944348" xlink:href="#mfd83587dd5" y="225.960977"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="185.301007" xlink:href="#mfd83587dd5" y="226.303898"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="187.657665" xlink:href="#mfd83587dd5" y="228.044619"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="190.014324" xlink:href="#mfd83587dd5" y="229.62176"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="192.370982" xlink:href="#mfd83587dd5" y="224.361074"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="194.727641" xlink:href="#mfd83587dd5" y="227.999552"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="197.0843" xlink:href="#mfd83587dd5" y="226.99113"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="199.440958" xlink:href="#mfd83587dd5" y="224.177334"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="201.797617" xlink:href="#mfd83587dd5" y="225.716222"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="204.154275" xlink:href="#mfd83587dd5" y="226.315478"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="206.510934" xlink:href="#mfd83587dd5" y="228.312768"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="208.867593" xlink:href="#mfd83587dd5" y="226.482174"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="211.224251" xlink:href="#mfd83587dd5" y="226.936442"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="213.58091" xlink:href="#mfd83587dd5" y="226.683012"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="215.937568" xlink:href="#mfd83587dd5" y="225.63115"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="218.294227" xlink:href="#mfd83587dd5" y="226.778955"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="220.650886" xlink:href="#mfd83587dd5" y="227.351389"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="223.007544" xlink:href="#mfd83587dd5" y="228.978198"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="225.364203" xlink:href="#mfd83587dd5" y="228.951021"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="227.720861" xlink:href="#mfd83587dd5" y="222.104383"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="230.07752" xlink:href="#mfd83587dd5" y="223.55617"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="232.434179" xlink:href="#mfd83587dd5" y="228.217685"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="234.790837" xlink:href="#mfd83587dd5" y="225.147451"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="237.147496" xlink:href="#mfd83587dd5" y="229.171062"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="239.504154" xlink:href="#mfd83587dd5" y="222.845526"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="241.860813" xlink:href="#mfd83587dd5" y="229.985753"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="244.217472" xlink:href="#mfd83587dd5" y="229.859455"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="246.57413" xlink:href="#mfd83587dd5" y="228.224068"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="248.930789" xlink:href="#mfd83587dd5" y="224.785821"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="251.287447" xlink:href="#mfd83587dd5" y="225.655454"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="253.644106" xlink:href="#mfd83587dd5" y="226.164554"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="256.000765" xlink:href="#mfd83587dd5" y="224.50351"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="258.357423" xlink:href="#mfd83587dd5" y="225.902302"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="260.714082" xlink:href="#mfd83587dd5" y="227.552933"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="263.070741" xlink:href="#mfd83587dd5" y="229.356185"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="265.427399" xlink:href="#mfd83587dd5" y="229.740142"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="267.784058" xlink:href="#mfd83587dd5" y="230.300013"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="270.140716" xlink:href="#mfd83587dd5" y="220.697895"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="272.497375" xlink:href="#mfd83587dd5" y="224.37142"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="274.854034" xlink:href="#mfd83587dd5" y="225.583609"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="277.210692" xlink:href="#mfd83587dd5" y="229.588702"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="279.567351" xlink:href="#mfd83587dd5" y="228.245899"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="281.924009" xlink:href="#mfd83587dd5" y="232.700885"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="284.280668" xlink:href="#mfd83587dd5" y="225.312214"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="286.637327" xlink:href="#mfd83587dd5" y="222.522103"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="288.993985" xlink:href="#mfd83587dd5" y="224.931326"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="291.350644" xlink:href="#mfd83587dd5" y="227.755894"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="293.707302" xlink:href="#mfd83587dd5" y="229.470548"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="296.063961" xlink:href="#mfd83587dd5" y="227.132988"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="298.42062" xlink:href="#mfd83587dd5" y="226.828175"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="300.777278" xlink:href="#mfd83587dd5" y="226.259652"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="303.133937" xlink:href="#mfd83587dd5" y="226.934801"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="305.490595" xlink:href="#mfd83587dd5" y="228.135851"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="307.847254" xlink:href="#mfd83587dd5" y="223.657094"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="310.203913" xlink:href="#mfd83587dd5" y="222.38369"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="312.560571" xlink:href="#mfd83587dd5" y="224.207799"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="314.91723" xlink:href="#mfd83587dd5" y="228.753395"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="317.273888" xlink:href="#mfd83587dd5" y="228.07724"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="319.630547" xlink:href="#mfd83587dd5" y="228.688602"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="321.987206" xlink:href="#mfd83587dd5" y="225.656857"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="324.343864" xlink:href="#mfd83587dd5" y="226.66109"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="326.700523" xlink:href="#mfd83587dd5" y="225.07325"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="329.057181" xlink:href="#mfd83587dd5" y="227.62303"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="331.41384" xlink:href="#mfd83587dd5" y="228.375464"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="333.770499" xlink:href="#mfd83587dd5" y="226.724588"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="336.127157" xlink:href="#mfd83587dd5" y="223.556097"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="338.483816" xlink:href="#mfd83587dd5" y="226.367428"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="340.840474" xlink:href="#mfd83587dd5" y="227.799928"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="343.197133" xlink:href="#mfd83587dd5" y="227.557845"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="345.553792" xlink:href="#mfd83587dd5" y="227.818428"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="347.91045" xlink:href="#mfd83587dd5" y="225.115582"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="350.267109" xlink:href="#mfd83587dd5" y="227.616127"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="352.623767" xlink:href="#mfd83587dd5" y="228.103111"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="354.980426" xlink:href="#mfd83587dd5" y="230.69887"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="357.337085" xlink:href="#mfd83587dd5" y="225.995672"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="359.693743" xlink:href="#mfd83587dd5" y="224.347443"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="362.050402" xlink:href="#mfd83587dd5" y="225.957696"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="364.40706" xlink:href="#mfd83587dd5" y="228.140245"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="366.763719" xlink:href="#mfd83587dd5" y="225.512937"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="369.120378" xlink:href="#mfd83587dd5" y="225.747108"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="371.477036" xlink:href="#mfd83587dd5" y="225.523583"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="373.833695" xlink:href="#mfd83587dd5" y="228.510455"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="376.190353" xlink:href="#mfd83587dd5" y="227.212485"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="378.547012" xlink:href="#mfd83587dd5" y="228.14459"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="380.903671" xlink:href="#mfd83587dd5" y="225.574331"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="383.260329" xlink:href="#mfd83587dd5" y="228.003802"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="385.616988" xlink:href="#mfd83587dd5" y="225.504125"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="387.973646" xlink:href="#mfd83587dd5" y="225.517385"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="390.330305" xlink:href="#mfd83587dd5" y="226.523913"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="392.686964" xlink:href="#mfd83587dd5" y="227.900555"/>
     <use style="fill:#1f77b4;stroke:#1f77b4;" x="395.043622" xlink:href="#mfd83587dd5" y="228.820551"/>
    </g>
   </g>
   <g id="patch_18">
    <path d="M 53.328125 255.718125 
L 53.328125 219.030265 
" style="fill:none;stroke:#000000;stroke-linecap:square;stroke-linejoin:miter;stroke-width:0.8;"/>
   </g>
   <g id="patch_19">
    <path d="M 402.113598 255.718125 
L 402.113598 219.030265 
" style="fill:none;stroke:#000000;stroke-linecap:square;stroke-linejoin:miter;stroke-width:0.8;"/>
   </g>
   <g id="patch_20">
    <path d="M 53.328125 255.718125 
L 402.113598 255.718125 
" style="fill:none;stroke:#000000;stroke-linecap:square;stroke-linejoin:miter;stroke-width:0.8;"/>
   </g>
   <g id="patch_21">
    <path d="M 53.328125 219.030265 
L 402.113598 219.030265 
" style="fill:none;stroke:#000000;stroke-linecap:square;stroke-linejoin:miter;stroke-width:0.8;"/>
   </g>
  </g>
 </g>
 <defs>
  <clipPath id="p98d895b6a3">
   <rect height="36.68786" width="348.785473" x="53.328125" y="22.318125"/>
  </clipPath>
  <clipPath id="pb237cea683">
   <rect height="36.68786" width="348.785473" x="53.328125" y="87.888838"/>
  </clipPath>
  <clipPath id="p1bc6f410b1">
   <rect height="36.68786" width="348.785473" x="53.328125" y="153.459552"/>
  </clipPath>
  <clipPath id="p4da15ee730">
   <rect height="36.68786" width="348.785473" x="53.328125" y="219.030265"/>
  </clipPath>
 </defs>
</svg>

</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[80]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">left_end</span><span class="o">=</span><span class="mi">50</span>
<span class="n">adjusted_b</span> <span class="o">=</span> <span class="n">result_b</span><span class="o">.</span><span class="n">observed</span> <span class="o">/</span> <span class="n">result_b</span><span class="o">.</span><span class="n">seasonal</span>
<span class="n">adjusted_c</span> <span class="o">=</span> <span class="n">nowcast</span><span class="o">.</span><span class="n">c</span><span class="p">[</span><span class="n">left_end</span><span class="p">:]</span> <span class="o">/</span> <span class="n">result_b</span><span class="o">.</span><span class="n">seasonal</span>
<span class="n">adjusted_d</span> <span class="o">=</span> <span class="n">nowcast</span><span class="o">.</span><span class="n">d</span><span class="p">[</span><span class="n">left_end</span><span class="p">:]</span> <span class="o">/</span> <span class="n">result_b</span><span class="o">.</span><span class="n">seasonal</span>

<span class="n">locale</span><span class="o">.</span><span class="n">setlocale</span><span class="p">(</span><span class="n">locale</span><span class="o">.</span><span class="n">LC_ALL</span><span class="p">,</span> <span class="s1">&#39;de_DE&#39;</span><span class="p">)</span>

<span class="n">fig</span> <span class="o">=</span> <span class="n">plt</span><span class="o">.</span><span class="n">figure</span><span class="p">(</span><span class="n">num</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span> <span class="n">figsize</span><span class="o">=</span><span class="p">(</span><span class="mf">6.75</span><span class="p">,</span> <span class="mf">3.5</span><span class="p">),</span> <span class="n">facecolor</span><span class="o">=</span><span class="s1">&#39;w&#39;</span><span class="p">,</span> <span class="n">edgecolor</span><span class="o">=</span><span class="s1">&#39;k&#39;</span><span class="p">)</span>

<span class="n">ax</span> <span class="o">=</span> <span class="n">adjusted_b</span><span class="p">[</span><span class="mi">2</span><span class="p">:]</span><span class="o">.</span><span class="n">plot</span><span class="p">()</span>
<span class="n">ax</span><span class="o">.</span><span class="n">fill_between</span><span class="p">(</span><span class="n">adjusted_b</span><span class="o">.</span><span class="n">index</span><span class="p">,</span><span class="n">adjusted_c</span><span class="p">,</span><span class="n">adjusted_d</span><span class="p">,</span><span class="n">color</span><span class="o">=</span><span class="s1">&#39;g&#39;</span><span class="p">,</span><span class="n">alpha</span><span class="o">=</span><span class="mf">0.3</span><span class="p">,</span><span class="n">lw</span><span class="o">=</span><span class="mi">0</span><span class="p">,</span><span class="n">zorder</span><span class="o">=</span><span class="mi">0</span><span class="p">)</span>
<span class="n">ax</span><span class="o">.</span><span class="n">set_xlim</span><span class="p">(</span><span class="n">left</span><span class="o">=</span><span class="n">nowcast</span><span class="o">.</span><span class="n">index</span><span class="p">[</span><span class="n">left_end</span><span class="p">],</span><span class="n">right</span><span class="o">=</span><span class="n">nowcast</span><span class="o">.</span><span class="n">index</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span><span class="o">+</span><span class="n">pd</span><span class="o">.</span><span class="n">Timedelta</span><span class="p">(</span><span class="n">days</span><span class="o">=</span><span class="mi">1</span><span class="p">))</span>
<span class="n">ax</span><span class="o">.</span><span class="n">set_ylim</span><span class="p">(</span><span class="n">top</span><span class="o">=</span><span class="mi">1500</span><span class="p">,</span><span class="n">bottom</span><span class="o">=</span><span class="mi">0</span><span class="p">)</span>
<span class="n">red_patch</span> <span class="o">=</span> <span class="n">mpatches</span><span class="o">.</span><span class="n">Patch</span><span class="p">(</span><span class="n">color</span><span class="o">=</span><span class="s1">&#39;green&#39;</span><span class="p">,</span> <span class="n">alpha</span><span class="o">=</span><span class="mf">0.3</span><span class="p">,</span> <span class="n">label</span><span class="o">=</span><span class="s1">&#39;95%-Prädiktionsintervall&#39;</span><span class="p">,</span><span class="n">ec</span><span class="o">=</span><span class="kc">None</span><span class="p">)</span>
<span class="n">ax</span><span class="o">.</span><span class="n">legend</span><span class="p">(</span><span class="n">handles</span><span class="o">=</span><span class="p">[</span><span class="n">red_patch</span><span class="p">],</span><span class="n">frameon</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s2">&quot;Deutsche COVID-19 Fallzahlen nach Erkrankungsbeginn&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s2">&quot;Saisonal bereinigte Fallzahlen&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s2">&quot;Datum des Erkrankungsbeginns&quot;</span><span class="p">)</span>
<span class="n">ax</span><span class="o">.</span><span class="n">tick_params</span><span class="p">(</span><span class="n">axis</span><span class="o">=</span><span class="s1">&#39;x&#39;</span><span class="p">,</span> <span class="n">which</span><span class="o">=</span><span class="s1">&#39;major&#39;</span><span class="p">,</span> <span class="n">pad</span><span class="o">=</span><span class="mi">5</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">grid</span><span class="p">(</span><span class="n">axis</span> <span class="o">=</span> <span class="s1">&#39;y&#39;</span><span class="p">,</span> <span class="n">b</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">which</span><span class="o">=</span><span class="s1">&#39;major&#39;</span><span class="p">,</span> <span class="n">color</span><span class="o">=</span><span class="s1">&#39;#999999&#39;</span><span class="p">,</span> <span class="n">linestyle</span><span class="o">=</span><span class="s1">&#39;-&#39;</span><span class="p">,</span> <span class="n">alpha</span><span class="o">=</span><span class="mf">0.15</span><span class="p">,</span><span class="n">zorder</span><span class="o">=-</span><span class="mi">1</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">subplots_adjust</span><span class="p">(</span><span class="n">left</span><span class="o">=</span><span class="mf">0.2</span><span class="p">,</span> <span class="n">right</span><span class="o">=</span><span class="mf">0.9</span><span class="p">,</span> <span class="n">top</span><span class="o">=</span><span class="mf">0.9</span><span class="p">,</span> <span class="n">bottom</span><span class="o">=</span><span class="mf">0.25</span><span class="p">)</span>
<span class="n">fig</span><span class="o">.</span><span class="n">text</span><span class="p">(</span><span class="mf">0.91</span><span class="p">,</span> <span class="mf">0.02</span><span class="p">,</span> <span class="s2">&quot;Datenstand: &quot;</span> <span class="o">+</span> <span class="n">today</span> <span class="o">+</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">Datenquelle:RKI Nowcast</span><span class="se">\n</span><span class="s2">Viz: @CorneliusRoemer&quot;</span><span class="p">,</span> <span class="n">size</span><span class="o">=</span><span class="mi">5</span><span class="p">,</span> <span class="n">va</span><span class="o">=</span><span class="s2">&quot;bottom&quot;</span><span class="p">,</span> <span class="n">ha</span><span class="o">=</span><span class="s2">&quot;right&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">savefig</span><span class="p">(</span><span class="s1">&#39;CasesNear.png&#39;</span><span class="p">,</span><span class="n">dpi</span><span class="o">=</span><span class="mi">300</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt"></div>



<div class="output_svg output_subarea ">
<?xml version="1.0" encoding="utf-8" standalone="no"?>
<!DOCTYPE svg PUBLIC "-//W3C//DTD SVG 1.1//EN"
  "http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd">
<!-- Created with matplotlib (https://matplotlib.org/) -->
<svg height="251.278125pt" version="1.1" viewBox="0 0 405.588125 251.278125" width="405.588125pt" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
 <defs>
  <style type="text/css">
*{stroke-linecap:butt;stroke-linejoin:round;}
  </style>
 </defs>
 <g id="figure_1">
  <g id="patch_1">
   <path d="M 0 251.278125 
L 405.588125 251.278125 
L 405.588125 0 
L 0 0 
z
" style="fill:#ffffff;"/>
  </g>
  <g id="axes_1">
   <g id="patch_2">
    <path d="M 53.328125 186.118125 
L 393.528125 186.118125 
L 393.528125 22.318125 
L 53.328125 22.318125 
z
" style="fill:#ffffff;"/>
   </g>
   <g id="PolyCollection_1">
    <defs>
     <path d="M 53.328125 -209.407525 
L 53.328125 -199.948671 
L 56.764489 -192.798522 
L 60.200852 -202.233837 
L 63.637216 -184.592032 
L 67.07358 -182.491611 
L 70.509943 -176.521939 
L 73.946307 -170.949442 
L 77.38267 -158.30915 
L 80.819034 -149.306126 
L 84.255398 -165.887662 
L 87.691761 -149.807049 
L 91.128125 -150.832618 
L 94.564489 -157.449607 
L 98.000852 -150.187028 
L 101.437216 -144.943378 
L 104.87358 -137.850087 
L 108.309943 -140.179392 
L 111.746307 -134.945353 
L 115.18267 -132.465569 
L 118.619034 -132.233168 
L 122.055398 -127.348373 
L 125.491761 -126.128483 
L 128.928125 -121.730528 
L 132.364489 -119.568451 
L 135.800852 -135.053047 
L 139.237216 -129.203001 
L 142.67358 -117.640914 
L 146.109943 -123.492496 
L 149.546307 -110.912066 
L 152.98267 -119.905672 
L 156.419034 -105.827824 
L 159.855398 -103.929641 
L 163.291761 -105.519174 
L 166.728125 -109.96078 
L 170.164489 -108.761069 
L 173.600852 -107.005148 
L 177.037216 -108.753776 
L 180.47358 -104.719709 
L 183.909943 -100.16037 
L 187.346307 -97.906516 
L 190.78267 -96.77655 
L 194.219034 -95.216066 
L 197.655398 -107.107962 
L 201.091761 -103.076447 
L 204.528125 -100.730494 
L 207.964489 -96.606486 
L 211.400852 -98.148187 
L 214.837216 -92.424475 
L 218.27358 -103.521031 
L 221.709943 -108.547352 
L 225.146307 -106.219254 
L 228.58267 -103.611594 
L 232.019034 -102.206546 
L 235.455398 -106.606697 
L 238.891761 -108.424753 
L 242.328125 -126.161949 
L 245.764489 -175.787467 
L 249.200852 -128.827189 
L 252.637216 -121.452247 
L 256.07358 -123.745235 
L 259.509943 -118.931954 
L 262.946307 -109.96078 
L 266.38267 -109.848624 
L 269.819034 -105.977012 
L 273.255398 -109.564823 
L 276.691761 -107.268373 
L 280.128125 -108.452766 
L 283.564489 -105.035831 
L 287.000852 -102.920657 
L 290.437216 -104.905192 
L 293.87358 -108.033284 
L 297.309943 -102.569543 
L 300.746307 -100.619683 
L 304.18267 -99.83729 
L 307.619034 -98.389859 
L 311.055398 -100.488615 
L 314.491761 -97.885519 
L 317.928125 -98.677244 
L 321.364489 -96.48669 
L 324.800852 -104.387274 
L 328.237216 -109.85278 
L 331.67358 -108.902578 
L 335.109943 -108.040747 
L 338.546307 -115.18753 
L 341.98267 -115.024611 
L 345.419034 -117.675293 
L 348.855398 -113.252195 
L 352.291761 -115.991307 
L 355.728125 -117.481923 
L 359.164489 -124.553034 
L 362.600852 -118.549064 
L 366.037216 -128.596011 
L 369.47358 -129.131332 
L 372.909943 -128.876618 
L 376.346307 -124.822169 
L 379.78267 -118.931954 
L 383.219034 -132.233168 
L 386.655398 -127.447241 
L 390.091761 -112.351457 
L 390.091761 -192.648903 
L 390.091761 -192.648903 
L 386.655398 -202.884011 
L 383.219034 -179.46599 
L 379.78267 -161.103666 
L 376.346307 -157.237897 
L 372.909943 -152.590281 
L 369.47358 -150.218554 
L 366.037216 -147.410905 
L 362.600852 -136.345419 
L 359.164489 -137.097252 
L 355.728125 -127.027956 
L 352.291761 -126.545265 
L 348.855398 -121.895493 
L 345.419034 -124.366431 
L 341.98267 -123.352515 
L 338.546307 -121.811729 
L 335.109943 -116.104887 
L 331.67358 -116.152729 
L 328.237216 -115.129759 
L 324.800852 -110.038661 
L 321.364489 -101.758496 
L 317.928125 -104.22918 
L 314.491761 -103.323294 
L 311.055398 -106.376718 
L 307.619034 -103.948308 
L 304.18267 -105.221962 
L 300.746307 -106.160258 
L 297.309943 -108.246872 
L 293.87358 -113.790848 
L 290.437216 -109.848624 
L 287.000852 -109.192767 
L 283.564489 -110.956788 
L 280.128125 -114.914372 
L 276.691761 -113.030572 
L 273.255398 -115.03939 
L 269.819034 -112.14583 
L 266.38267 -115.681874 
L 262.946307 -116.360891 
L 259.509943 -126.061269 
L 256.07358 -130.099148 
L 252.637216 -128.987429 
L 249.200852 -136.025232 
L 245.764489 -183.909744 
L 242.328125 -132.58841 
L 238.891761 -114.312856 
L 235.455398 -112.527654 
L 232.019034 -107.591218 
L 228.58267 -109.484604 
L 225.146307 -111.389679 
L 221.709943 -113.996475 
L 218.27358 -108.167857 
L 214.837216 -97.800568 
L 211.400852 -103.827472 
L 207.964489 -101.452692 
L 204.528125 -106.049447 
L 201.091761 -107.739967 
L 197.655398 -113.688034 
L 194.219034 -100.258366 
L 190.78267 -102.152644 
L 187.346307 -103.464965 
L 183.909943 -105.975816 
L 180.47358 -110.481907 
L 177.037216 -113.82282 
L 173.600852 -112.659898 
L 170.164489 -113.407895 
L 166.728125 -115.976885 
L 163.291761 -112.165146 
L 159.855398 -109.5297 
L 156.419034 -111.479211 
L 152.98267 -125.076097 
L 149.546307 -116.361188 
L 146.109943 -129.424614 
L 142.67358 -126.217063 
L 139.237216 -135.848973 
L 135.800852 -141.945427 
L 132.364489 -126.660388 
L 128.928125 -128.016142 
L 125.491761 -132.502929 
L 122.055398 -133.972571 
L 118.619034 -140.169306 
L 115.18267 -139.594884 
L 111.746307 -141.622347 
L 108.309943 -147.271328 
L 104.87358 -145.048129 
L 101.437216 -153.579723 
L 98.000852 -158.491993 
L 94.564489 -166.28176 
L 91.128125 -159.653635 
L 87.691761 -157.34559 
L 84.255398 -173.422844 
L 80.819034 -156.504168 
L 77.38267 -166.328613 
L 73.946307 -178.562327 
L 70.509943 -185.610097 
L 67.07358 -191.433464 
L 63.637216 -192.884428 
L 60.200852 -211.763626 
L 56.764489 -201.720039 
L 53.328125 -209.407525 
z
" id="m83bc5d3784"/>
    </defs>
    <g clip-path="url(#p9afea4b7e9)">
     <use style="fill:#008000;fill-opacity:0.3;" x="0" xlink:href="#m83bc5d3784" y="251.278125"/>
    </g>
   </g>
   <g id="matplotlib.axis_1">
    <g id="xtick_1">
     <g id="line2d_1">
      <defs>
       <path d="M 0 0 
L 0 3.5 
" id="macf79c3104" style="stroke:#000000;stroke-width:0.8;"/>
      </defs>
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="53.328125" xlink:href="#macf79c3104" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_2">
     <g id="line2d_2">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="87.691761" xlink:href="#macf79c3104" y="186.118125"/>
      </g>
     </g>
     <g id="text_1">
      <!-- Mai -->
      <defs>
       <path d="M 9.8125 72.90625 
L 24.515625 72.90625 
L 43.109375 23.296875 
L 61.8125 72.90625 
L 76.515625 72.90625 
L 76.515625 0 
L 66.890625 0 
L 66.890625 64.015625 
L 48.09375 14.015625 
L 38.1875 14.015625 
L 19.390625 64.015625 
L 19.390625 0 
L 9.8125 0 
z
" id="DejaVuSans-77"/>
       <path d="M 34.28125 27.484375 
Q 23.390625 27.484375 19.1875 25 
Q 14.984375 22.515625 14.984375 16.5 
Q 14.984375 11.71875 18.140625 8.90625 
Q 21.296875 6.109375 26.703125 6.109375 
Q 34.1875 6.109375 38.703125 11.40625 
Q 43.21875 16.703125 43.21875 25.484375 
L 43.21875 27.484375 
z
M 52.203125 31.203125 
L 52.203125 0 
L 43.21875 0 
L 43.21875 8.296875 
Q 40.140625 3.328125 35.546875 0.953125 
Q 30.953125 -1.421875 24.3125 -1.421875 
Q 15.921875 -1.421875 10.953125 3.296875 
Q 6 8.015625 6 15.921875 
Q 6 25.140625 12.171875 29.828125 
Q 18.359375 34.515625 30.609375 34.515625 
L 43.21875 34.515625 
L 43.21875 35.40625 
Q 43.21875 41.609375 39.140625 45 
Q 35.0625 48.390625 27.6875 48.390625 
Q 23 48.390625 18.546875 47.265625 
Q 14.109375 46.140625 10.015625 43.890625 
L 10.015625 52.203125 
Q 14.9375 54.109375 19.578125 55.046875 
Q 24.21875 56 28.609375 56 
Q 40.484375 56 46.34375 49.84375 
Q 52.203125 43.703125 52.203125 31.203125 
z
" id="DejaVuSans-97"/>
       <path d="M 9.421875 54.6875 
L 18.40625 54.6875 
L 18.40625 0 
L 9.421875 0 
z
M 9.421875 75.984375 
L 18.40625 75.984375 
L 18.40625 64.59375 
L 9.421875 64.59375 
z
" id="DejaVuSans-105"/>
      </defs>
      <g transform="translate(78.924574 202.216563)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-77"/>
       <use x="86.279297" xlink:href="#DejaVuSans-97"/>
       <use x="147.558594" xlink:href="#DejaVuSans-105"/>
      </g>
      <!-- 2020 -->
      <defs>
       <path d="M 19.1875 8.296875 
L 53.609375 8.296875 
L 53.609375 0 
L 7.328125 0 
L 7.328125 8.296875 
Q 12.9375 14.109375 22.625 23.890625 
Q 32.328125 33.6875 34.8125 36.53125 
Q 39.546875 41.84375 41.421875 45.53125 
Q 43.3125 49.21875 43.3125 52.78125 
Q 43.3125 58.59375 39.234375 62.25 
Q 35.15625 65.921875 28.609375 65.921875 
Q 23.96875 65.921875 18.8125 64.3125 
Q 13.671875 62.703125 7.8125 59.421875 
L 7.8125 69.390625 
Q 13.765625 71.78125 18.9375 73 
Q 24.125 74.21875 28.421875 74.21875 
Q 39.75 74.21875 46.484375 68.546875 
Q 53.21875 62.890625 53.21875 53.421875 
Q 53.21875 48.921875 51.53125 44.890625 
Q 49.859375 40.875 45.40625 35.40625 
Q 44.1875 33.984375 37.640625 27.21875 
Q 31.109375 20.453125 19.1875 8.296875 
z
" id="DejaVuSans-50"/>
       <path d="M 31.78125 66.40625 
Q 24.171875 66.40625 20.328125 58.90625 
Q 16.5 51.421875 16.5 36.375 
Q 16.5 21.390625 20.328125 13.890625 
Q 24.171875 6.390625 31.78125 6.390625 
Q 39.453125 6.390625 43.28125 13.890625 
Q 47.125 21.390625 47.125 36.375 
Q 47.125 51.421875 43.28125 58.90625 
Q 39.453125 66.40625 31.78125 66.40625 
z
M 31.78125 74.21875 
Q 44.046875 74.21875 50.515625 64.515625 
Q 56.984375 54.828125 56.984375 36.375 
Q 56.984375 17.96875 50.515625 8.265625 
Q 44.046875 -1.421875 31.78125 -1.421875 
Q 19.53125 -1.421875 13.0625 8.265625 
Q 6.59375 17.96875 6.59375 36.375 
Q 6.59375 54.828125 13.0625 64.515625 
Q 19.53125 74.21875 31.78125 74.21875 
z
" id="DejaVuSans-48"/>
      </defs>
      <g transform="translate(74.966761 213.414375)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
      </g>
     </g>
    </g>
    <g id="xtick_3">
     <g id="line2d_3">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="194.219034" xlink:href="#macf79c3104" y="186.118125"/>
      </g>
     </g>
     <g id="text_2">
      <!-- Jun -->
      <defs>
       <path d="M 9.8125 72.90625 
L 19.671875 72.90625 
L 19.671875 5.078125 
Q 19.671875 -8.109375 14.671875 -14.0625 
Q 9.671875 -20.015625 -1.421875 -20.015625 
L -5.171875 -20.015625 
L -5.171875 -11.71875 
L -2.09375 -11.71875 
Q 4.4375 -11.71875 7.125 -8.046875 
Q 9.8125 -4.390625 9.8125 5.078125 
z
" id="DejaVuSans-74"/>
       <path d="M 8.5 21.578125 
L 8.5 54.6875 
L 17.484375 54.6875 
L 17.484375 21.921875 
Q 17.484375 14.15625 20.5 10.265625 
Q 23.53125 6.390625 29.59375 6.390625 
Q 36.859375 6.390625 41.078125 11.03125 
Q 45.3125 15.671875 45.3125 23.6875 
L 45.3125 54.6875 
L 54.296875 54.6875 
L 54.296875 0 
L 45.3125 0 
L 45.3125 8.40625 
Q 42.046875 3.421875 37.71875 1 
Q 33.40625 -1.421875 27.6875 -1.421875 
Q 18.265625 -1.421875 13.375 4.4375 
Q 8.5 10.296875 8.5 21.578125 
z
M 31.109375 56 
z
" id="DejaVuSans-117"/>
       <path d="M 54.890625 33.015625 
L 54.890625 0 
L 45.90625 0 
L 45.90625 32.71875 
Q 45.90625 40.484375 42.875 44.328125 
Q 39.84375 48.1875 33.796875 48.1875 
Q 26.515625 48.1875 22.3125 43.546875 
Q 18.109375 38.921875 18.109375 30.90625 
L 18.109375 0 
L 9.078125 0 
L 9.078125 54.6875 
L 18.109375 54.6875 
L 18.109375 46.1875 
Q 21.34375 51.125 25.703125 53.5625 
Q 30.078125 56 35.796875 56 
Q 45.21875 56 50.046875 50.171875 
Q 54.890625 44.34375 54.890625 33.015625 
z
" id="DejaVuSans-110"/>
      </defs>
      <g transform="translate(186.406534 202.216563)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-74"/>
       <use x="29.492188" xlink:href="#DejaVuSans-117"/>
       <use x="92.871094" xlink:href="#DejaVuSans-110"/>
      </g>
     </g>
    </g>
    <g id="xtick_4">
     <g id="line2d_4">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="297.309943" xlink:href="#macf79c3104" y="186.118125"/>
      </g>
     </g>
     <g id="text_3">
      <!-- Jul -->
      <defs>
       <path d="M 9.421875 75.984375 
L 18.40625 75.984375 
L 18.40625 0 
L 9.421875 0 
z
" id="DejaVuSans-108"/>
      </defs>
      <g transform="translate(291.277131 202.216563)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-74"/>
       <use x="29.492188" xlink:href="#DejaVuSans-117"/>
       <use x="92.871094" xlink:href="#DejaVuSans-108"/>
      </g>
     </g>
    </g>
    <g id="xtick_5">
     <g id="line2d_5">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="393.528125" xlink:href="#macf79c3104" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_6">
     <g id="line2d_6">
      <defs>
       <path d="M 0 0 
L 0 2 
" id="m9e03397c56" style="stroke:#000000;stroke-width:0.6;"/>
      </defs>
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="73.946307" xlink:href="#m9e03397c56" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_7">
     <g id="line2d_7">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="98.000852" xlink:href="#m9e03397c56" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_8">
     <g id="line2d_8">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="122.055398" xlink:href="#m9e03397c56" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_9">
     <g id="line2d_9">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="146.109943" xlink:href="#m9e03397c56" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_10">
     <g id="line2d_10">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="170.164489" xlink:href="#m9e03397c56" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_11">
     <g id="line2d_11">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="218.27358" xlink:href="#m9e03397c56" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_12">
     <g id="line2d_12">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="242.328125" xlink:href="#m9e03397c56" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_13">
     <g id="line2d_13">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="266.38267" xlink:href="#m9e03397c56" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_14">
     <g id="line2d_14">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="290.437216" xlink:href="#m9e03397c56" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_15">
     <g id="line2d_15">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="314.491761" xlink:href="#m9e03397c56" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_16">
     <g id="line2d_16">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="338.546307" xlink:href="#m9e03397c56" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_17">
     <g id="line2d_17">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="362.600852" xlink:href="#m9e03397c56" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_18">
     <g id="line2d_18">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="386.655398" xlink:href="#m9e03397c56" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="text_4">
     <!-- Datum des Erkrankungsbeginns -->
     <defs>
      <path d="M 19.671875 64.796875 
L 19.671875 8.109375 
L 31.59375 8.109375 
Q 46.6875 8.109375 53.6875 14.9375 
Q 60.6875 21.78125 60.6875 36.53125 
Q 60.6875 51.171875 53.6875 57.984375 
Q 46.6875 64.796875 31.59375 64.796875 
z
M 9.8125 72.90625 
L 30.078125 72.90625 
Q 51.265625 72.90625 61.171875 64.09375 
Q 71.09375 55.28125 71.09375 36.53125 
Q 71.09375 17.671875 61.125 8.828125 
Q 51.171875 0 30.078125 0 
L 9.8125 0 
z
" id="DejaVuSans-68"/>
      <path d="M 18.3125 70.21875 
L 18.3125 54.6875 
L 36.8125 54.6875 
L 36.8125 47.703125 
L 18.3125 47.703125 
L 18.3125 18.015625 
Q 18.3125 11.328125 20.140625 9.421875 
Q 21.96875 7.515625 27.59375 7.515625 
L 36.8125 7.515625 
L 36.8125 0 
L 27.59375 0 
Q 17.1875 0 13.234375 3.875 
Q 9.28125 7.765625 9.28125 18.015625 
L 9.28125 47.703125 
L 2.6875 47.703125 
L 2.6875 54.6875 
L 9.28125 54.6875 
L 9.28125 70.21875 
z
" id="DejaVuSans-116"/>
      <path d="M 52 44.1875 
Q 55.375 50.25 60.0625 53.125 
Q 64.75 56 71.09375 56 
Q 79.640625 56 84.28125 50.015625 
Q 88.921875 44.046875 88.921875 33.015625 
L 88.921875 0 
L 79.890625 0 
L 79.890625 32.71875 
Q 79.890625 40.578125 77.09375 44.375 
Q 74.3125 48.1875 68.609375 48.1875 
Q 61.625 48.1875 57.5625 43.546875 
Q 53.515625 38.921875 53.515625 30.90625 
L 53.515625 0 
L 44.484375 0 
L 44.484375 32.71875 
Q 44.484375 40.625 41.703125 44.40625 
Q 38.921875 48.1875 33.109375 48.1875 
Q 26.21875 48.1875 22.15625 43.53125 
Q 18.109375 38.875 18.109375 30.90625 
L 18.109375 0 
L 9.078125 0 
L 9.078125 54.6875 
L 18.109375 54.6875 
L 18.109375 46.1875 
Q 21.1875 51.21875 25.484375 53.609375 
Q 29.78125 56 35.6875 56 
Q 41.65625 56 45.828125 52.96875 
Q 50 49.953125 52 44.1875 
z
" id="DejaVuSans-109"/>
      <path id="DejaVuSans-32"/>
      <path d="M 45.40625 46.390625 
L 45.40625 75.984375 
L 54.390625 75.984375 
L 54.390625 0 
L 45.40625 0 
L 45.40625 8.203125 
Q 42.578125 3.328125 38.25 0.953125 
Q 33.9375 -1.421875 27.875 -1.421875 
Q 17.96875 -1.421875 11.734375 6.484375 
Q 5.515625 14.40625 5.515625 27.296875 
Q 5.515625 40.1875 11.734375 48.09375 
Q 17.96875 56 27.875 56 
Q 33.9375 56 38.25 53.625 
Q 42.578125 51.265625 45.40625 46.390625 
z
M 14.796875 27.296875 
Q 14.796875 17.390625 18.875 11.75 
Q 22.953125 6.109375 30.078125 6.109375 
Q 37.203125 6.109375 41.296875 11.75 
Q 45.40625 17.390625 45.40625 27.296875 
Q 45.40625 37.203125 41.296875 42.84375 
Q 37.203125 48.484375 30.078125 48.484375 
Q 22.953125 48.484375 18.875 42.84375 
Q 14.796875 37.203125 14.796875 27.296875 
z
" id="DejaVuSans-100"/>
      <path d="M 56.203125 29.59375 
L 56.203125 25.203125 
L 14.890625 25.203125 
Q 15.484375 15.921875 20.484375 11.0625 
Q 25.484375 6.203125 34.421875 6.203125 
Q 39.59375 6.203125 44.453125 7.46875 
Q 49.3125 8.734375 54.109375 11.28125 
L 54.109375 2.78125 
Q 49.265625 0.734375 44.1875 -0.34375 
Q 39.109375 -1.421875 33.890625 -1.421875 
Q 20.796875 -1.421875 13.15625 6.1875 
Q 5.515625 13.8125 5.515625 26.8125 
Q 5.515625 40.234375 12.765625 48.109375 
Q 20.015625 56 32.328125 56 
Q 43.359375 56 49.78125 48.890625 
Q 56.203125 41.796875 56.203125 29.59375 
z
M 47.21875 32.234375 
Q 47.125 39.59375 43.09375 43.984375 
Q 39.0625 48.390625 32.421875 48.390625 
Q 24.90625 48.390625 20.390625 44.140625 
Q 15.875 39.890625 15.1875 32.171875 
z
" id="DejaVuSans-101"/>
      <path d="M 44.28125 53.078125 
L 44.28125 44.578125 
Q 40.484375 46.53125 36.375 47.5 
Q 32.28125 48.484375 27.875 48.484375 
Q 21.1875 48.484375 17.84375 46.4375 
Q 14.5 44.390625 14.5 40.28125 
Q 14.5 37.15625 16.890625 35.375 
Q 19.28125 33.59375 26.515625 31.984375 
L 29.59375 31.296875 
Q 39.15625 29.25 43.1875 25.515625 
Q 47.21875 21.78125 47.21875 15.09375 
Q 47.21875 7.46875 41.1875 3.015625 
Q 35.15625 -1.421875 24.609375 -1.421875 
Q 20.21875 -1.421875 15.453125 -0.5625 
Q 10.6875 0.296875 5.421875 2 
L 5.421875 11.28125 
Q 10.40625 8.6875 15.234375 7.390625 
Q 20.0625 6.109375 24.8125 6.109375 
Q 31.15625 6.109375 34.5625 8.28125 
Q 37.984375 10.453125 37.984375 14.40625 
Q 37.984375 18.0625 35.515625 20.015625 
Q 33.0625 21.96875 24.703125 23.78125 
L 21.578125 24.515625 
Q 13.234375 26.265625 9.515625 29.90625 
Q 5.8125 33.546875 5.8125 39.890625 
Q 5.8125 47.609375 11.28125 51.796875 
Q 16.75 56 26.8125 56 
Q 31.78125 56 36.171875 55.265625 
Q 40.578125 54.546875 44.28125 53.078125 
z
" id="DejaVuSans-115"/>
      <path d="M 9.8125 72.90625 
L 55.90625 72.90625 
L 55.90625 64.59375 
L 19.671875 64.59375 
L 19.671875 43.015625 
L 54.390625 43.015625 
L 54.390625 34.71875 
L 19.671875 34.71875 
L 19.671875 8.296875 
L 56.78125 8.296875 
L 56.78125 0 
L 9.8125 0 
z
" id="DejaVuSans-69"/>
      <path d="M 41.109375 46.296875 
Q 39.59375 47.171875 37.8125 47.578125 
Q 36.03125 48 33.890625 48 
Q 26.265625 48 22.1875 43.046875 
Q 18.109375 38.09375 18.109375 28.8125 
L 18.109375 0 
L 9.078125 0 
L 9.078125 54.6875 
L 18.109375 54.6875 
L 18.109375 46.1875 
Q 20.953125 51.171875 25.484375 53.578125 
Q 30.03125 56 36.53125 56 
Q 37.453125 56 38.578125 55.875 
Q 39.703125 55.765625 41.0625 55.515625 
z
" id="DejaVuSans-114"/>
      <path d="M 9.078125 75.984375 
L 18.109375 75.984375 
L 18.109375 31.109375 
L 44.921875 54.6875 
L 56.390625 54.6875 
L 27.390625 29.109375 
L 57.625 0 
L 45.90625 0 
L 18.109375 26.703125 
L 18.109375 0 
L 9.078125 0 
z
" id="DejaVuSans-107"/>
      <path d="M 45.40625 27.984375 
Q 45.40625 37.75 41.375 43.109375 
Q 37.359375 48.484375 30.078125 48.484375 
Q 22.859375 48.484375 18.828125 43.109375 
Q 14.796875 37.75 14.796875 27.984375 
Q 14.796875 18.265625 18.828125 12.890625 
Q 22.859375 7.515625 30.078125 7.515625 
Q 37.359375 7.515625 41.375 12.890625 
Q 45.40625 18.265625 45.40625 27.984375 
z
M 54.390625 6.78125 
Q 54.390625 -7.171875 48.1875 -13.984375 
Q 42 -20.796875 29.203125 -20.796875 
Q 24.46875 -20.796875 20.265625 -20.09375 
Q 16.0625 -19.390625 12.109375 -17.921875 
L 12.109375 -9.1875 
Q 16.0625 -11.328125 19.921875 -12.34375 
Q 23.78125 -13.375 27.78125 -13.375 
Q 36.625 -13.375 41.015625 -8.765625 
Q 45.40625 -4.15625 45.40625 5.171875 
L 45.40625 9.625 
Q 42.625 4.78125 38.28125 2.390625 
Q 33.9375 0 27.875 0 
Q 17.828125 0 11.671875 7.65625 
Q 5.515625 15.328125 5.515625 27.984375 
Q 5.515625 40.671875 11.671875 48.328125 
Q 17.828125 56 27.875 56 
Q 33.9375 56 38.28125 53.609375 
Q 42.625 51.21875 45.40625 46.390625 
L 45.40625 54.6875 
L 54.390625 54.6875 
z
" id="DejaVuSans-103"/>
      <path d="M 48.6875 27.296875 
Q 48.6875 37.203125 44.609375 42.84375 
Q 40.53125 48.484375 33.40625 48.484375 
Q 26.265625 48.484375 22.1875 42.84375 
Q 18.109375 37.203125 18.109375 27.296875 
Q 18.109375 17.390625 22.1875 11.75 
Q 26.265625 6.109375 33.40625 6.109375 
Q 40.53125 6.109375 44.609375 11.75 
Q 48.6875 17.390625 48.6875 27.296875 
z
M 18.109375 46.390625 
Q 20.953125 51.265625 25.265625 53.625 
Q 29.59375 56 35.59375 56 
Q 45.5625 56 51.78125 48.09375 
Q 58.015625 40.1875 58.015625 27.296875 
Q 58.015625 14.40625 51.78125 6.484375 
Q 45.5625 -1.421875 35.59375 -1.421875 
Q 29.59375 -1.421875 25.265625 0.953125 
Q 20.953125 3.328125 18.109375 8.203125 
L 18.109375 0 
L 9.078125 0 
L 9.078125 75.984375 
L 18.109375 75.984375 
z
" id="DejaVuSans-98"/>
     </defs>
     <g transform="translate(143.317188 227.0925)scale(0.1 -0.1)">
      <use xlink:href="#DejaVuSans-68"/>
      <use x="77.001953" xlink:href="#DejaVuSans-97"/>
      <use x="138.28125" xlink:href="#DejaVuSans-116"/>
      <use x="177.490234" xlink:href="#DejaVuSans-117"/>
      <use x="240.869141" xlink:href="#DejaVuSans-109"/>
      <use x="338.28125" xlink:href="#DejaVuSans-32"/>
      <use x="370.068359" xlink:href="#DejaVuSans-100"/>
      <use x="433.544922" xlink:href="#DejaVuSans-101"/>
      <use x="495.068359" xlink:href="#DejaVuSans-115"/>
      <use x="547.167969" xlink:href="#DejaVuSans-32"/>
      <use x="578.955078" xlink:href="#DejaVuSans-69"/>
      <use x="642.138672" xlink:href="#DejaVuSans-114"/>
      <use x="683.251953" xlink:href="#DejaVuSans-107"/>
      <use x="741.162109" xlink:href="#DejaVuSans-114"/>
      <use x="782.275391" xlink:href="#DejaVuSans-97"/>
      <use x="843.554688" xlink:href="#DejaVuSans-110"/>
      <use x="906.933594" xlink:href="#DejaVuSans-107"/>
      <use x="964.796875" xlink:href="#DejaVuSans-117"/>
      <use x="1028.175781" xlink:href="#DejaVuSans-110"/>
      <use x="1091.554688" xlink:href="#DejaVuSans-103"/>
      <use x="1155.03125" xlink:href="#DejaVuSans-115"/>
      <use x="1207.130859" xlink:href="#DejaVuSans-98"/>
      <use x="1270.607422" xlink:href="#DejaVuSans-101"/>
      <use x="1332.130859" xlink:href="#DejaVuSans-103"/>
      <use x="1395.607422" xlink:href="#DejaVuSans-105"/>
      <use x="1423.390625" xlink:href="#DejaVuSans-110"/>
      <use x="1486.769531" xlink:href="#DejaVuSans-110"/>
      <use x="1550.148438" xlink:href="#DejaVuSans-115"/>
     </g>
    </g>
   </g>
   <g id="matplotlib.axis_2">
    <g id="ytick_1">
     <g id="line2d_19">
      <path clip-path="url(#p9afea4b7e9)" d="M 53.328125 186.118125 
L 393.528125 186.118125 
" style="fill:none;stroke:#999999;stroke-linecap:square;stroke-opacity:0.15;stroke-width:0.8;"/>
     </g>
     <g id="line2d_20">
      <defs>
       <path d="M 0 0 
L -3.5 0 
" id="m004a693e37" style="stroke:#000000;stroke-width:0.8;"/>
      </defs>
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="53.328125" xlink:href="#m004a693e37" y="186.118125"/>
      </g>
     </g>
     <g id="text_5">
      <!-- 0 -->
      <g transform="translate(39.965625 189.917344)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-48"/>
      </g>
     </g>
    </g>
    <g id="ytick_2">
     <g id="line2d_21">
      <path clip-path="url(#p9afea4b7e9)" d="M 53.328125 164.278125 
L 393.528125 164.278125 
" style="fill:none;stroke:#999999;stroke-linecap:square;stroke-opacity:0.15;stroke-width:0.8;"/>
     </g>
     <g id="line2d_22">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="53.328125" xlink:href="#m004a693e37" y="164.278125"/>
      </g>
     </g>
     <g id="text_6">
      <!-- 200 -->
      <g transform="translate(27.240625 168.077344)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-48"/>
      </g>
     </g>
    </g>
    <g id="ytick_3">
     <g id="line2d_23">
      <path clip-path="url(#p9afea4b7e9)" d="M 53.328125 142.438125 
L 393.528125 142.438125 
" style="fill:none;stroke:#999999;stroke-linecap:square;stroke-opacity:0.15;stroke-width:0.8;"/>
     </g>
     <g id="line2d_24">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="53.328125" xlink:href="#m004a693e37" y="142.438125"/>
      </g>
     </g>
     <g id="text_7">
      <!-- 400 -->
      <defs>
       <path d="M 37.796875 64.3125 
L 12.890625 25.390625 
L 37.796875 25.390625 
z
M 35.203125 72.90625 
L 47.609375 72.90625 
L 47.609375 25.390625 
L 58.015625 25.390625 
L 58.015625 17.1875 
L 47.609375 17.1875 
L 47.609375 0 
L 37.796875 0 
L 37.796875 17.1875 
L 4.890625 17.1875 
L 4.890625 26.703125 
z
" id="DejaVuSans-52"/>
      </defs>
      <g transform="translate(27.240625 146.237344)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-52"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-48"/>
      </g>
     </g>
    </g>
    <g id="ytick_4">
     <g id="line2d_25">
      <path clip-path="url(#p9afea4b7e9)" d="M 53.328125 120.598125 
L 393.528125 120.598125 
" style="fill:none;stroke:#999999;stroke-linecap:square;stroke-opacity:0.15;stroke-width:0.8;"/>
     </g>
     <g id="line2d_26">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="53.328125" xlink:href="#m004a693e37" y="120.598125"/>
      </g>
     </g>
     <g id="text_8">
      <!-- 600 -->
      <defs>
       <path d="M 33.015625 40.375 
Q 26.375 40.375 22.484375 35.828125 
Q 18.609375 31.296875 18.609375 23.390625 
Q 18.609375 15.53125 22.484375 10.953125 
Q 26.375 6.390625 33.015625 6.390625 
Q 39.65625 6.390625 43.53125 10.953125 
Q 47.40625 15.53125 47.40625 23.390625 
Q 47.40625 31.296875 43.53125 35.828125 
Q 39.65625 40.375 33.015625 40.375 
z
M 52.59375 71.296875 
L 52.59375 62.3125 
Q 48.875 64.0625 45.09375 64.984375 
Q 41.3125 65.921875 37.59375 65.921875 
Q 27.828125 65.921875 22.671875 59.328125 
Q 17.53125 52.734375 16.796875 39.40625 
Q 19.671875 43.65625 24.015625 45.921875 
Q 28.375 48.1875 33.59375 48.1875 
Q 44.578125 48.1875 50.953125 41.515625 
Q 57.328125 34.859375 57.328125 23.390625 
Q 57.328125 12.15625 50.6875 5.359375 
Q 44.046875 -1.421875 33.015625 -1.421875 
Q 20.359375 -1.421875 13.671875 8.265625 
Q 6.984375 17.96875 6.984375 36.375 
Q 6.984375 53.65625 15.1875 63.9375 
Q 23.390625 74.21875 37.203125 74.21875 
Q 40.921875 74.21875 44.703125 73.484375 
Q 48.484375 72.75 52.59375 71.296875 
z
" id="DejaVuSans-54"/>
      </defs>
      <g transform="translate(27.240625 124.397344)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-54"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-48"/>
      </g>
     </g>
    </g>
    <g id="ytick_5">
     <g id="line2d_27">
      <path clip-path="url(#p9afea4b7e9)" d="M 53.328125 98.758125 
L 393.528125 98.758125 
" style="fill:none;stroke:#999999;stroke-linecap:square;stroke-opacity:0.15;stroke-width:0.8;"/>
     </g>
     <g id="line2d_28">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="53.328125" xlink:href="#m004a693e37" y="98.758125"/>
      </g>
     </g>
     <g id="text_9">
      <!-- 800 -->
      <defs>
       <path d="M 31.78125 34.625 
Q 24.75 34.625 20.71875 30.859375 
Q 16.703125 27.09375 16.703125 20.515625 
Q 16.703125 13.921875 20.71875 10.15625 
Q 24.75 6.390625 31.78125 6.390625 
Q 38.8125 6.390625 42.859375 10.171875 
Q 46.921875 13.96875 46.921875 20.515625 
Q 46.921875 27.09375 42.890625 30.859375 
Q 38.875 34.625 31.78125 34.625 
z
M 21.921875 38.8125 
Q 15.578125 40.375 12.03125 44.71875 
Q 8.5 49.078125 8.5 55.328125 
Q 8.5 64.0625 14.71875 69.140625 
Q 20.953125 74.21875 31.78125 74.21875 
Q 42.671875 74.21875 48.875 69.140625 
Q 55.078125 64.0625 55.078125 55.328125 
Q 55.078125 49.078125 51.53125 44.71875 
Q 48 40.375 41.703125 38.8125 
Q 48.828125 37.15625 52.796875 32.3125 
Q 56.78125 27.484375 56.78125 20.515625 
Q 56.78125 9.90625 50.3125 4.234375 
Q 43.84375 -1.421875 31.78125 -1.421875 
Q 19.734375 -1.421875 13.25 4.234375 
Q 6.78125 9.90625 6.78125 20.515625 
Q 6.78125 27.484375 10.78125 32.3125 
Q 14.796875 37.15625 21.921875 38.8125 
z
M 18.3125 54.390625 
Q 18.3125 48.734375 21.84375 45.5625 
Q 25.390625 42.390625 31.78125 42.390625 
Q 38.140625 42.390625 41.71875 45.5625 
Q 45.3125 48.734375 45.3125 54.390625 
Q 45.3125 60.0625 41.71875 63.234375 
Q 38.140625 66.40625 31.78125 66.40625 
Q 25.390625 66.40625 21.84375 63.234375 
Q 18.3125 60.0625 18.3125 54.390625 
z
" id="DejaVuSans-56"/>
      </defs>
      <g transform="translate(27.240625 102.557344)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-56"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-48"/>
      </g>
     </g>
    </g>
    <g id="ytick_6">
     <g id="line2d_29">
      <path clip-path="url(#p9afea4b7e9)" d="M 53.328125 76.918125 
L 393.528125 76.918125 
" style="fill:none;stroke:#999999;stroke-linecap:square;stroke-opacity:0.15;stroke-width:0.8;"/>
     </g>
     <g id="line2d_30">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="53.328125" xlink:href="#m004a693e37" y="76.918125"/>
      </g>
     </g>
     <g id="text_10">
      <!-- 1000 -->
      <defs>
       <path d="M 12.40625 8.296875 
L 28.515625 8.296875 
L 28.515625 63.921875 
L 10.984375 60.40625 
L 10.984375 69.390625 
L 28.421875 72.90625 
L 38.28125 72.90625 
L 38.28125 8.296875 
L 54.390625 8.296875 
L 54.390625 0 
L 12.40625 0 
z
" id="DejaVuSans-49"/>
      </defs>
      <g transform="translate(20.878125 80.717344)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-49"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-48"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
      </g>
     </g>
    </g>
    <g id="ytick_7">
     <g id="line2d_31">
      <path clip-path="url(#p9afea4b7e9)" d="M 53.328125 55.078125 
L 393.528125 55.078125 
" style="fill:none;stroke:#999999;stroke-linecap:square;stroke-opacity:0.15;stroke-width:0.8;"/>
     </g>
     <g id="line2d_32">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="53.328125" xlink:href="#m004a693e37" y="55.078125"/>
      </g>
     </g>
     <g id="text_11">
      <!-- 1200 -->
      <g transform="translate(20.878125 58.877344)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-49"/>
       <use x="63.623047" xlink:href="#DejaVuSans-50"/>
       <use x="127.246094" xlink:href="#DejaVuSans-48"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
      </g>
     </g>
    </g>
    <g id="ytick_8">
     <g id="line2d_33">
      <path clip-path="url(#p9afea4b7e9)" d="M 53.328125 33.238125 
L 393.528125 33.238125 
" style="fill:none;stroke:#999999;stroke-linecap:square;stroke-opacity:0.15;stroke-width:0.8;"/>
     </g>
     <g id="line2d_34">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="53.328125" xlink:href="#m004a693e37" y="33.238125"/>
      </g>
     </g>
     <g id="text_12">
      <!-- 1400 -->
      <g transform="translate(20.878125 37.037344)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-49"/>
       <use x="63.623047" xlink:href="#DejaVuSans-52"/>
       <use x="127.246094" xlink:href="#DejaVuSans-48"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
      </g>
     </g>
    </g>
    <g id="text_13">
     <!-- Saisonal bereinigte Fallzahlen -->
     <defs>
      <path d="M 53.515625 70.515625 
L 53.515625 60.890625 
Q 47.90625 63.578125 42.921875 64.890625 
Q 37.9375 66.21875 33.296875 66.21875 
Q 25.25 66.21875 20.875 63.09375 
Q 16.5 59.96875 16.5 54.203125 
Q 16.5 49.359375 19.40625 46.890625 
Q 22.3125 44.4375 30.421875 42.921875 
L 36.375 41.703125 
Q 47.40625 39.59375 52.65625 34.296875 
Q 57.90625 29 57.90625 20.125 
Q 57.90625 9.515625 50.796875 4.046875 
Q 43.703125 -1.421875 29.984375 -1.421875 
Q 24.8125 -1.421875 18.96875 -0.25 
Q 13.140625 0.921875 6.890625 3.21875 
L 6.890625 13.375 
Q 12.890625 10.015625 18.65625 8.296875 
Q 24.421875 6.59375 29.984375 6.59375 
Q 38.421875 6.59375 43.015625 9.90625 
Q 47.609375 13.234375 47.609375 19.390625 
Q 47.609375 24.75 44.3125 27.78125 
Q 41.015625 30.8125 33.5 32.328125 
L 27.484375 33.5 
Q 16.453125 35.6875 11.515625 40.375 
Q 6.59375 45.0625 6.59375 53.421875 
Q 6.59375 63.09375 13.40625 68.65625 
Q 20.21875 74.21875 32.171875 74.21875 
Q 37.3125 74.21875 42.625 73.28125 
Q 47.953125 72.359375 53.515625 70.515625 
z
" id="DejaVuSans-83"/>
      <path d="M 30.609375 48.390625 
Q 23.390625 48.390625 19.1875 42.75 
Q 14.984375 37.109375 14.984375 27.296875 
Q 14.984375 17.484375 19.15625 11.84375 
Q 23.34375 6.203125 30.609375 6.203125 
Q 37.796875 6.203125 41.984375 11.859375 
Q 46.1875 17.53125 46.1875 27.296875 
Q 46.1875 37.015625 41.984375 42.703125 
Q 37.796875 48.390625 30.609375 48.390625 
z
M 30.609375 56 
Q 42.328125 56 49.015625 48.375 
Q 55.71875 40.765625 55.71875 27.296875 
Q 55.71875 13.875 49.015625 6.21875 
Q 42.328125 -1.421875 30.609375 -1.421875 
Q 18.84375 -1.421875 12.171875 6.21875 
Q 5.515625 13.875 5.515625 27.296875 
Q 5.515625 40.765625 12.171875 48.375 
Q 18.84375 56 30.609375 56 
z
" id="DejaVuSans-111"/>
      <path d="M 9.8125 72.90625 
L 51.703125 72.90625 
L 51.703125 64.59375 
L 19.671875 64.59375 
L 19.671875 43.109375 
L 48.578125 43.109375 
L 48.578125 34.8125 
L 19.671875 34.8125 
L 19.671875 0 
L 9.8125 0 
z
" id="DejaVuSans-70"/>
      <path d="M 5.515625 54.6875 
L 48.1875 54.6875 
L 48.1875 46.484375 
L 14.40625 7.171875 
L 48.1875 7.171875 
L 48.1875 0 
L 4.296875 0 
L 4.296875 8.203125 
L 38.09375 47.515625 
L 5.515625 47.515625 
z
" id="DejaVuSans-122"/>
      <path d="M 54.890625 33.015625 
L 54.890625 0 
L 45.90625 0 
L 45.90625 32.71875 
Q 45.90625 40.484375 42.875 44.328125 
Q 39.84375 48.1875 33.796875 48.1875 
Q 26.515625 48.1875 22.3125 43.546875 
Q 18.109375 38.921875 18.109375 30.90625 
L 18.109375 0 
L 9.078125 0 
L 9.078125 75.984375 
L 18.109375 75.984375 
L 18.109375 46.1875 
Q 21.34375 51.125 25.703125 53.5625 
Q 30.078125 56 35.796875 56 
Q 45.21875 56 50.046875 50.171875 
Q 54.890625 44.34375 54.890625 33.015625 
z
" id="DejaVuSans-104"/>
     </defs>
     <g transform="translate(14.798438 179.050937)rotate(-90)scale(0.1 -0.1)">
      <use xlink:href="#DejaVuSans-83"/>
      <use x="63.476562" xlink:href="#DejaVuSans-97"/>
      <use x="124.755859" xlink:href="#DejaVuSans-105"/>
      <use x="152.539062" xlink:href="#DejaVuSans-115"/>
      <use x="204.638672" xlink:href="#DejaVuSans-111"/>
      <use x="265.820312" xlink:href="#DejaVuSans-110"/>
      <use x="329.199219" xlink:href="#DejaVuSans-97"/>
      <use x="390.478516" xlink:href="#DejaVuSans-108"/>
      <use x="418.261719" xlink:href="#DejaVuSans-32"/>
      <use x="450.048828" xlink:href="#DejaVuSans-98"/>
      <use x="513.525391" xlink:href="#DejaVuSans-101"/>
      <use x="575.048828" xlink:href="#DejaVuSans-114"/>
      <use x="616.130859" xlink:href="#DejaVuSans-101"/>
      <use x="677.654297" xlink:href="#DejaVuSans-105"/>
      <use x="705.4375" xlink:href="#DejaVuSans-110"/>
      <use x="768.816406" xlink:href="#DejaVuSans-105"/>
      <use x="796.599609" xlink:href="#DejaVuSans-103"/>
      <use x="860.076172" xlink:href="#DejaVuSans-116"/>
      <use x="899.285156" xlink:href="#DejaVuSans-101"/>
      <use x="960.808594" xlink:href="#DejaVuSans-32"/>
      <use x="992.595703" xlink:href="#DejaVuSans-70"/>
      <use x="1049.974609" xlink:href="#DejaVuSans-97"/>
      <use x="1111.253906" xlink:href="#DejaVuSans-108"/>
      <use x="1139.037109" xlink:href="#DejaVuSans-108"/>
      <use x="1166.820312" xlink:href="#DejaVuSans-122"/>
      <use x="1219.310547" xlink:href="#DejaVuSans-97"/>
      <use x="1280.589844" xlink:href="#DejaVuSans-104"/>
      <use x="1343.96875" xlink:href="#DejaVuSans-108"/>
      <use x="1371.751953" xlink:href="#DejaVuSans-101"/>
      <use x="1433.275391" xlink:href="#DejaVuSans-110"/>
     </g>
    </g>
   </g>
   <g id="line2d_35">
    <path clip-path="url(#p9afea4b7e9)" d="M 37.672339 -1 
L 39.58267 8.208551 
L 43.019034 12.477007 
L 46.455398 18.819213 
L 49.891761 30.004547 
L 53.328125 46.908468 
L 56.764489 54.018845 
L 60.200852 44.944262 
L 63.637216 62.378355 
L 67.07358 64.315587 
L 70.509943 70.404111 
L 73.946307 77.066018 
L 77.38267 88.753616 
L 80.819034 98.322287 
L 84.255398 81.844495 
L 87.691761 97.701805 
L 91.128125 96.216252 
L 94.564489 88.836431 
L 98.000852 97.630695 
L 101.437216 101.708134 
L 104.87358 110.082469 
L 108.309943 107.8852 
L 111.746307 112.778888 
L 115.18267 115.18748 
L 118.619034 115.076888 
L 122.055398 120.765956 
L 125.491761 122.168046 
L 128.928125 126.506171 
L 132.364489 128.052894 
L 135.800852 112.994275 
L 139.237216 118.933392 
L 142.67358 129.54114 
L 146.109943 125.017307 
L 149.546307 137.692905 
L 152.98267 128.837931 
L 156.419034 142.901636 
L 159.855398 144.763842 
L 163.291761 142.496383 
L 166.728125 138.501296 
L 170.164489 140.04534 
L 173.600852 141.394195 
L 177.037216 139.888446 
L 180.47358 143.788129 
L 183.909943 148.317725 
L 187.346307 150.834057 
L 194.219034 153.491475 
L 197.655398 140.982941 
L 201.091761 145.869918 
L 204.528125 147.998966 
L 207.964489 152.194689 
L 211.400852 150.229877 
L 214.837216 156.037601 
L 218.27358 145.186509 
L 221.709943 140.263245 
L 228.58267 145.007055 
L 232.019034 146.486937 
L 235.455398 141.892204 
L 238.891761 140.293327 
L 242.328125 122.347854 
L 245.764489 70.658417 
L 249.200852 118.29432 
L 252.637216 126.390722 
L 256.07358 124.302087 
L 259.509943 129.083603 
L 262.946307 138.245292 
L 266.38267 138.957785 
L 269.819034 142.113891 
L 273.255398 138.773256 
L 276.691761 141.350275 
L 280.128125 139.594556 
L 283.564489 143.46307 
L 287.000852 145.669421 
L 290.437216 144.000086 
L 293.87358 140.571686 
L 297.309943 145.667156 
L 300.746307 147.998966 
L 304.18267 148.640806 
L 307.619034 150.350713 
L 311.055398 147.717456 
L 314.491761 150.525416 
L 317.928125 149.824913 
L 321.364489 152.155532 
L 324.800852 144.231375 
L 328.237216 138.733008 
L 331.67358 138.5088 
L 335.109943 139.013305 
L 338.546307 132.729061 
L 341.98267 131.832528 
L 345.419034 130.155882 
L 348.855398 133.925904 
L 352.291761 129.794452 
L 355.728125 129.204439 
L 359.164489 120.580984 
L 362.600852 123.138803 
L 366.037216 114.045769 
L 369.47358 111.501801 
L 372.909943 111.209545 
L 376.346307 109.548084 
L 379.78267 109.991539 
L 383.219034 96.644567 
L 386.655398 87.150619 
L 390.091761 97.904029 
L 390.091761 97.904029 
" style="fill:none;stroke:#1f77b4;stroke-linecap:square;stroke-width:1.5;"/>
   </g>
   <g id="patch_3">
    <path d="M 53.328125 186.118125 
L 53.328125 22.318125 
" style="fill:none;stroke:#000000;stroke-linecap:square;stroke-linejoin:miter;stroke-width:0.8;"/>
   </g>
   <g id="patch_4">
    <path d="M 393.528125 186.118125 
L 393.528125 22.318125 
" style="fill:none;stroke:#000000;stroke-linecap:square;stroke-linejoin:miter;stroke-width:0.8;"/>
   </g>
   <g id="patch_5">
    <path d="M 53.328125 186.118125 
L 393.528125 186.118125 
" style="fill:none;stroke:#000000;stroke-linecap:square;stroke-linejoin:miter;stroke-width:0.8;"/>
   </g>
   <g id="patch_6">
    <path d="M 53.328125 22.318125 
L 393.528125 22.318125 
" style="fill:none;stroke:#000000;stroke-linecap:square;stroke-linejoin:miter;stroke-width:0.8;"/>
   </g>
   <g id="text_14">
    <!-- Deutsche COVID-19 Fallzahlen nach Erkrankungsbeginn -->
    <defs>
     <path d="M 48.78125 52.59375 
L 48.78125 44.1875 
Q 44.96875 46.296875 41.140625 47.34375 
Q 37.3125 48.390625 33.40625 48.390625 
Q 24.65625 48.390625 19.8125 42.84375 
Q 14.984375 37.3125 14.984375 27.296875 
Q 14.984375 17.28125 19.8125 11.734375 
Q 24.65625 6.203125 33.40625 6.203125 
Q 37.3125 6.203125 41.140625 7.25 
Q 44.96875 8.296875 48.78125 10.40625 
L 48.78125 2.09375 
Q 45.015625 0.34375 40.984375 -0.53125 
Q 36.96875 -1.421875 32.421875 -1.421875 
Q 20.0625 -1.421875 12.78125 6.34375 
Q 5.515625 14.109375 5.515625 27.296875 
Q 5.515625 40.671875 12.859375 48.328125 
Q 20.21875 56 33.015625 56 
Q 37.15625 56 41.109375 55.140625 
Q 45.0625 54.296875 48.78125 52.59375 
z
" id="DejaVuSans-99"/>
     <path d="M 64.40625 67.28125 
L 64.40625 56.890625 
Q 59.421875 61.53125 53.78125 63.8125 
Q 48.140625 66.109375 41.796875 66.109375 
Q 29.296875 66.109375 22.65625 58.46875 
Q 16.015625 50.828125 16.015625 36.375 
Q 16.015625 21.96875 22.65625 14.328125 
Q 29.296875 6.6875 41.796875 6.6875 
Q 48.140625 6.6875 53.78125 8.984375 
Q 59.421875 11.28125 64.40625 15.921875 
L 64.40625 5.609375 
Q 59.234375 2.09375 53.4375 0.328125 
Q 47.65625 -1.421875 41.21875 -1.421875 
Q 24.65625 -1.421875 15.125 8.703125 
Q 5.609375 18.84375 5.609375 36.375 
Q 5.609375 53.953125 15.125 64.078125 
Q 24.65625 74.21875 41.21875 74.21875 
Q 47.75 74.21875 53.53125 72.484375 
Q 59.328125 70.75 64.40625 67.28125 
z
" id="DejaVuSans-67"/>
     <path d="M 39.40625 66.21875 
Q 28.65625 66.21875 22.328125 58.203125 
Q 16.015625 50.203125 16.015625 36.375 
Q 16.015625 22.609375 22.328125 14.59375 
Q 28.65625 6.59375 39.40625 6.59375 
Q 50.140625 6.59375 56.421875 14.59375 
Q 62.703125 22.609375 62.703125 36.375 
Q 62.703125 50.203125 56.421875 58.203125 
Q 50.140625 66.21875 39.40625 66.21875 
z
M 39.40625 74.21875 
Q 54.734375 74.21875 63.90625 63.9375 
Q 73.09375 53.65625 73.09375 36.375 
Q 73.09375 19.140625 63.90625 8.859375 
Q 54.734375 -1.421875 39.40625 -1.421875 
Q 24.03125 -1.421875 14.8125 8.828125 
Q 5.609375 19.09375 5.609375 36.375 
Q 5.609375 53.65625 14.8125 63.9375 
Q 24.03125 74.21875 39.40625 74.21875 
z
" id="DejaVuSans-79"/>
     <path d="M 28.609375 0 
L 0.78125 72.90625 
L 11.078125 72.90625 
L 34.1875 11.53125 
L 57.328125 72.90625 
L 67.578125 72.90625 
L 39.796875 0 
z
" id="DejaVuSans-86"/>
     <path d="M 9.8125 72.90625 
L 19.671875 72.90625 
L 19.671875 0 
L 9.8125 0 
z
" id="DejaVuSans-73"/>
     <path d="M 4.890625 31.390625 
L 31.203125 31.390625 
L 31.203125 23.390625 
L 4.890625 23.390625 
z
" id="DejaVuSans-45"/>
     <path d="M 10.984375 1.515625 
L 10.984375 10.5 
Q 14.703125 8.734375 18.5 7.8125 
Q 22.3125 6.890625 25.984375 6.890625 
Q 35.75 6.890625 40.890625 13.453125 
Q 46.046875 20.015625 46.78125 33.40625 
Q 43.953125 29.203125 39.59375 26.953125 
Q 35.25 24.703125 29.984375 24.703125 
Q 19.046875 24.703125 12.671875 31.3125 
Q 6.296875 37.9375 6.296875 49.421875 
Q 6.296875 60.640625 12.9375 67.421875 
Q 19.578125 74.21875 30.609375 74.21875 
Q 43.265625 74.21875 49.921875 64.515625 
Q 56.59375 54.828125 56.59375 36.375 
Q 56.59375 19.140625 48.40625 8.859375 
Q 40.234375 -1.421875 26.421875 -1.421875 
Q 22.703125 -1.421875 18.890625 -0.6875 
Q 15.09375 0.046875 10.984375 1.515625 
z
M 30.609375 32.421875 
Q 37.25 32.421875 41.125 36.953125 
Q 45.015625 41.5 45.015625 49.421875 
Q 45.015625 57.28125 41.125 61.84375 
Q 37.25 66.40625 30.609375 66.40625 
Q 23.96875 66.40625 20.09375 61.84375 
Q 16.21875 57.28125 16.21875 49.421875 
Q 16.21875 41.5 20.09375 36.953125 
Q 23.96875 32.421875 30.609375 32.421875 
z
" id="DejaVuSans-57"/>
    </defs>
    <g transform="translate(55.114063 16.318125)scale(0.12 -0.12)">
     <use xlink:href="#DejaVuSans-68"/>
     <use x="77.001953" xlink:href="#DejaVuSans-101"/>
     <use x="138.525391" xlink:href="#DejaVuSans-117"/>
     <use x="201.904297" xlink:href="#DejaVuSans-116"/>
     <use x="241.113281" xlink:href="#DejaVuSans-115"/>
     <use x="293.212891" xlink:href="#DejaVuSans-99"/>
     <use x="348.193359" xlink:href="#DejaVuSans-104"/>
     <use x="411.572266" xlink:href="#DejaVuSans-101"/>
     <use x="473.095703" xlink:href="#DejaVuSans-32"/>
     <use x="504.882812" xlink:href="#DejaVuSans-67"/>
     <use x="574.707031" xlink:href="#DejaVuSans-79"/>
     <use x="653.402344" xlink:href="#DejaVuSans-86"/>
     <use x="721.810547" xlink:href="#DejaVuSans-73"/>
     <use x="751.302734" xlink:href="#DejaVuSans-68"/>
     <use x="828.304688" xlink:href="#DejaVuSans-45"/>
     <use x="864.388672" xlink:href="#DejaVuSans-49"/>
     <use x="928.011719" xlink:href="#DejaVuSans-57"/>
     <use x="991.634766" xlink:href="#DejaVuSans-32"/>
     <use x="1023.421875" xlink:href="#DejaVuSans-70"/>
     <use x="1080.800781" xlink:href="#DejaVuSans-97"/>
     <use x="1142.080078" xlink:href="#DejaVuSans-108"/>
     <use x="1169.863281" xlink:href="#DejaVuSans-108"/>
     <use x="1197.646484" xlink:href="#DejaVuSans-122"/>
     <use x="1250.136719" xlink:href="#DejaVuSans-97"/>
     <use x="1311.416016" xlink:href="#DejaVuSans-104"/>
     <use x="1374.794922" xlink:href="#DejaVuSans-108"/>
     <use x="1402.578125" xlink:href="#DejaVuSans-101"/>
     <use x="1464.101562" xlink:href="#DejaVuSans-110"/>
     <use x="1527.480469" xlink:href="#DejaVuSans-32"/>
     <use x="1559.267578" xlink:href="#DejaVuSans-110"/>
     <use x="1622.646484" xlink:href="#DejaVuSans-97"/>
     <use x="1683.925781" xlink:href="#DejaVuSans-99"/>
     <use x="1738.90625" xlink:href="#DejaVuSans-104"/>
     <use x="1802.285156" xlink:href="#DejaVuSans-32"/>
     <use x="1834.072266" xlink:href="#DejaVuSans-69"/>
     <use x="1897.255859" xlink:href="#DejaVuSans-114"/>
     <use x="1938.369141" xlink:href="#DejaVuSans-107"/>
     <use x="1996.279297" xlink:href="#DejaVuSans-114"/>
     <use x="2037.392578" xlink:href="#DejaVuSans-97"/>
     <use x="2098.671875" xlink:href="#DejaVuSans-110"/>
     <use x="2162.050781" xlink:href="#DejaVuSans-107"/>
     <use x="2219.914062" xlink:href="#DejaVuSans-117"/>
     <use x="2283.292969" xlink:href="#DejaVuSans-110"/>
     <use x="2346.671875" xlink:href="#DejaVuSans-103"/>
     <use x="2410.148438" xlink:href="#DejaVuSans-115"/>
     <use x="2462.248047" xlink:href="#DejaVuSans-98"/>
     <use x="2525.724609" xlink:href="#DejaVuSans-101"/>
     <use x="2587.248047" xlink:href="#DejaVuSans-103"/>
     <use x="2650.724609" xlink:href="#DejaVuSans-105"/>
     <use x="2678.507812" xlink:href="#DejaVuSans-110"/>
     <use x="2741.886719" xlink:href="#DejaVuSans-110"/>
    </g>
   </g>
   <g id="legend_1">
    <g id="patch_7">
     <path d="M 234.242188 38.916562 
L 254.242188 38.916562 
L 254.242188 31.916562 
L 234.242188 31.916562 
z
" style="fill:#008000;opacity:0.3;"/>
    </g>
    <g id="text_15">
     <!-- 95%-Prädiktionsintervall -->
     <defs>
      <path d="M 10.796875 72.90625 
L 49.515625 72.90625 
L 49.515625 64.59375 
L 19.828125 64.59375 
L 19.828125 46.734375 
Q 21.96875 47.46875 24.109375 47.828125 
Q 26.265625 48.1875 28.421875 48.1875 
Q 40.625 48.1875 47.75 41.5 
Q 54.890625 34.8125 54.890625 23.390625 
Q 54.890625 11.625 47.5625 5.09375 
Q 40.234375 -1.421875 26.90625 -1.421875 
Q 22.3125 -1.421875 17.546875 -0.640625 
Q 12.796875 0.140625 7.71875 1.703125 
L 7.71875 11.625 
Q 12.109375 9.234375 16.796875 8.0625 
Q 21.484375 6.890625 26.703125 6.890625 
Q 35.15625 6.890625 40.078125 11.328125 
Q 45.015625 15.765625 45.015625 23.390625 
Q 45.015625 31 40.078125 35.4375 
Q 35.15625 39.890625 26.703125 39.890625 
Q 22.75 39.890625 18.8125 39.015625 
Q 14.890625 38.140625 10.796875 36.28125 
z
" id="DejaVuSans-53"/>
      <path d="M 72.703125 32.078125 
Q 68.453125 32.078125 66.03125 28.46875 
Q 63.625 24.859375 63.625 18.40625 
Q 63.625 12.0625 66.03125 8.421875 
Q 68.453125 4.78125 72.703125 4.78125 
Q 76.859375 4.78125 79.265625 8.421875 
Q 81.6875 12.0625 81.6875 18.40625 
Q 81.6875 24.8125 79.265625 28.4375 
Q 76.859375 32.078125 72.703125 32.078125 
z
M 72.703125 38.28125 
Q 80.421875 38.28125 84.953125 32.90625 
Q 89.5 27.546875 89.5 18.40625 
Q 89.5 9.28125 84.9375 3.921875 
Q 80.375 -1.421875 72.703125 -1.421875 
Q 64.890625 -1.421875 60.34375 3.921875 
Q 55.8125 9.28125 55.8125 18.40625 
Q 55.8125 27.59375 60.375 32.9375 
Q 64.9375 38.28125 72.703125 38.28125 
z
M 22.3125 68.015625 
Q 18.109375 68.015625 15.6875 64.375 
Q 13.28125 60.75 13.28125 54.390625 
Q 13.28125 47.953125 15.671875 44.328125 
Q 18.0625 40.71875 22.3125 40.71875 
Q 26.5625 40.71875 28.96875 44.328125 
Q 31.390625 47.953125 31.390625 54.390625 
Q 31.390625 60.6875 28.953125 64.34375 
Q 26.515625 68.015625 22.3125 68.015625 
z
M 66.40625 74.21875 
L 74.21875 74.21875 
L 28.609375 -1.421875 
L 20.796875 -1.421875 
z
M 22.3125 74.21875 
Q 30.03125 74.21875 34.609375 68.875 
Q 39.203125 63.53125 39.203125 54.390625 
Q 39.203125 45.171875 34.640625 39.84375 
Q 30.078125 34.515625 22.3125 34.515625 
Q 14.546875 34.515625 10.03125 39.859375 
Q 5.515625 45.21875 5.515625 54.390625 
Q 5.515625 63.484375 10.046875 68.84375 
Q 14.59375 74.21875 22.3125 74.21875 
z
" id="DejaVuSans-37"/>
      <path d="M 19.671875 64.796875 
L 19.671875 37.40625 
L 32.078125 37.40625 
Q 38.96875 37.40625 42.71875 40.96875 
Q 46.484375 44.53125 46.484375 51.125 
Q 46.484375 57.671875 42.71875 61.234375 
Q 38.96875 64.796875 32.078125 64.796875 
z
M 9.8125 72.90625 
L 32.078125 72.90625 
Q 44.34375 72.90625 50.609375 67.359375 
Q 56.890625 61.8125 56.890625 51.125 
Q 56.890625 40.328125 50.609375 34.8125 
Q 44.34375 29.296875 32.078125 29.296875 
L 19.671875 29.296875 
L 19.671875 0 
L 9.8125 0 
z
" id="DejaVuSans-80"/>
      <path d="M 34.28125 27.484375 
Q 23.390625 27.484375 19.1875 25 
Q 14.984375 22.515625 14.984375 16.5 
Q 14.984375 11.71875 18.140625 8.90625 
Q 21.296875 6.109375 26.703125 6.109375 
Q 34.1875 6.109375 38.703125 11.40625 
Q 43.21875 16.703125 43.21875 25.484375 
L 43.21875 27.484375 
z
M 52.203125 31.203125 
L 52.203125 0 
L 43.21875 0 
L 43.21875 8.296875 
Q 40.140625 3.328125 35.546875 0.953125 
Q 30.953125 -1.421875 24.3125 -1.421875 
Q 15.921875 -1.421875 10.953125 3.296875 
Q 6 8.015625 6 15.921875 
Q 6 25.140625 12.171875 29.828125 
Q 18.359375 34.515625 30.609375 34.515625 
L 43.21875 34.515625 
L 43.21875 35.40625 
Q 43.21875 41.609375 39.140625 45 
Q 35.0625 48.390625 27.6875 48.390625 
Q 23 48.390625 18.546875 47.265625 
Q 14.109375 46.140625 10.015625 43.890625 
L 10.015625 52.203125 
Q 14.9375 54.109375 19.578125 55.046875 
Q 24.21875 56 28.609375 56 
Q 40.484375 56 46.34375 49.84375 
Q 52.203125 43.703125 52.203125 31.203125 
z
M 33.59375 75.78125 
L 43.5 75.78125 
L 43.5 65.921875 
L 33.59375 65.921875 
z
M 14.5 75.78125 
L 24.421875 75.78125 
L 24.421875 65.921875 
L 14.5 65.921875 
z
" id="DejaVuSans-228"/>
      <path d="M 2.984375 54.6875 
L 12.5 54.6875 
L 29.59375 8.796875 
L 46.6875 54.6875 
L 56.203125 54.6875 
L 35.6875 0 
L 23.484375 0 
z
" id="DejaVuSans-118"/>
     </defs>
     <g transform="translate(262.242188 38.916562)scale(0.1 -0.1)">
      <use xlink:href="#DejaVuSans-57"/>
      <use x="63.623047" xlink:href="#DejaVuSans-53"/>
      <use x="127.246094" xlink:href="#DejaVuSans-37"/>
      <use x="222.265625" xlink:href="#DejaVuSans-45"/>
      <use x="258.349609" xlink:href="#DejaVuSans-80"/>
      <use x="318.636719" xlink:href="#DejaVuSans-114"/>
      <use x="359.75" xlink:href="#DejaVuSans-228"/>
      <use x="421.029297" xlink:href="#DejaVuSans-100"/>
      <use x="484.505859" xlink:href="#DejaVuSans-105"/>
      <use x="512.289062" xlink:href="#DejaVuSans-107"/>
      <use x="570.199219" xlink:href="#DejaVuSans-116"/>
      <use x="609.408203" xlink:href="#DejaVuSans-105"/>
      <use x="637.191406" xlink:href="#DejaVuSans-111"/>
      <use x="698.373047" xlink:href="#DejaVuSans-110"/>
      <use x="761.751953" xlink:href="#DejaVuSans-115"/>
      <use x="813.851562" xlink:href="#DejaVuSans-105"/>
      <use x="841.634766" xlink:href="#DejaVuSans-110"/>
      <use x="905.013672" xlink:href="#DejaVuSans-116"/>
      <use x="944.222656" xlink:href="#DejaVuSans-101"/>
      <use x="1005.746094" xlink:href="#DejaVuSans-114"/>
      <use x="1046.859375" xlink:href="#DejaVuSans-118"/>
      <use x="1106.039062" xlink:href="#DejaVuSans-97"/>
      <use x="1167.318359" xlink:href="#DejaVuSans-108"/>
      <use x="1195.101562" xlink:href="#DejaVuSans-108"/>
     </g>
    </g>
   </g>
  </g>
  <g id="text_16">
   <!-- Datenstand: 1. August 2020 -->
   <defs>
    <path d="M 11.71875 12.40625 
L 22.015625 12.40625 
L 22.015625 0 
L 11.71875 0 
z
M 11.71875 51.703125 
L 22.015625 51.703125 
L 22.015625 39.3125 
L 11.71875 39.3125 
z
" id="DejaVuSans-58"/>
    <path d="M 10.6875 12.40625 
L 21 12.40625 
L 21 0 
L 10.6875 0 
z
" id="DejaVuSans-46"/>
    <path d="M 34.1875 63.1875 
L 20.796875 26.90625 
L 47.609375 26.90625 
z
M 28.609375 72.90625 
L 39.796875 72.90625 
L 67.578125 0 
L 57.328125 0 
L 50.6875 18.703125 
L 17.828125 18.703125 
L 11.1875 0 
L 0.78125 0 
z
" id="DejaVuSans-65"/>
   </defs>
   <g transform="translate(327.852969 231.840469)scale(0.05 -0.05)">
    <use xlink:href="#DejaVuSans-68"/>
    <use x="77.001953" xlink:href="#DejaVuSans-97"/>
    <use x="138.28125" xlink:href="#DejaVuSans-116"/>
    <use x="177.490234" xlink:href="#DejaVuSans-101"/>
    <use x="239.013672" xlink:href="#DejaVuSans-110"/>
    <use x="302.392578" xlink:href="#DejaVuSans-115"/>
    <use x="354.492188" xlink:href="#DejaVuSans-116"/>
    <use x="393.701172" xlink:href="#DejaVuSans-97"/>
    <use x="454.980469" xlink:href="#DejaVuSans-110"/>
    <use x="518.359375" xlink:href="#DejaVuSans-100"/>
    <use x="581.835938" xlink:href="#DejaVuSans-58"/>
    <use x="615.527344" xlink:href="#DejaVuSans-32"/>
    <use x="647.314453" xlink:href="#DejaVuSans-49"/>
    <use x="710.9375" xlink:href="#DejaVuSans-46"/>
    <use x="742.724609" xlink:href="#DejaVuSans-32"/>
    <use x="774.511719" xlink:href="#DejaVuSans-65"/>
    <use x="842.919922" xlink:href="#DejaVuSans-117"/>
    <use x="906.298828" xlink:href="#DejaVuSans-103"/>
    <use x="969.775391" xlink:href="#DejaVuSans-117"/>
    <use x="1033.154297" xlink:href="#DejaVuSans-115"/>
    <use x="1085.253906" xlink:href="#DejaVuSans-116"/>
    <use x="1124.462891" xlink:href="#DejaVuSans-32"/>
    <use x="1156.25" xlink:href="#DejaVuSans-50"/>
    <use x="1219.873047" xlink:href="#DejaVuSans-48"/>
    <use x="1283.496094" xlink:href="#DejaVuSans-50"/>
    <use x="1347.119141" xlink:href="#DejaVuSans-48"/>
   </g>
   <!-- Datenquelle:RKI Nowcast -->
   <defs>
    <path d="M 14.796875 27.296875 
Q 14.796875 17.390625 18.875 11.75 
Q 22.953125 6.109375 30.078125 6.109375 
Q 37.203125 6.109375 41.296875 11.75 
Q 45.40625 17.390625 45.40625 27.296875 
Q 45.40625 37.203125 41.296875 42.84375 
Q 37.203125 48.484375 30.078125 48.484375 
Q 22.953125 48.484375 18.875 42.84375 
Q 14.796875 37.203125 14.796875 27.296875 
z
M 45.40625 8.203125 
Q 42.578125 3.328125 38.25 0.953125 
Q 33.9375 -1.421875 27.875 -1.421875 
Q 17.96875 -1.421875 11.734375 6.484375 
Q 5.515625 14.40625 5.515625 27.296875 
Q 5.515625 40.1875 11.734375 48.09375 
Q 17.96875 56 27.875 56 
Q 33.9375 56 38.25 53.625 
Q 42.578125 51.265625 45.40625 46.390625 
L 45.40625 54.6875 
L 54.390625 54.6875 
L 54.390625 -20.796875 
L 45.40625 -20.796875 
z
" id="DejaVuSans-113"/>
    <path d="M 44.390625 34.1875 
Q 47.5625 33.109375 50.5625 29.59375 
Q 53.5625 26.078125 56.59375 19.921875 
L 66.609375 0 
L 56 0 
L 46.6875 18.703125 
Q 43.0625 26.03125 39.671875 28.421875 
Q 36.28125 30.8125 30.421875 30.8125 
L 19.671875 30.8125 
L 19.671875 0 
L 9.8125 0 
L 9.8125 72.90625 
L 32.078125 72.90625 
Q 44.578125 72.90625 50.734375 67.671875 
Q 56.890625 62.453125 56.890625 51.90625 
Q 56.890625 45.015625 53.6875 40.46875 
Q 50.484375 35.9375 44.390625 34.1875 
z
M 19.671875 64.796875 
L 19.671875 38.921875 
L 32.078125 38.921875 
Q 39.203125 38.921875 42.84375 42.21875 
Q 46.484375 45.515625 46.484375 51.90625 
Q 46.484375 58.296875 42.84375 61.546875 
Q 39.203125 64.796875 32.078125 64.796875 
z
" id="DejaVuSans-82"/>
    <path d="M 9.8125 72.90625 
L 19.671875 72.90625 
L 19.671875 42.09375 
L 52.390625 72.90625 
L 65.09375 72.90625 
L 28.90625 38.921875 
L 67.671875 0 
L 54.6875 0 
L 19.671875 35.109375 
L 19.671875 0 
L 9.8125 0 
z
" id="DejaVuSans-75"/>
    <path d="M 9.8125 72.90625 
L 23.09375 72.90625 
L 55.421875 11.921875 
L 55.421875 72.90625 
L 64.984375 72.90625 
L 64.984375 0 
L 51.703125 0 
L 19.390625 60.984375 
L 19.390625 0 
L 9.8125 0 
z
" id="DejaVuSans-78"/>
    <path d="M 4.203125 54.6875 
L 13.1875 54.6875 
L 24.421875 12.015625 
L 35.59375 54.6875 
L 46.1875 54.6875 
L 57.421875 12.015625 
L 68.609375 54.6875 
L 77.59375 54.6875 
L 63.28125 0 
L 52.6875 0 
L 40.921875 44.828125 
L 29.109375 0 
L 18.5 0 
z
" id="DejaVuSans-119"/>
   </defs>
   <g transform="translate(335.225625 237.439375)scale(0.05 -0.05)">
    <use xlink:href="#DejaVuSans-68"/>
    <use x="77.001953" xlink:href="#DejaVuSans-97"/>
    <use x="138.28125" xlink:href="#DejaVuSans-116"/>
    <use x="177.490234" xlink:href="#DejaVuSans-101"/>
    <use x="239.013672" xlink:href="#DejaVuSans-110"/>
    <use x="302.392578" xlink:href="#DejaVuSans-113"/>
    <use x="365.869141" xlink:href="#DejaVuSans-117"/>
    <use x="429.248047" xlink:href="#DejaVuSans-101"/>
    <use x="490.771484" xlink:href="#DejaVuSans-108"/>
    <use x="518.554688" xlink:href="#DejaVuSans-108"/>
    <use x="546.337891" xlink:href="#DejaVuSans-101"/>
    <use x="607.861328" xlink:href="#DejaVuSans-58"/>
    <use x="641.552734" xlink:href="#DejaVuSans-82"/>
    <use x="711.035156" xlink:href="#DejaVuSans-75"/>
    <use x="776.611328" xlink:href="#DejaVuSans-73"/>
    <use x="806.103516" xlink:href="#DejaVuSans-32"/>
    <use x="837.890625" xlink:href="#DejaVuSans-78"/>
    <use x="912.695312" xlink:href="#DejaVuSans-111"/>
    <use x="973.876953" xlink:href="#DejaVuSans-119"/>
    <use x="1055.664062" xlink:href="#DejaVuSans-99"/>
    <use x="1110.644531" xlink:href="#DejaVuSans-97"/>
    <use x="1171.923828" xlink:href="#DejaVuSans-115"/>
    <use x="1224.023438" xlink:href="#DejaVuSans-116"/>
   </g>
   <!-- Viz: @CorneliusRoemer -->
   <defs>
    <path d="M 37.203125 26.21875 
Q 37.203125 19.234375 40.671875 15.25 
Q 44.140625 11.28125 50.203125 11.28125 
Q 56.203125 11.28125 59.640625 15.28125 
Q 63.09375 19.28125 63.09375 26.21875 
Q 63.09375 33.0625 59.578125 37.078125 
Q 56.0625 41.109375 50.09375 41.109375 
Q 44.1875 41.109375 40.6875 37.109375 
Q 37.203125 33.109375 37.203125 26.21875 
z
M 63.8125 11.625 
Q 60.890625 7.859375 57.109375 6.078125 
Q 53.328125 4.296875 48.296875 4.296875 
Q 39.890625 4.296875 34.640625 10.375 
Q 29.390625 16.453125 29.390625 26.21875 
Q 29.390625 35.984375 34.65625 42.078125 
Q 39.9375 48.1875 48.296875 48.1875 
Q 53.328125 48.1875 57.125 46.359375 
Q 60.9375 44.53125 63.8125 40.828125 
L 63.8125 47.21875 
L 70.796875 47.21875 
L 70.796875 11.28125 
Q 77.9375 12.359375 81.953125 17.796875 
Q 85.984375 23.25 85.984375 31.890625 
Q 85.984375 37.109375 84.4375 41.703125 
Q 82.90625 46.296875 79.78125 50.203125 
Q 74.703125 56.59375 67.40625 59.984375 
Q 60.109375 63.375 51.515625 63.375 
Q 45.515625 63.375 39.984375 61.78125 
Q 34.46875 60.203125 29.78125 57.078125 
Q 22.125 52.09375 17.796875 44.015625 
Q 13.484375 35.9375 13.484375 26.515625 
Q 13.484375 18.75 16.28125 11.953125 
Q 19.09375 5.171875 24.421875 0 
Q 29.546875 -5.078125 36.28125 -7.734375 
Q 43.015625 -10.40625 50.6875 -10.40625 
Q 56.984375 -10.40625 63.0625 -8.28125 
Q 69.140625 -6.15625 74.21875 -2.203125 
L 78.609375 -7.625 
Q 72.515625 -12.359375 65.3125 -14.875 
Q 58.109375 -17.390625 50.6875 -17.390625 
Q 41.65625 -17.390625 33.640625 -14.1875 
Q 25.640625 -10.984375 19.390625 -4.890625 
Q 13.140625 1.21875 9.859375 9.25 
Q 6.59375 17.28125 6.59375 26.515625 
Q 6.59375 35.40625 9.90625 43.453125 
Q 13.234375 51.515625 19.390625 57.625 
Q 25.6875 63.8125 33.9375 67.109375 
Q 42.1875 70.40625 51.421875 70.40625 
Q 61.765625 70.40625 70.625 66.15625 
Q 79.5 61.921875 85.5 54.109375 
Q 89.15625 49.3125 91.078125 43.703125 
Q 93.015625 38.09375 93.015625 32.078125 
Q 93.015625 19.234375 85.25 11.8125 
Q 77.484375 4.390625 63.8125 4.109375 
z
" id="DejaVuSans-64"/>
   </defs>
   <g transform="translate(339.670937 243.038281)scale(0.05 -0.05)">
    <use xlink:href="#DejaVuSans-86"/>
    <use x="68.376953" xlink:href="#DejaVuSans-105"/>
    <use x="96.160156" xlink:href="#DejaVuSans-122"/>
    <use x="148.650391" xlink:href="#DejaVuSans-58"/>
    <use x="182.341797" xlink:href="#DejaVuSans-32"/>
    <use x="214.128906" xlink:href="#DejaVuSans-64"/>
    <use x="314.128906" xlink:href="#DejaVuSans-67"/>
    <use x="383.953125" xlink:href="#DejaVuSans-111"/>
    <use x="445.134766" xlink:href="#DejaVuSans-114"/>
    <use x="486.232422" xlink:href="#DejaVuSans-110"/>
    <use x="549.611328" xlink:href="#DejaVuSans-101"/>
    <use x="611.134766" xlink:href="#DejaVuSans-108"/>
    <use x="638.917969" xlink:href="#DejaVuSans-105"/>
    <use x="666.701172" xlink:href="#DejaVuSans-117"/>
    <use x="730.080078" xlink:href="#DejaVuSans-115"/>
    <use x="782.179688" xlink:href="#DejaVuSans-82"/>
    <use x="851.599609" xlink:href="#DejaVuSans-111"/>
    <use x="912.78125" xlink:href="#DejaVuSans-101"/>
    <use x="974.304688" xlink:href="#DejaVuSans-109"/>
    <use x="1071.716797" xlink:href="#DejaVuSans-101"/>
    <use x="1133.240234" xlink:href="#DejaVuSans-114"/>
   </g>
  </g>
 </g>
 <defs>
  <clipPath id="p9afea4b7e9">
   <rect height="163.8" width="340.2" x="53.328125" y="22.318125"/>
  </clipPath>
 </defs>
</svg>

</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[81]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">adjusted_b</span> <span class="o">=</span> <span class="n">result_b</span><span class="o">.</span><span class="n">observed</span> <span class="o">/</span> <span class="n">result_b</span><span class="o">.</span><span class="n">seasonal</span>
<span class="n">adjusted_c</span> <span class="o">=</span> <span class="n">nowcast</span><span class="o">.</span><span class="n">c</span><span class="p">[</span><span class="mi">10</span><span class="p">:]</span> <span class="o">/</span> <span class="n">result_b</span><span class="o">.</span><span class="n">seasonal</span>
<span class="n">adjusted_d</span> <span class="o">=</span> <span class="n">nowcast</span><span class="o">.</span><span class="n">d</span><span class="p">[</span><span class="mi">10</span><span class="p">:]</span> <span class="o">/</span> <span class="n">result_b</span><span class="o">.</span><span class="n">seasonal</span>

<span class="n">locale</span><span class="o">.</span><span class="n">setlocale</span><span class="p">(</span><span class="n">locale</span><span class="o">.</span><span class="n">LC_ALL</span><span class="p">,</span> <span class="s1">&#39;de_DE&#39;</span><span class="p">)</span>

<span class="n">fig</span> <span class="o">=</span> <span class="n">plt</span><span class="o">.</span><span class="n">figure</span><span class="p">(</span><span class="n">num</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span> <span class="n">figsize</span><span class="o">=</span><span class="p">(</span><span class="mf">6.75</span><span class="p">,</span> <span class="mf">3.5</span><span class="p">),</span> <span class="n">facecolor</span><span class="o">=</span><span class="s1">&#39;w&#39;</span><span class="p">,</span> <span class="n">edgecolor</span><span class="o">=</span><span class="s1">&#39;k&#39;</span><span class="p">)</span>

<span class="n">ax</span> <span class="o">=</span> <span class="n">adjusted_b</span><span class="p">[</span><span class="mi">2</span><span class="p">:]</span><span class="o">.</span><span class="n">plot</span><span class="p">()</span>
<span class="n">ax</span><span class="o">.</span><span class="n">fill_between</span><span class="p">(</span><span class="n">adjusted_b</span><span class="o">.</span><span class="n">index</span><span class="p">,</span><span class="n">adjusted_c</span><span class="p">,</span><span class="n">adjusted_d</span><span class="p">,</span><span class="n">color</span><span class="o">=</span><span class="s1">&#39;g&#39;</span><span class="p">,</span><span class="n">alpha</span><span class="o">=</span><span class="mf">0.3</span><span class="p">,</span><span class="n">lw</span><span class="o">=</span><span class="mi">0</span><span class="p">,</span><span class="n">zorder</span><span class="o">=</span><span class="mi">0</span><span class="p">)</span>
<span class="n">ax</span><span class="o">.</span><span class="n">set_xlim</span><span class="p">(</span><span class="n">right</span><span class="o">=</span><span class="n">nowcast</span><span class="o">.</span><span class="n">index</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span><span class="o">+</span><span class="n">pd</span><span class="o">.</span><span class="n">Timedelta</span><span class="p">(</span><span class="n">days</span><span class="o">=</span><span class="mi">1</span><span class="p">))</span>
<span class="c1">#ax.set_ylim(top=5000,bottom=0)</span>
<span class="n">red_patch</span> <span class="o">=</span> <span class="n">mpatches</span><span class="o">.</span><span class="n">Patch</span><span class="p">(</span><span class="n">color</span><span class="o">=</span><span class="s1">&#39;green&#39;</span><span class="p">,</span> <span class="n">alpha</span><span class="o">=</span><span class="mf">0.3</span><span class="p">,</span> <span class="n">label</span><span class="o">=</span><span class="s1">&#39;95%-Prädiktionsintervall&#39;</span><span class="p">,</span><span class="n">ec</span><span class="o">=</span><span class="kc">None</span><span class="p">)</span>
<span class="n">ax</span><span class="o">.</span><span class="n">legend</span><span class="p">(</span><span class="n">handles</span><span class="o">=</span><span class="p">[</span><span class="n">red_patch</span><span class="p">],</span><span class="n">frameon</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s2">&quot;Deutsche COVID-19 Fallzahlen nach Erkrankungsbeginn&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s2">&quot;Saisonal bereinigte Fallzahlen&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s2">&quot;Datum des Erkrankungsbeginns&quot;</span><span class="p">)</span>
<span class="c1">#ax.tick_params(axis=&#39;x&#39;, which=&#39;major&#39;, pad=-5)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">grid</span><span class="p">(</span><span class="n">axis</span> <span class="o">=</span> <span class="s1">&#39;y&#39;</span><span class="p">,</span> <span class="n">b</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">which</span><span class="o">=</span><span class="s1">&#39;major&#39;</span><span class="p">,</span> <span class="n">color</span><span class="o">=</span><span class="s1">&#39;#999999&#39;</span><span class="p">,</span> <span class="n">linestyle</span><span class="o">=</span><span class="s1">&#39;-&#39;</span><span class="p">,</span> <span class="n">alpha</span><span class="o">=</span><span class="mf">0.15</span><span class="p">,</span><span class="n">zorder</span><span class="o">=-</span><span class="mi">1</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">subplots_adjust</span><span class="p">(</span><span class="n">left</span><span class="o">=</span><span class="mf">0.2</span><span class="p">,</span> <span class="n">right</span><span class="o">=</span><span class="mf">0.9</span><span class="p">,</span> <span class="n">top</span><span class="o">=</span><span class="mf">0.9</span><span class="p">,</span> <span class="n">bottom</span><span class="o">=</span><span class="mf">0.25</span><span class="p">)</span>
<span class="n">fig</span><span class="o">.</span><span class="n">text</span><span class="p">(</span><span class="mf">0.91</span><span class="p">,</span> <span class="mf">0.08</span><span class="p">,</span> <span class="s2">&quot;Datenstand: &quot;</span> <span class="o">+</span> <span class="n">today</span> <span class="o">+</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">Datenquelle:RKI Nowcast</span><span class="se">\n</span><span class="s2">Viz: @CorneliusRoemer&quot;</span><span class="p">,</span> <span class="n">size</span><span class="o">=</span><span class="mi">5</span><span class="p">,</span> <span class="n">va</span><span class="o">=</span><span class="s2">&quot;bottom&quot;</span><span class="p">,</span> <span class="n">ha</span><span class="o">=</span><span class="s2">&quot;right&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">savefig</span><span class="p">(</span><span class="s1">&#39;CasesAll.png&#39;</span><span class="p">,</span><span class="n">dpi</span><span class="o">=</span><span class="mi">400</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt"></div>



<div class="output_svg output_subarea ">
<?xml version="1.0" encoding="utf-8" standalone="no"?>
<!DOCTYPE svg PUBLIC "-//W3C//DTD SVG 1.1//EN"
  "http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd">
<!-- Created with matplotlib (https://matplotlib.org/) -->
<svg height="236.158125pt" version="1.1" viewBox="0 0 405.588125 236.158125" width="405.588125pt" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
 <defs>
  <style type="text/css">
*{stroke-linecap:butt;stroke-linejoin:round;}
  </style>
 </defs>
 <g id="figure_1">
  <g id="patch_1">
   <path d="M 0 236.158125 
L 405.588125 236.158125 
L 405.588125 0 
L 0 0 
z
" style="fill:#ffffff;"/>
  </g>
  <g id="axes_1">
   <g id="patch_2">
    <path d="M 53.328125 186.118125 
L 393.528125 186.118125 
L 393.528125 22.318125 
L 53.328125 22.318125 
z
" style="fill:#ffffff;"/>
   </g>
   <g id="PolyCollection_1">
    <defs>
     <path d="M 71.842411 -154.8295 
L 71.842411 -152.009136 
L 74.156696 -170.000391 
L 76.470982 -186.792248 
L 78.785268 -202.511391 
L 81.099554 -201.89185 
L 83.413839 -187.26345 
L 85.728125 -186.999285 
L 88.042411 -183.175583 
L 90.356696 -196.524444 
L 92.670982 -186.63692 
L 94.985268 -174.144621 
L 97.299554 -179.752656 
L 99.613839 -156.945543 
L 101.928125 -164.401794 
L 104.242411 -162.94873 
L 106.556696 -163.078665 
L 108.870982 -169.271203 
L 111.185268 -156.176806 
L 113.499554 -160.739893 
L 115.813839 -143.7558 
L 118.128125 -154.367152 
L 120.442411 -155.000431 
L 122.756696 -152.280773 
L 125.070982 -142.244059 
L 127.385268 -137.550829 
L 129.699554 -134.254198 
L 132.013839 -129.455898 
L 134.328125 -124.080779 
L 136.642411 -125.828181 
L 138.956696 -113.60217 
L 141.270982 -111.395836 
L 143.585268 -113.100121 
L 145.899554 -97.296233 
L 148.213839 -100.723932 
L 150.528125 -99.528488 
L 152.842411 -99.134433 
L 155.156696 -94.885824 
L 157.470982 -93.781594 
L 159.785268 -91.973129 
L 162.099554 -89.619957 
L 164.413839 -85.128845 
L 166.728125 -83.290613 
L 169.042411 -85.716338 
L 171.356696 -81.180807 
L 173.670982 -80.64081 
L 175.985268 -79.106067 
L 178.299554 -77.673434 
L 180.613839 -74.423742 
L 182.928125 -72.109155 
L 185.242411 -76.372102 
L 187.556696 -72.237938 
L 189.870982 -72.501601 
L 192.185268 -74.202762 
L 194.499554 -72.335626 
L 196.813839 -70.987537 
L 199.128125 -69.163923 
L 201.442411 -69.762764 
L 203.756696 -68.417145 
L 206.070982 -67.779617 
L 208.385268 -67.719869 
L 210.699554 -66.464038 
L 213.013839 -66.150416 
L 215.328125 -65.019746 
L 217.642411 -64.463898 
L 219.956696 -68.444832 
L 222.270982 -66.940844 
L 224.585268 -63.968348 
L 226.899554 -65.472731 
L 229.213839 -62.238428 
L 231.528125 -64.550594 
L 233.842411 -60.931321 
L 236.156696 -60.443317 
L 238.470982 -60.85197 
L 240.785268 -61.993862 
L 243.099554 -61.685429 
L 245.413839 -61.233999 
L 247.728125 -61.683554 
L 250.042411 -60.646436 
L 252.356696 -59.474276 
L 254.670982 -58.894832 
L 256.985268 -58.604329 
L 259.299554 -58.203145 
L 261.613839 -61.260431 
L 263.928125 -60.22397 
L 266.242411 -59.620849 
L 268.556696 -58.560608 
L 270.870982 -58.956964 
L 273.185268 -57.485455 
L 275.499554 -60.338268 
L 277.813839 -61.630484 
L 280.128125 -61.031954 
L 282.442411 -60.36155 
L 284.756696 -60.000327 
L 287.070982 -61.131561 
L 289.385268 -61.598965 
L 291.699554 -66.15902 
L 294.013839 -78.917242 
L 296.328125 -66.844227 
L 298.642411 -64.948203 
L 300.956696 -65.537707 
L 303.270982 -64.300261 
L 305.585268 -61.993862 
L 307.899554 -61.965028 
L 310.213839 -60.969676 
L 312.528125 -61.892066 
L 314.842411 -61.301672 
L 317.156696 -61.606167 
L 319.470982 -60.727707 
L 321.785268 -60.183918 
L 324.099554 -60.694122 
L 326.413839 -61.498323 
L 328.728125 -60.09365 
L 331.042411 -59.59236 
L 333.356696 -59.391215 
L 335.670982 -59.019095 
L 337.985268 -59.558664 
L 340.299554 -58.889434 
L 342.613839 -59.092979 
L 344.928125 -58.529809 
L 347.242411 -60.56097 
L 349.556696 -61.966097 
L 351.870982 -61.721809 
L 354.185268 -61.500241 
L 356.499554 -63.337607 
L 358.813839 -63.295723 
L 361.128125 -63.977186 
L 363.442411 -62.840052 
L 365.756696 -63.54425 
L 368.070982 -63.927473 
L 370.385268 -65.745384 
L 372.699554 -64.201824 
L 375.013839 -66.784793 
L 377.328125 -66.922419 
L 379.642411 -66.856934 
L 381.956696 -65.814576 
L 384.270982 -64.300261 
L 386.585268 -67.719869 
L 388.899554 -66.489456 
L 391.213839 -62.608481 
L 391.213839 -83.252148 
L 391.213839 -83.252148 
L 388.899554 -85.883491 
L 386.585268 -79.862953 
L 384.270982 -75.142184 
L 381.956696 -74.148334 
L 379.642411 -72.953479 
L 377.328125 -72.343731 
L 375.013839 -71.621913 
L 372.699554 -68.777088 
L 370.385268 -68.970377 
L 368.070982 -66.381662 
L 365.756696 -66.257567 
L 363.442411 -65.062157 
L 361.128125 -65.69741 
L 358.813839 -65.436743 
L 356.499554 -65.040622 
L 354.185268 -63.573451 
L 351.870982 -63.58575 
L 349.556696 -63.322755 
L 347.242411 -62.013885 
L 344.928125 -59.885138 
L 342.613839 -60.520326 
L 340.299554 -60.287431 
L 337.985268 -61.072436 
L 335.670982 -60.448116 
L 333.356696 -60.77556 
L 331.042411 -61.016786 
L 328.728125 -61.553234 
L 326.413839 -62.978534 
L 324.099554 -61.965028 
L 321.785268 -61.796414 
L 319.470982 -62.249926 
L 317.156696 -63.267381 
L 314.842411 -62.783075 
L 312.528125 -63.299522 
L 310.213839 -62.555617 
L 307.899554 -63.464698 
L 305.585268 -63.639267 
L 303.270982 -66.133136 
L 300.956696 -67.171234 
L 298.642411 -66.885423 
L 296.328125 -68.694771 
L 294.013839 -81.005398 
L 291.699554 -67.811199 
L 289.385268 -63.112737 
L 287.070982 -62.65378 
L 284.756696 -61.384672 
L 282.442411 -61.871442 
L 280.128125 -62.361218 
L 277.813839 -63.031399 
L 275.499554 -61.53292 
L 273.185268 -58.867594 
L 270.870982 -60.417051 
L 268.556696 -59.806518 
L 266.242411 -60.988298 
L 263.928125 -61.422914 
L 261.613839 -62.952102 
L 259.299554 -59.499469 
L 256.985268 -59.986469 
L 254.670982 -60.323854 
L 252.356696 -60.969368 
L 250.042411 -62.127839 
L 247.728125 -62.986754 
L 245.413839 -62.687778 
L 243.099554 -62.880081 
L 240.785268 -63.540542 
L 238.470982 -62.560583 
L 236.156696 -61.883036 
L 233.842411 -62.384236 
L 231.528125 -65.879858 
L 229.213839 -63.639343 
L 226.899554 -66.997819 
L 224.585268 -66.173189 
L 222.270982 -68.649457 
L 219.956696 -70.216794 
L 217.642411 -66.287164 
L 215.328125 -66.635715 
L 213.013839 -67.789222 
L 210.699554 -68.167053 
L 208.385268 -69.760171 
L 206.070982 -69.612493 
L 203.756696 -70.133733 
L 201.442411 -71.586029 
L 199.128125 -71.014467 
L 196.813839 -73.207854 
L 194.499554 -74.47075 
L 192.185268 -76.47342 
L 189.870982 -74.769396 
L 187.556696 -74.176021 
L 185.242411 -78.309321 
L 182.928125 -73.9597 
L 180.613839 -76.485466 
L 178.299554 -79.630631 
L 175.985268 -81.442541 
L 173.670982 -82.939671 
L 171.356696 -83.312699 
L 169.042411 -88.166351 
L 166.728125 -85.584246 
L 164.413839 -87.560621 
L 162.099554 -91.831334 
L 159.785268 -94.803225 
L 157.470982 -96.422177 
L 155.156696 -97.571454 
L 152.842411 -101.812355 
L 150.528125 -101.848184 
L 148.213839 -103.367167 
L 145.899554 -99.863464 
L 143.585268 -116.325113 
L 141.270982 -114.626667 
L 138.956696 -116.177052 
L 136.642411 -128.961919 
L 134.328125 -126.895692 
L 132.013839 -132.548483 
L 129.699554 -137.075611 
L 127.385268 -140.775821 
L 125.070982 -145.785547 
L 122.756696 -155.492454 
L 120.442411 -158.533008 
L 118.128125 -158.172497 
L 115.813839 -147.218438 
L 113.499554 -163.739232 
L 111.185268 -159.829603 
L 108.870982 -172.999085 
L 106.556696 -166.401094 
L 104.242411 -166.538284 
L 101.928125 -167.216706 
L 99.613839 -160.011696 
L 97.299554 -183.387449 
L 94.985268 -177.929051 
L 92.670982 -190.209473 
L 90.356696 -199.791498 
L 88.042411 -187.021534 
L 85.728125 -190.231221 
L 83.413839 -190.699656 
L 81.099554 -205.323298 
L 78.785268 -206.394545 
L 76.470982 -190.30267 
L 74.156696 -173.018264 
L 71.842411 -154.8295 
z
" id="mee67274403"/>
    </defs>
    <g clip-path="url(#p580b4bc92d)">
     <use style="fill:#008000;fill-opacity:0.3;" x="0" xlink:href="#mee67274403" y="236.158125"/>
    </g>
   </g>
   <g id="matplotlib.axis_1">
    <g id="xtick_1">
     <g id="line2d_1">
      <defs>
       <path d="M 0 0 
L 0 3.5 
" id="mee6710a27a" style="stroke:#000000;stroke-width:0.8;"/>
      </defs>
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="53.328125" xlink:href="#mee6710a27a" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_2">
     <g id="line2d_2">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="118.128125" xlink:href="#mee6710a27a" y="186.118125"/>
      </g>
     </g>
     <g id="text_1">
      <!-- Apr -->
      <defs>
       <path d="M 34.1875 63.1875 
L 20.796875 26.90625 
L 47.609375 26.90625 
z
M 28.609375 72.90625 
L 39.796875 72.90625 
L 67.578125 0 
L 57.328125 0 
L 50.6875 18.703125 
L 17.828125 18.703125 
L 11.1875 0 
L 0.78125 0 
z
" id="DejaVuSans-65"/>
       <path d="M 18.109375 8.203125 
L 18.109375 -20.796875 
L 9.078125 -20.796875 
L 9.078125 54.6875 
L 18.109375 54.6875 
L 18.109375 46.390625 
Q 20.953125 51.265625 25.265625 53.625 
Q 29.59375 56 35.59375 56 
Q 45.5625 56 51.78125 48.09375 
Q 58.015625 40.1875 58.015625 27.296875 
Q 58.015625 14.40625 51.78125 6.484375 
Q 45.5625 -1.421875 35.59375 -1.421875 
Q 29.59375 -1.421875 25.265625 0.953125 
Q 20.953125 3.328125 18.109375 8.203125 
z
M 48.6875 27.296875 
Q 48.6875 37.203125 44.609375 42.84375 
Q 40.53125 48.484375 33.40625 48.484375 
Q 26.265625 48.484375 22.1875 42.84375 
Q 18.109375 37.203125 18.109375 27.296875 
Q 18.109375 17.390625 22.1875 11.75 
Q 26.265625 6.109375 33.40625 6.109375 
Q 40.53125 6.109375 44.609375 11.75 
Q 48.6875 17.390625 48.6875 27.296875 
z
" id="DejaVuSans-112"/>
       <path d="M 41.109375 46.296875 
Q 39.59375 47.171875 37.8125 47.578125 
Q 36.03125 48 33.890625 48 
Q 26.265625 48 22.1875 43.046875 
Q 18.109375 38.09375 18.109375 28.8125 
L 18.109375 0 
L 9.078125 0 
L 9.078125 54.6875 
L 18.109375 54.6875 
L 18.109375 46.1875 
Q 20.953125 51.171875 25.484375 53.578125 
Q 30.03125 56 36.53125 56 
Q 37.453125 56 38.578125 55.875 
Q 39.703125 55.765625 41.0625 55.515625 
z
" id="DejaVuSans-114"/>
      </defs>
      <g transform="translate(109.478125 200.716562)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-65"/>
       <use x="68.408203" xlink:href="#DejaVuSans-112"/>
       <use x="131.884766" xlink:href="#DejaVuSans-114"/>
      </g>
      <!-- 2020 -->
      <defs>
       <path d="M 19.1875 8.296875 
L 53.609375 8.296875 
L 53.609375 0 
L 7.328125 0 
L 7.328125 8.296875 
Q 12.9375 14.109375 22.625 23.890625 
Q 32.328125 33.6875 34.8125 36.53125 
Q 39.546875 41.84375 41.421875 45.53125 
Q 43.3125 49.21875 43.3125 52.78125 
Q 43.3125 58.59375 39.234375 62.25 
Q 35.15625 65.921875 28.609375 65.921875 
Q 23.96875 65.921875 18.8125 64.3125 
Q 13.671875 62.703125 7.8125 59.421875 
L 7.8125 69.390625 
Q 13.765625 71.78125 18.9375 73 
Q 24.125 74.21875 28.421875 74.21875 
Q 39.75 74.21875 46.484375 68.546875 
Q 53.21875 62.890625 53.21875 53.421875 
Q 53.21875 48.921875 51.53125 44.890625 
Q 49.859375 40.875 45.40625 35.40625 
Q 44.1875 33.984375 37.640625 27.21875 
Q 31.109375 20.453125 19.1875 8.296875 
z
" id="DejaVuSans-50"/>
       <path d="M 31.78125 66.40625 
Q 24.171875 66.40625 20.328125 58.90625 
Q 16.5 51.421875 16.5 36.375 
Q 16.5 21.390625 20.328125 13.890625 
Q 24.171875 6.390625 31.78125 6.390625 
Q 39.453125 6.390625 43.28125 13.890625 
Q 47.125 21.390625 47.125 36.375 
Q 47.125 51.421875 43.28125 58.90625 
Q 39.453125 66.40625 31.78125 66.40625 
z
M 31.78125 74.21875 
Q 44.046875 74.21875 50.515625 64.515625 
Q 56.984375 54.828125 56.984375 36.375 
Q 56.984375 17.96875 50.515625 8.265625 
Q 44.046875 -1.421875 31.78125 -1.421875 
Q 19.53125 -1.421875 13.0625 8.265625 
Q 6.59375 17.96875 6.59375 36.375 
Q 6.59375 54.828125 13.0625 64.515625 
Q 19.53125 74.21875 31.78125 74.21875 
z
" id="DejaVuSans-48"/>
      </defs>
      <g transform="translate(105.403125 211.914375)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
      </g>
     </g>
    </g>
    <g id="xtick_3">
     <g id="line2d_3">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="187.556696" xlink:href="#mee6710a27a" y="186.118125"/>
      </g>
     </g>
     <g id="text_2">
      <!-- Mai -->
      <defs>
       <path d="M 9.8125 72.90625 
L 24.515625 72.90625 
L 43.109375 23.296875 
L 61.8125 72.90625 
L 76.515625 72.90625 
L 76.515625 0 
L 66.890625 0 
L 66.890625 64.015625 
L 48.09375 14.015625 
L 38.1875 14.015625 
L 19.390625 64.015625 
L 19.390625 0 
L 9.8125 0 
z
" id="DejaVuSans-77"/>
       <path d="M 34.28125 27.484375 
Q 23.390625 27.484375 19.1875 25 
Q 14.984375 22.515625 14.984375 16.5 
Q 14.984375 11.71875 18.140625 8.90625 
Q 21.296875 6.109375 26.703125 6.109375 
Q 34.1875 6.109375 38.703125 11.40625 
Q 43.21875 16.703125 43.21875 25.484375 
L 43.21875 27.484375 
z
M 52.203125 31.203125 
L 52.203125 0 
L 43.21875 0 
L 43.21875 8.296875 
Q 40.140625 3.328125 35.546875 0.953125 
Q 30.953125 -1.421875 24.3125 -1.421875 
Q 15.921875 -1.421875 10.953125 3.296875 
Q 6 8.015625 6 15.921875 
Q 6 25.140625 12.171875 29.828125 
Q 18.359375 34.515625 30.609375 34.515625 
L 43.21875 34.515625 
L 43.21875 35.40625 
Q 43.21875 41.609375 39.140625 45 
Q 35.0625 48.390625 27.6875 48.390625 
Q 23 48.390625 18.546875 47.265625 
Q 14.109375 46.140625 10.015625 43.890625 
L 10.015625 52.203125 
Q 14.9375 54.109375 19.578125 55.046875 
Q 24.21875 56 28.609375 56 
Q 40.484375 56 46.34375 49.84375 
Q 52.203125 43.703125 52.203125 31.203125 
z
" id="DejaVuSans-97"/>
       <path d="M 9.421875 54.6875 
L 18.40625 54.6875 
L 18.40625 0 
L 9.421875 0 
z
M 9.421875 75.984375 
L 18.40625 75.984375 
L 18.40625 64.59375 
L 9.421875 64.59375 
z
" id="DejaVuSans-105"/>
      </defs>
      <g transform="translate(178.789509 200.716562)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-77"/>
       <use x="86.279297" xlink:href="#DejaVuSans-97"/>
       <use x="147.558594" xlink:href="#DejaVuSans-105"/>
      </g>
     </g>
    </g>
    <g id="xtick_4">
     <g id="line2d_4">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="259.299554" xlink:href="#mee6710a27a" y="186.118125"/>
      </g>
     </g>
     <g id="text_3">
      <!-- Jun -->
      <defs>
       <path d="M 9.8125 72.90625 
L 19.671875 72.90625 
L 19.671875 5.078125 
Q 19.671875 -8.109375 14.671875 -14.0625 
Q 9.671875 -20.015625 -1.421875 -20.015625 
L -5.171875 -20.015625 
L -5.171875 -11.71875 
L -2.09375 -11.71875 
Q 4.4375 -11.71875 7.125 -8.046875 
Q 9.8125 -4.390625 9.8125 5.078125 
z
" id="DejaVuSans-74"/>
       <path d="M 8.5 21.578125 
L 8.5 54.6875 
L 17.484375 54.6875 
L 17.484375 21.921875 
Q 17.484375 14.15625 20.5 10.265625 
Q 23.53125 6.390625 29.59375 6.390625 
Q 36.859375 6.390625 41.078125 11.03125 
Q 45.3125 15.671875 45.3125 23.6875 
L 45.3125 54.6875 
L 54.296875 54.6875 
L 54.296875 0 
L 45.3125 0 
L 45.3125 8.40625 
Q 42.046875 3.421875 37.71875 1 
Q 33.40625 -1.421875 27.6875 -1.421875 
Q 18.265625 -1.421875 13.375 4.4375 
Q 8.5 10.296875 8.5 21.578125 
z
M 31.109375 56 
z
" id="DejaVuSans-117"/>
       <path d="M 54.890625 33.015625 
L 54.890625 0 
L 45.90625 0 
L 45.90625 32.71875 
Q 45.90625 40.484375 42.875 44.328125 
Q 39.84375 48.1875 33.796875 48.1875 
Q 26.515625 48.1875 22.3125 43.546875 
Q 18.109375 38.921875 18.109375 30.90625 
L 18.109375 0 
L 9.078125 0 
L 9.078125 54.6875 
L 18.109375 54.6875 
L 18.109375 46.1875 
Q 21.34375 51.125 25.703125 53.5625 
Q 30.078125 56 35.796875 56 
Q 45.21875 56 50.046875 50.171875 
Q 54.890625 44.34375 54.890625 33.015625 
z
" id="DejaVuSans-110"/>
      </defs>
      <g transform="translate(251.487054 200.716562)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-74"/>
       <use x="29.492188" xlink:href="#DejaVuSans-117"/>
       <use x="92.871094" xlink:href="#DejaVuSans-110"/>
      </g>
     </g>
    </g>
    <g id="xtick_5">
     <g id="line2d_5">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="328.728125" xlink:href="#mee6710a27a" y="186.118125"/>
      </g>
     </g>
     <g id="text_4">
      <!-- Jul -->
      <defs>
       <path d="M 9.421875 75.984375 
L 18.40625 75.984375 
L 18.40625 0 
L 9.421875 0 
z
" id="DejaVuSans-108"/>
      </defs>
      <g transform="translate(322.695313 200.716562)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-74"/>
       <use x="29.492188" xlink:href="#DejaVuSans-117"/>
       <use x="92.871094" xlink:href="#DejaVuSans-108"/>
      </g>
     </g>
    </g>
    <g id="xtick_6">
     <g id="line2d_6">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="393.528125" xlink:href="#mee6710a27a" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_7">
     <g id="line2d_7">
      <defs>
       <path d="M 0 0 
L 0 2 
" id="mcfe8227f61" style="stroke:#000000;stroke-width:0.6;"/>
      </defs>
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="64.899554" xlink:href="#mcfe8227f61" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_8">
     <g id="line2d_8">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="81.099554" xlink:href="#mcfe8227f61" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_9">
     <g id="line2d_9">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="97.299554" xlink:href="#mcfe8227f61" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_10">
     <g id="line2d_10">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="113.499554" xlink:href="#mcfe8227f61" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_11">
     <g id="line2d_11">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="129.699554" xlink:href="#mcfe8227f61" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_12">
     <g id="line2d_12">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="145.899554" xlink:href="#mcfe8227f61" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_13">
     <g id="line2d_13">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="162.099554" xlink:href="#mcfe8227f61" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_14">
     <g id="line2d_14">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="178.299554" xlink:href="#mcfe8227f61" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_15">
     <g id="line2d_15">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="194.499554" xlink:href="#mcfe8227f61" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_16">
     <g id="line2d_16">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="210.699554" xlink:href="#mcfe8227f61" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_17">
     <g id="line2d_17">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="226.899554" xlink:href="#mcfe8227f61" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_18">
     <g id="line2d_18">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="243.099554" xlink:href="#mcfe8227f61" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_19">
     <g id="line2d_19">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="275.499554" xlink:href="#mcfe8227f61" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_20">
     <g id="line2d_20">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="291.699554" xlink:href="#mcfe8227f61" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_21">
     <g id="line2d_21">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="307.899554" xlink:href="#mcfe8227f61" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_22">
     <g id="line2d_22">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="324.099554" xlink:href="#mcfe8227f61" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_23">
     <g id="line2d_23">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="340.299554" xlink:href="#mcfe8227f61" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_24">
     <g id="line2d_24">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="356.499554" xlink:href="#mcfe8227f61" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_25">
     <g id="line2d_25">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="372.699554" xlink:href="#mcfe8227f61" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_26">
     <g id="line2d_26">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="388.899554" xlink:href="#mcfe8227f61" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="text_5">
     <!-- Datum des Erkrankungsbeginns -->
     <defs>
      <path d="M 19.671875 64.796875 
L 19.671875 8.109375 
L 31.59375 8.109375 
Q 46.6875 8.109375 53.6875 14.9375 
Q 60.6875 21.78125 60.6875 36.53125 
Q 60.6875 51.171875 53.6875 57.984375 
Q 46.6875 64.796875 31.59375 64.796875 
z
M 9.8125 72.90625 
L 30.078125 72.90625 
Q 51.265625 72.90625 61.171875 64.09375 
Q 71.09375 55.28125 71.09375 36.53125 
Q 71.09375 17.671875 61.125 8.828125 
Q 51.171875 0 30.078125 0 
L 9.8125 0 
z
" id="DejaVuSans-68"/>
      <path d="M 18.3125 70.21875 
L 18.3125 54.6875 
L 36.8125 54.6875 
L 36.8125 47.703125 
L 18.3125 47.703125 
L 18.3125 18.015625 
Q 18.3125 11.328125 20.140625 9.421875 
Q 21.96875 7.515625 27.59375 7.515625 
L 36.8125 7.515625 
L 36.8125 0 
L 27.59375 0 
Q 17.1875 0 13.234375 3.875 
Q 9.28125 7.765625 9.28125 18.015625 
L 9.28125 47.703125 
L 2.6875 47.703125 
L 2.6875 54.6875 
L 9.28125 54.6875 
L 9.28125 70.21875 
z
" id="DejaVuSans-116"/>
      <path d="M 52 44.1875 
Q 55.375 50.25 60.0625 53.125 
Q 64.75 56 71.09375 56 
Q 79.640625 56 84.28125 50.015625 
Q 88.921875 44.046875 88.921875 33.015625 
L 88.921875 0 
L 79.890625 0 
L 79.890625 32.71875 
Q 79.890625 40.578125 77.09375 44.375 
Q 74.3125 48.1875 68.609375 48.1875 
Q 61.625 48.1875 57.5625 43.546875 
Q 53.515625 38.921875 53.515625 30.90625 
L 53.515625 0 
L 44.484375 0 
L 44.484375 32.71875 
Q 44.484375 40.625 41.703125 44.40625 
Q 38.921875 48.1875 33.109375 48.1875 
Q 26.21875 48.1875 22.15625 43.53125 
Q 18.109375 38.875 18.109375 30.90625 
L 18.109375 0 
L 9.078125 0 
L 9.078125 54.6875 
L 18.109375 54.6875 
L 18.109375 46.1875 
Q 21.1875 51.21875 25.484375 53.609375 
Q 29.78125 56 35.6875 56 
Q 41.65625 56 45.828125 52.96875 
Q 50 49.953125 52 44.1875 
z
" id="DejaVuSans-109"/>
      <path id="DejaVuSans-32"/>
      <path d="M 45.40625 46.390625 
L 45.40625 75.984375 
L 54.390625 75.984375 
L 54.390625 0 
L 45.40625 0 
L 45.40625 8.203125 
Q 42.578125 3.328125 38.25 0.953125 
Q 33.9375 -1.421875 27.875 -1.421875 
Q 17.96875 -1.421875 11.734375 6.484375 
Q 5.515625 14.40625 5.515625 27.296875 
Q 5.515625 40.1875 11.734375 48.09375 
Q 17.96875 56 27.875 56 
Q 33.9375 56 38.25 53.625 
Q 42.578125 51.265625 45.40625 46.390625 
z
M 14.796875 27.296875 
Q 14.796875 17.390625 18.875 11.75 
Q 22.953125 6.109375 30.078125 6.109375 
Q 37.203125 6.109375 41.296875 11.75 
Q 45.40625 17.390625 45.40625 27.296875 
Q 45.40625 37.203125 41.296875 42.84375 
Q 37.203125 48.484375 30.078125 48.484375 
Q 22.953125 48.484375 18.875 42.84375 
Q 14.796875 37.203125 14.796875 27.296875 
z
" id="DejaVuSans-100"/>
      <path d="M 56.203125 29.59375 
L 56.203125 25.203125 
L 14.890625 25.203125 
Q 15.484375 15.921875 20.484375 11.0625 
Q 25.484375 6.203125 34.421875 6.203125 
Q 39.59375 6.203125 44.453125 7.46875 
Q 49.3125 8.734375 54.109375 11.28125 
L 54.109375 2.78125 
Q 49.265625 0.734375 44.1875 -0.34375 
Q 39.109375 -1.421875 33.890625 -1.421875 
Q 20.796875 -1.421875 13.15625 6.1875 
Q 5.515625 13.8125 5.515625 26.8125 
Q 5.515625 40.234375 12.765625 48.109375 
Q 20.015625 56 32.328125 56 
Q 43.359375 56 49.78125 48.890625 
Q 56.203125 41.796875 56.203125 29.59375 
z
M 47.21875 32.234375 
Q 47.125 39.59375 43.09375 43.984375 
Q 39.0625 48.390625 32.421875 48.390625 
Q 24.90625 48.390625 20.390625 44.140625 
Q 15.875 39.890625 15.1875 32.171875 
z
" id="DejaVuSans-101"/>
      <path d="M 44.28125 53.078125 
L 44.28125 44.578125 
Q 40.484375 46.53125 36.375 47.5 
Q 32.28125 48.484375 27.875 48.484375 
Q 21.1875 48.484375 17.84375 46.4375 
Q 14.5 44.390625 14.5 40.28125 
Q 14.5 37.15625 16.890625 35.375 
Q 19.28125 33.59375 26.515625 31.984375 
L 29.59375 31.296875 
Q 39.15625 29.25 43.1875 25.515625 
Q 47.21875 21.78125 47.21875 15.09375 
Q 47.21875 7.46875 41.1875 3.015625 
Q 35.15625 -1.421875 24.609375 -1.421875 
Q 20.21875 -1.421875 15.453125 -0.5625 
Q 10.6875 0.296875 5.421875 2 
L 5.421875 11.28125 
Q 10.40625 8.6875 15.234375 7.390625 
Q 20.0625 6.109375 24.8125 6.109375 
Q 31.15625 6.109375 34.5625 8.28125 
Q 37.984375 10.453125 37.984375 14.40625 
Q 37.984375 18.0625 35.515625 20.015625 
Q 33.0625 21.96875 24.703125 23.78125 
L 21.578125 24.515625 
Q 13.234375 26.265625 9.515625 29.90625 
Q 5.8125 33.546875 5.8125 39.890625 
Q 5.8125 47.609375 11.28125 51.796875 
Q 16.75 56 26.8125 56 
Q 31.78125 56 36.171875 55.265625 
Q 40.578125 54.546875 44.28125 53.078125 
z
" id="DejaVuSans-115"/>
      <path d="M 9.8125 72.90625 
L 55.90625 72.90625 
L 55.90625 64.59375 
L 19.671875 64.59375 
L 19.671875 43.015625 
L 54.390625 43.015625 
L 54.390625 34.71875 
L 19.671875 34.71875 
L 19.671875 8.296875 
L 56.78125 8.296875 
L 56.78125 0 
L 9.8125 0 
z
" id="DejaVuSans-69"/>
      <path d="M 9.078125 75.984375 
L 18.109375 75.984375 
L 18.109375 31.109375 
L 44.921875 54.6875 
L 56.390625 54.6875 
L 27.390625 29.109375 
L 57.625 0 
L 45.90625 0 
L 18.109375 26.703125 
L 18.109375 0 
L 9.078125 0 
z
" id="DejaVuSans-107"/>
      <path d="M 45.40625 27.984375 
Q 45.40625 37.75 41.375 43.109375 
Q 37.359375 48.484375 30.078125 48.484375 
Q 22.859375 48.484375 18.828125 43.109375 
Q 14.796875 37.75 14.796875 27.984375 
Q 14.796875 18.265625 18.828125 12.890625 
Q 22.859375 7.515625 30.078125 7.515625 
Q 37.359375 7.515625 41.375 12.890625 
Q 45.40625 18.265625 45.40625 27.984375 
z
M 54.390625 6.78125 
Q 54.390625 -7.171875 48.1875 -13.984375 
Q 42 -20.796875 29.203125 -20.796875 
Q 24.46875 -20.796875 20.265625 -20.09375 
Q 16.0625 -19.390625 12.109375 -17.921875 
L 12.109375 -9.1875 
Q 16.0625 -11.328125 19.921875 -12.34375 
Q 23.78125 -13.375 27.78125 -13.375 
Q 36.625 -13.375 41.015625 -8.765625 
Q 45.40625 -4.15625 45.40625 5.171875 
L 45.40625 9.625 
Q 42.625 4.78125 38.28125 2.390625 
Q 33.9375 0 27.875 0 
Q 17.828125 0 11.671875 7.65625 
Q 5.515625 15.328125 5.515625 27.984375 
Q 5.515625 40.671875 11.671875 48.328125 
Q 17.828125 56 27.875 56 
Q 33.9375 56 38.28125 53.609375 
Q 42.625 51.21875 45.40625 46.390625 
L 45.40625 54.6875 
L 54.390625 54.6875 
z
" id="DejaVuSans-103"/>
      <path d="M 48.6875 27.296875 
Q 48.6875 37.203125 44.609375 42.84375 
Q 40.53125 48.484375 33.40625 48.484375 
Q 26.265625 48.484375 22.1875 42.84375 
Q 18.109375 37.203125 18.109375 27.296875 
Q 18.109375 17.390625 22.1875 11.75 
Q 26.265625 6.109375 33.40625 6.109375 
Q 40.53125 6.109375 44.609375 11.75 
Q 48.6875 17.390625 48.6875 27.296875 
z
M 18.109375 46.390625 
Q 20.953125 51.265625 25.265625 53.625 
Q 29.59375 56 35.59375 56 
Q 45.5625 56 51.78125 48.09375 
Q 58.015625 40.1875 58.015625 27.296875 
Q 58.015625 14.40625 51.78125 6.484375 
Q 45.5625 -1.421875 35.59375 -1.421875 
Q 29.59375 -1.421875 25.265625 0.953125 
Q 20.953125 3.328125 18.109375 8.203125 
L 18.109375 0 
L 9.078125 0 
L 9.078125 75.984375 
L 18.109375 75.984375 
z
" id="DejaVuSans-98"/>
     </defs>
     <g transform="translate(143.317188 225.5925)scale(0.1 -0.1)">
      <use xlink:href="#DejaVuSans-68"/>
      <use x="77.001953" xlink:href="#DejaVuSans-97"/>
      <use x="138.28125" xlink:href="#DejaVuSans-116"/>
      <use x="177.490234" xlink:href="#DejaVuSans-117"/>
      <use x="240.869141" xlink:href="#DejaVuSans-109"/>
      <use x="338.28125" xlink:href="#DejaVuSans-32"/>
      <use x="370.068359" xlink:href="#DejaVuSans-100"/>
      <use x="433.544922" xlink:href="#DejaVuSans-101"/>
      <use x="495.068359" xlink:href="#DejaVuSans-115"/>
      <use x="547.167969" xlink:href="#DejaVuSans-32"/>
      <use x="578.955078" xlink:href="#DejaVuSans-69"/>
      <use x="642.138672" xlink:href="#DejaVuSans-114"/>
      <use x="683.251953" xlink:href="#DejaVuSans-107"/>
      <use x="741.162109" xlink:href="#DejaVuSans-114"/>
      <use x="782.275391" xlink:href="#DejaVuSans-97"/>
      <use x="843.554688" xlink:href="#DejaVuSans-110"/>
      <use x="906.933594" xlink:href="#DejaVuSans-107"/>
      <use x="964.796875" xlink:href="#DejaVuSans-117"/>
      <use x="1028.175781" xlink:href="#DejaVuSans-110"/>
      <use x="1091.554688" xlink:href="#DejaVuSans-103"/>
      <use x="1155.03125" xlink:href="#DejaVuSans-115"/>
      <use x="1207.130859" xlink:href="#DejaVuSans-98"/>
      <use x="1270.607422" xlink:href="#DejaVuSans-101"/>
      <use x="1332.130859" xlink:href="#DejaVuSans-103"/>
      <use x="1395.607422" xlink:href="#DejaVuSans-105"/>
      <use x="1423.390625" xlink:href="#DejaVuSans-110"/>
      <use x="1486.769531" xlink:href="#DejaVuSans-110"/>
      <use x="1550.148438" xlink:href="#DejaVuSans-115"/>
     </g>
    </g>
   </g>
   <g id="matplotlib.axis_2">
    <g id="ytick_1">
     <g id="line2d_27">
      <path clip-path="url(#p580b4bc92d)" d="M 53.328125 185.682093 
L 393.528125 185.682093 
" style="fill:none;stroke:#999999;stroke-linecap:square;stroke-opacity:0.15;stroke-width:0.8;"/>
     </g>
     <g id="line2d_28">
      <defs>
       <path d="M 0 0 
L -3.5 0 
" id="m22503e56a2" style="stroke:#000000;stroke-width:0.8;"/>
      </defs>
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="53.328125" xlink:href="#m22503e56a2" y="185.682093"/>
      </g>
     </g>
     <g id="text_6">
      <!-- 0 -->
      <g transform="translate(39.965625 189.481312)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-48"/>
      </g>
     </g>
    </g>
    <g id="ytick_2">
     <g id="line2d_29">
      <path clip-path="url(#p580b4bc92d)" d="M 53.328125 157.60787 
L 393.528125 157.60787 
" style="fill:none;stroke:#999999;stroke-linecap:square;stroke-opacity:0.15;stroke-width:0.8;"/>
     </g>
     <g id="line2d_30">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="53.328125" xlink:href="#m22503e56a2" y="157.60787"/>
      </g>
     </g>
     <g id="text_7">
      <!-- 1000 -->
      <defs>
       <path d="M 12.40625 8.296875 
L 28.515625 8.296875 
L 28.515625 63.921875 
L 10.984375 60.40625 
L 10.984375 69.390625 
L 28.421875 72.90625 
L 38.28125 72.90625 
L 38.28125 8.296875 
L 54.390625 8.296875 
L 54.390625 0 
L 12.40625 0 
z
" id="DejaVuSans-49"/>
      </defs>
      <g transform="translate(20.878125 161.407089)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-49"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-48"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
      </g>
     </g>
    </g>
    <g id="ytick_3">
     <g id="line2d_31">
      <path clip-path="url(#p580b4bc92d)" d="M 53.328125 129.533648 
L 393.528125 129.533648 
" style="fill:none;stroke:#999999;stroke-linecap:square;stroke-opacity:0.15;stroke-width:0.8;"/>
     </g>
     <g id="line2d_32">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="53.328125" xlink:href="#m22503e56a2" y="129.533648"/>
      </g>
     </g>
     <g id="text_8">
      <!-- 2000 -->
      <g transform="translate(20.878125 133.332867)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-48"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
      </g>
     </g>
    </g>
    <g id="ytick_4">
     <g id="line2d_33">
      <path clip-path="url(#p580b4bc92d)" d="M 53.328125 101.459426 
L 393.528125 101.459426 
" style="fill:none;stroke:#999999;stroke-linecap:square;stroke-opacity:0.15;stroke-width:0.8;"/>
     </g>
     <g id="line2d_34">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="53.328125" xlink:href="#m22503e56a2" y="101.459426"/>
      </g>
     </g>
     <g id="text_9">
      <!-- 3000 -->
      <defs>
       <path d="M 40.578125 39.3125 
Q 47.65625 37.796875 51.625 33 
Q 55.609375 28.21875 55.609375 21.1875 
Q 55.609375 10.40625 48.1875 4.484375 
Q 40.765625 -1.421875 27.09375 -1.421875 
Q 22.515625 -1.421875 17.65625 -0.515625 
Q 12.796875 0.390625 7.625 2.203125 
L 7.625 11.71875 
Q 11.71875 9.328125 16.59375 8.109375 
Q 21.484375 6.890625 26.8125 6.890625 
Q 36.078125 6.890625 40.9375 10.546875 
Q 45.796875 14.203125 45.796875 21.1875 
Q 45.796875 27.640625 41.28125 31.265625 
Q 36.765625 34.90625 28.71875 34.90625 
L 20.21875 34.90625 
L 20.21875 43.015625 
L 29.109375 43.015625 
Q 36.375 43.015625 40.234375 45.921875 
Q 44.09375 48.828125 44.09375 54.296875 
Q 44.09375 59.90625 40.109375 62.90625 
Q 36.140625 65.921875 28.71875 65.921875 
Q 24.65625 65.921875 20.015625 65.03125 
Q 15.375 64.15625 9.8125 62.3125 
L 9.8125 71.09375 
Q 15.4375 72.65625 20.34375 73.4375 
Q 25.25 74.21875 29.59375 74.21875 
Q 40.828125 74.21875 47.359375 69.109375 
Q 53.90625 64.015625 53.90625 55.328125 
Q 53.90625 49.265625 50.4375 45.09375 
Q 46.96875 40.921875 40.578125 39.3125 
z
" id="DejaVuSans-51"/>
      </defs>
      <g transform="translate(20.878125 105.258644)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-51"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-48"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
      </g>
     </g>
    </g>
    <g id="ytick_5">
     <g id="line2d_35">
      <path clip-path="url(#p580b4bc92d)" d="M 53.328125 73.385203 
L 393.528125 73.385203 
" style="fill:none;stroke:#999999;stroke-linecap:square;stroke-opacity:0.15;stroke-width:0.8;"/>
     </g>
     <g id="line2d_36">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="53.328125" xlink:href="#m22503e56a2" y="73.385203"/>
      </g>
     </g>
     <g id="text_10">
      <!-- 4000 -->
      <defs>
       <path d="M 37.796875 64.3125 
L 12.890625 25.390625 
L 37.796875 25.390625 
z
M 35.203125 72.90625 
L 47.609375 72.90625 
L 47.609375 25.390625 
L 58.015625 25.390625 
L 58.015625 17.1875 
L 47.609375 17.1875 
L 47.609375 0 
L 37.796875 0 
L 37.796875 17.1875 
L 4.890625 17.1875 
L 4.890625 26.703125 
z
" id="DejaVuSans-52"/>
      </defs>
      <g transform="translate(20.878125 77.184422)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-52"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-48"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
      </g>
     </g>
    </g>
    <g id="ytick_6">
     <g id="line2d_37">
      <path clip-path="url(#p580b4bc92d)" d="M 53.328125 45.310981 
L 393.528125 45.310981 
" style="fill:none;stroke:#999999;stroke-linecap:square;stroke-opacity:0.15;stroke-width:0.8;"/>
     </g>
     <g id="line2d_38">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="53.328125" xlink:href="#m22503e56a2" y="45.310981"/>
      </g>
     </g>
     <g id="text_11">
      <!-- 5000 -->
      <defs>
       <path d="M 10.796875 72.90625 
L 49.515625 72.90625 
L 49.515625 64.59375 
L 19.828125 64.59375 
L 19.828125 46.734375 
Q 21.96875 47.46875 24.109375 47.828125 
Q 26.265625 48.1875 28.421875 48.1875 
Q 40.625 48.1875 47.75 41.5 
Q 54.890625 34.8125 54.890625 23.390625 
Q 54.890625 11.625 47.5625 5.09375 
Q 40.234375 -1.421875 26.90625 -1.421875 
Q 22.3125 -1.421875 17.546875 -0.640625 
Q 12.796875 0.140625 7.71875 1.703125 
L 7.71875 11.625 
Q 12.109375 9.234375 16.796875 8.0625 
Q 21.484375 6.890625 26.703125 6.890625 
Q 35.15625 6.890625 40.078125 11.328125 
Q 45.015625 15.765625 45.015625 23.390625 
Q 45.015625 31 40.078125 35.4375 
Q 35.15625 39.890625 26.703125 39.890625 
Q 22.75 39.890625 18.8125 39.015625 
Q 14.890625 38.140625 10.796875 36.28125 
z
" id="DejaVuSans-53"/>
      </defs>
      <g transform="translate(20.878125 49.110199)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-53"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-48"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
      </g>
     </g>
    </g>
    <g id="text_12">
     <!-- Saisonal bereinigte Fallzahlen -->
     <defs>
      <path d="M 53.515625 70.515625 
L 53.515625 60.890625 
Q 47.90625 63.578125 42.921875 64.890625 
Q 37.9375 66.21875 33.296875 66.21875 
Q 25.25 66.21875 20.875 63.09375 
Q 16.5 59.96875 16.5 54.203125 
Q 16.5 49.359375 19.40625 46.890625 
Q 22.3125 44.4375 30.421875 42.921875 
L 36.375 41.703125 
Q 47.40625 39.59375 52.65625 34.296875 
Q 57.90625 29 57.90625 20.125 
Q 57.90625 9.515625 50.796875 4.046875 
Q 43.703125 -1.421875 29.984375 -1.421875 
Q 24.8125 -1.421875 18.96875 -0.25 
Q 13.140625 0.921875 6.890625 3.21875 
L 6.890625 13.375 
Q 12.890625 10.015625 18.65625 8.296875 
Q 24.421875 6.59375 29.984375 6.59375 
Q 38.421875 6.59375 43.015625 9.90625 
Q 47.609375 13.234375 47.609375 19.390625 
Q 47.609375 24.75 44.3125 27.78125 
Q 41.015625 30.8125 33.5 32.328125 
L 27.484375 33.5 
Q 16.453125 35.6875 11.515625 40.375 
Q 6.59375 45.0625 6.59375 53.421875 
Q 6.59375 63.09375 13.40625 68.65625 
Q 20.21875 74.21875 32.171875 74.21875 
Q 37.3125 74.21875 42.625 73.28125 
Q 47.953125 72.359375 53.515625 70.515625 
z
" id="DejaVuSans-83"/>
      <path d="M 30.609375 48.390625 
Q 23.390625 48.390625 19.1875 42.75 
Q 14.984375 37.109375 14.984375 27.296875 
Q 14.984375 17.484375 19.15625 11.84375 
Q 23.34375 6.203125 30.609375 6.203125 
Q 37.796875 6.203125 41.984375 11.859375 
Q 46.1875 17.53125 46.1875 27.296875 
Q 46.1875 37.015625 41.984375 42.703125 
Q 37.796875 48.390625 30.609375 48.390625 
z
M 30.609375 56 
Q 42.328125 56 49.015625 48.375 
Q 55.71875 40.765625 55.71875 27.296875 
Q 55.71875 13.875 49.015625 6.21875 
Q 42.328125 -1.421875 30.609375 -1.421875 
Q 18.84375 -1.421875 12.171875 6.21875 
Q 5.515625 13.875 5.515625 27.296875 
Q 5.515625 40.765625 12.171875 48.375 
Q 18.84375 56 30.609375 56 
z
" id="DejaVuSans-111"/>
      <path d="M 9.8125 72.90625 
L 51.703125 72.90625 
L 51.703125 64.59375 
L 19.671875 64.59375 
L 19.671875 43.109375 
L 48.578125 43.109375 
L 48.578125 34.8125 
L 19.671875 34.8125 
L 19.671875 0 
L 9.8125 0 
z
" id="DejaVuSans-70"/>
      <path d="M 5.515625 54.6875 
L 48.1875 54.6875 
L 48.1875 46.484375 
L 14.40625 7.171875 
L 48.1875 7.171875 
L 48.1875 0 
L 4.296875 0 
L 4.296875 8.203125 
L 38.09375 47.515625 
L 5.515625 47.515625 
z
" id="DejaVuSans-122"/>
      <path d="M 54.890625 33.015625 
L 54.890625 0 
L 45.90625 0 
L 45.90625 32.71875 
Q 45.90625 40.484375 42.875 44.328125 
Q 39.84375 48.1875 33.796875 48.1875 
Q 26.515625 48.1875 22.3125 43.546875 
Q 18.109375 38.921875 18.109375 30.90625 
L 18.109375 0 
L 9.078125 0 
L 9.078125 75.984375 
L 18.109375 75.984375 
L 18.109375 46.1875 
Q 21.34375 51.125 25.703125 53.5625 
Q 30.078125 56 35.796875 56 
Q 45.21875 56 50.046875 50.171875 
Q 54.890625 44.34375 54.890625 33.015625 
z
" id="DejaVuSans-104"/>
     </defs>
     <g transform="translate(14.798438 179.050937)rotate(-90)scale(0.1 -0.1)">
      <use xlink:href="#DejaVuSans-83"/>
      <use x="63.476562" xlink:href="#DejaVuSans-97"/>
      <use x="124.755859" xlink:href="#DejaVuSans-105"/>
      <use x="152.539062" xlink:href="#DejaVuSans-115"/>
      <use x="204.638672" xlink:href="#DejaVuSans-111"/>
      <use x="265.820312" xlink:href="#DejaVuSans-110"/>
      <use x="329.199219" xlink:href="#DejaVuSans-97"/>
      <use x="390.478516" xlink:href="#DejaVuSans-108"/>
      <use x="418.261719" xlink:href="#DejaVuSans-32"/>
      <use x="450.048828" xlink:href="#DejaVuSans-98"/>
      <use x="513.525391" xlink:href="#DejaVuSans-101"/>
      <use x="575.048828" xlink:href="#DejaVuSans-114"/>
      <use x="616.130859" xlink:href="#DejaVuSans-101"/>
      <use x="677.654297" xlink:href="#DejaVuSans-105"/>
      <use x="705.4375" xlink:href="#DejaVuSans-110"/>
      <use x="768.816406" xlink:href="#DejaVuSans-105"/>
      <use x="796.599609" xlink:href="#DejaVuSans-103"/>
      <use x="860.076172" xlink:href="#DejaVuSans-116"/>
      <use x="899.285156" xlink:href="#DejaVuSans-101"/>
      <use x="960.808594" xlink:href="#DejaVuSans-32"/>
      <use x="992.595703" xlink:href="#DejaVuSans-70"/>
      <use x="1049.974609" xlink:href="#DejaVuSans-97"/>
      <use x="1111.253906" xlink:href="#DejaVuSans-108"/>
      <use x="1139.037109" xlink:href="#DejaVuSans-108"/>
      <use x="1166.820312" xlink:href="#DejaVuSans-122"/>
      <use x="1219.310547" xlink:href="#DejaVuSans-97"/>
      <use x="1280.589844" xlink:href="#DejaVuSans-104"/>
      <use x="1343.96875" xlink:href="#DejaVuSans-108"/>
      <use x="1371.751953" xlink:href="#DejaVuSans-101"/>
      <use x="1433.275391" xlink:href="#DejaVuSans-110"/>
     </g>
    </g>
   </g>
   <g id="line2d_39">
    <path clip-path="url(#p580b4bc92d)" d="M 53.328125 174.005419 
L 55.642411 171.295388 
L 57.956696 164.695421 
L 60.270982 155.020264 
L 62.585268 141.618165 
L 64.899554 134.134119 
L 69.528125 101.312912 
L 74.156696 64.634954 
L 76.470982 47.564067 
L 78.785268 31.836789 
L 81.099554 32.537842 
L 83.413839 47.176572 
L 85.728125 47.595 
L 88.042411 50.845903 
L 90.356696 37.972467 
L 92.670982 47.626199 
L 94.985268 60.104835 
L 97.299554 54.575363 
L 99.613839 77.705938 
L 101.928125 70.322811 
L 104.242411 71.500084 
L 106.556696 71.445932 
L 108.870982 65.054047 
L 111.185268 78.204283 
L 113.499554 73.994817 
L 115.813839 90.842816 
L 118.128125 79.992557 
L 120.442411 79.30594 
L 122.756696 82.188451 
L 125.070982 92.019059 
L 127.385268 96.928984 
L 129.699554 100.556766 
L 132.013839 105.116286 
L 134.328125 110.826273 
L 136.642411 108.734586 
L 138.956696 121.25467 
L 141.270982 123.146873 
L 143.585268 121.215152 
L 145.899554 137.540149 
L 148.213839 134.218305 
L 150.528125 135.430693 
L 152.842411 135.684731 
L 155.156696 139.94333 
L 157.470982 141.040707 
L 159.785268 142.671224 
L 162.099554 145.546861 
L 164.413839 149.892689 
L 166.728125 151.720696 
L 169.042411 149.387712 
L 171.356696 153.869842 
L 173.670982 154.367885 
L 175.985268 155.933183 
L 178.299554 157.645892 
L 180.613839 160.650656 
L 182.928125 163.110665 
L 185.242411 158.874391 
L 187.556696 162.951146 
L 189.870982 162.569225 
L 192.185268 160.671947 
L 194.499554 162.932864 
L 196.813839 163.981132 
L 199.128125 166.13409 
L 201.442411 165.569194 
L 203.756696 166.827312 
L 206.070982 167.446537 
L 208.385268 167.418105 
L 210.699554 168.880707 
L 213.013839 169.24117 
L 215.328125 170.356459 
L 217.642411 170.754106 
L 219.956696 166.882686 
L 222.270982 168.409573 
L 224.585268 171.136719 
L 226.899554 169.973687 
L 229.213839 173.232455 
L 231.528125 170.955931 
L 233.842411 174.571568 
L 236.156696 175.050322 
L 238.470982 174.467381 
L 240.785268 173.440285 
L 245.413839 174.18402 
L 247.728125 173.796907 
L 250.042411 174.799476 
L 252.356696 175.96399 
L 254.670982 176.610913 
L 259.299554 177.294109 
L 261.613839 174.078291 
L 263.928125 175.334683 
L 266.242411 175.88204 
L 268.556696 176.960718 
L 270.870982 176.455585 
L 273.185268 177.948693 
L 275.499554 175.158986 
L 277.813839 173.893264 
L 282.442411 175.11285 
L 284.756696 175.493313 
L 287.070982 174.312053 
L 289.385268 173.900998 
L 291.699554 169.287397 
L 294.013839 155.998562 
L 296.328125 168.245274 
L 298.642411 170.326778 
L 300.956696 169.789811 
L 303.270982 171.019091 
L 305.585268 173.374469 
L 307.899554 173.557643 
L 310.213839 174.369047 
L 312.528125 173.510203 
L 314.842411 174.172729 
L 317.156696 173.721351 
L 319.470982 174.715907 
L 321.785268 175.283138 
L 324.099554 174.853968 
L 326.413839 173.972561 
L 328.728125 175.282555 
L 331.042411 175.88204 
L 333.356696 176.047051 
L 335.670982 176.486651 
L 337.985268 175.809667 
L 340.299554 176.531565 
L 342.613839 176.351473 
L 344.928125 176.950652 
L 347.242411 174.91343 
L 349.556696 173.499856 
L 351.870982 173.442214 
L 354.185268 173.571917 
L 356.499554 171.956301 
L 358.813839 171.725811 
L 361.128125 171.294763 
L 363.442411 172.263997 
L 365.756696 171.201843 
L 368.070982 171.050156 
L 370.385268 168.833153 
L 372.699554 169.490742 
L 375.013839 167.153015 
L 377.328125 166.498986 
L 379.642411 166.42385 
L 381.956696 165.996705 
L 384.270982 166.110713 
L 386.585268 162.67934 
L 388.899554 160.238542 
L 391.213839 163.003135 
L 391.213839 163.003135 
" style="fill:none;stroke:#1f77b4;stroke-linecap:square;stroke-width:1.5;"/>
   </g>
   <g id="patch_3">
    <path d="M 53.328125 186.118125 
L 53.328125 22.318125 
" style="fill:none;stroke:#000000;stroke-linecap:square;stroke-linejoin:miter;stroke-width:0.8;"/>
   </g>
   <g id="patch_4">
    <path d="M 393.528125 186.118125 
L 393.528125 22.318125 
" style="fill:none;stroke:#000000;stroke-linecap:square;stroke-linejoin:miter;stroke-width:0.8;"/>
   </g>
   <g id="patch_5">
    <path d="M 53.328125 186.118125 
L 393.528125 186.118125 
" style="fill:none;stroke:#000000;stroke-linecap:square;stroke-linejoin:miter;stroke-width:0.8;"/>
   </g>
   <g id="patch_6">
    <path d="M 53.328125 22.318125 
L 393.528125 22.318125 
" style="fill:none;stroke:#000000;stroke-linecap:square;stroke-linejoin:miter;stroke-width:0.8;"/>
   </g>
   <g id="text_13">
    <!-- Deutsche COVID-19 Fallzahlen nach Erkrankungsbeginn -->
    <defs>
     <path d="M 48.78125 52.59375 
L 48.78125 44.1875 
Q 44.96875 46.296875 41.140625 47.34375 
Q 37.3125 48.390625 33.40625 48.390625 
Q 24.65625 48.390625 19.8125 42.84375 
Q 14.984375 37.3125 14.984375 27.296875 
Q 14.984375 17.28125 19.8125 11.734375 
Q 24.65625 6.203125 33.40625 6.203125 
Q 37.3125 6.203125 41.140625 7.25 
Q 44.96875 8.296875 48.78125 10.40625 
L 48.78125 2.09375 
Q 45.015625 0.34375 40.984375 -0.53125 
Q 36.96875 -1.421875 32.421875 -1.421875 
Q 20.0625 -1.421875 12.78125 6.34375 
Q 5.515625 14.109375 5.515625 27.296875 
Q 5.515625 40.671875 12.859375 48.328125 
Q 20.21875 56 33.015625 56 
Q 37.15625 56 41.109375 55.140625 
Q 45.0625 54.296875 48.78125 52.59375 
z
" id="DejaVuSans-99"/>
     <path d="M 64.40625 67.28125 
L 64.40625 56.890625 
Q 59.421875 61.53125 53.78125 63.8125 
Q 48.140625 66.109375 41.796875 66.109375 
Q 29.296875 66.109375 22.65625 58.46875 
Q 16.015625 50.828125 16.015625 36.375 
Q 16.015625 21.96875 22.65625 14.328125 
Q 29.296875 6.6875 41.796875 6.6875 
Q 48.140625 6.6875 53.78125 8.984375 
Q 59.421875 11.28125 64.40625 15.921875 
L 64.40625 5.609375 
Q 59.234375 2.09375 53.4375 0.328125 
Q 47.65625 -1.421875 41.21875 -1.421875 
Q 24.65625 -1.421875 15.125 8.703125 
Q 5.609375 18.84375 5.609375 36.375 
Q 5.609375 53.953125 15.125 64.078125 
Q 24.65625 74.21875 41.21875 74.21875 
Q 47.75 74.21875 53.53125 72.484375 
Q 59.328125 70.75 64.40625 67.28125 
z
" id="DejaVuSans-67"/>
     <path d="M 39.40625 66.21875 
Q 28.65625 66.21875 22.328125 58.203125 
Q 16.015625 50.203125 16.015625 36.375 
Q 16.015625 22.609375 22.328125 14.59375 
Q 28.65625 6.59375 39.40625 6.59375 
Q 50.140625 6.59375 56.421875 14.59375 
Q 62.703125 22.609375 62.703125 36.375 
Q 62.703125 50.203125 56.421875 58.203125 
Q 50.140625 66.21875 39.40625 66.21875 
z
M 39.40625 74.21875 
Q 54.734375 74.21875 63.90625 63.9375 
Q 73.09375 53.65625 73.09375 36.375 
Q 73.09375 19.140625 63.90625 8.859375 
Q 54.734375 -1.421875 39.40625 -1.421875 
Q 24.03125 -1.421875 14.8125 8.828125 
Q 5.609375 19.09375 5.609375 36.375 
Q 5.609375 53.65625 14.8125 63.9375 
Q 24.03125 74.21875 39.40625 74.21875 
z
" id="DejaVuSans-79"/>
     <path d="M 28.609375 0 
L 0.78125 72.90625 
L 11.078125 72.90625 
L 34.1875 11.53125 
L 57.328125 72.90625 
L 67.578125 72.90625 
L 39.796875 0 
z
" id="DejaVuSans-86"/>
     <path d="M 9.8125 72.90625 
L 19.671875 72.90625 
L 19.671875 0 
L 9.8125 0 
z
" id="DejaVuSans-73"/>
     <path d="M 4.890625 31.390625 
L 31.203125 31.390625 
L 31.203125 23.390625 
L 4.890625 23.390625 
z
" id="DejaVuSans-45"/>
     <path d="M 10.984375 1.515625 
L 10.984375 10.5 
Q 14.703125 8.734375 18.5 7.8125 
Q 22.3125 6.890625 25.984375 6.890625 
Q 35.75 6.890625 40.890625 13.453125 
Q 46.046875 20.015625 46.78125 33.40625 
Q 43.953125 29.203125 39.59375 26.953125 
Q 35.25 24.703125 29.984375 24.703125 
Q 19.046875 24.703125 12.671875 31.3125 
Q 6.296875 37.9375 6.296875 49.421875 
Q 6.296875 60.640625 12.9375 67.421875 
Q 19.578125 74.21875 30.609375 74.21875 
Q 43.265625 74.21875 49.921875 64.515625 
Q 56.59375 54.828125 56.59375 36.375 
Q 56.59375 19.140625 48.40625 8.859375 
Q 40.234375 -1.421875 26.421875 -1.421875 
Q 22.703125 -1.421875 18.890625 -0.6875 
Q 15.09375 0.046875 10.984375 1.515625 
z
M 30.609375 32.421875 
Q 37.25 32.421875 41.125 36.953125 
Q 45.015625 41.5 45.015625 49.421875 
Q 45.015625 57.28125 41.125 61.84375 
Q 37.25 66.40625 30.609375 66.40625 
Q 23.96875 66.40625 20.09375 61.84375 
Q 16.21875 57.28125 16.21875 49.421875 
Q 16.21875 41.5 20.09375 36.953125 
Q 23.96875 32.421875 30.609375 32.421875 
z
" id="DejaVuSans-57"/>
    </defs>
    <g transform="translate(55.114063 16.318125)scale(0.12 -0.12)">
     <use xlink:href="#DejaVuSans-68"/>
     <use x="77.001953" xlink:href="#DejaVuSans-101"/>
     <use x="138.525391" xlink:href="#DejaVuSans-117"/>
     <use x="201.904297" xlink:href="#DejaVuSans-116"/>
     <use x="241.113281" xlink:href="#DejaVuSans-115"/>
     <use x="293.212891" xlink:href="#DejaVuSans-99"/>
     <use x="348.193359" xlink:href="#DejaVuSans-104"/>
     <use x="411.572266" xlink:href="#DejaVuSans-101"/>
     <use x="473.095703" xlink:href="#DejaVuSans-32"/>
     <use x="504.882812" xlink:href="#DejaVuSans-67"/>
     <use x="574.707031" xlink:href="#DejaVuSans-79"/>
     <use x="653.402344" xlink:href="#DejaVuSans-86"/>
     <use x="721.810547" xlink:href="#DejaVuSans-73"/>
     <use x="751.302734" xlink:href="#DejaVuSans-68"/>
     <use x="828.304688" xlink:href="#DejaVuSans-45"/>
     <use x="864.388672" xlink:href="#DejaVuSans-49"/>
     <use x="928.011719" xlink:href="#DejaVuSans-57"/>
     <use x="991.634766" xlink:href="#DejaVuSans-32"/>
     <use x="1023.421875" xlink:href="#DejaVuSans-70"/>
     <use x="1080.800781" xlink:href="#DejaVuSans-97"/>
     <use x="1142.080078" xlink:href="#DejaVuSans-108"/>
     <use x="1169.863281" xlink:href="#DejaVuSans-108"/>
     <use x="1197.646484" xlink:href="#DejaVuSans-122"/>
     <use x="1250.136719" xlink:href="#DejaVuSans-97"/>
     <use x="1311.416016" xlink:href="#DejaVuSans-104"/>
     <use x="1374.794922" xlink:href="#DejaVuSans-108"/>
     <use x="1402.578125" xlink:href="#DejaVuSans-101"/>
     <use x="1464.101562" xlink:href="#DejaVuSans-110"/>
     <use x="1527.480469" xlink:href="#DejaVuSans-32"/>
     <use x="1559.267578" xlink:href="#DejaVuSans-110"/>
     <use x="1622.646484" xlink:href="#DejaVuSans-97"/>
     <use x="1683.925781" xlink:href="#DejaVuSans-99"/>
     <use x="1738.90625" xlink:href="#DejaVuSans-104"/>
     <use x="1802.285156" xlink:href="#DejaVuSans-32"/>
     <use x="1834.072266" xlink:href="#DejaVuSans-69"/>
     <use x="1897.255859" xlink:href="#DejaVuSans-114"/>
     <use x="1938.369141" xlink:href="#DejaVuSans-107"/>
     <use x="1996.279297" xlink:href="#DejaVuSans-114"/>
     <use x="2037.392578" xlink:href="#DejaVuSans-97"/>
     <use x="2098.671875" xlink:href="#DejaVuSans-110"/>
     <use x="2162.050781" xlink:href="#DejaVuSans-107"/>
     <use x="2219.914062" xlink:href="#DejaVuSans-117"/>
     <use x="2283.292969" xlink:href="#DejaVuSans-110"/>
     <use x="2346.671875" xlink:href="#DejaVuSans-103"/>
     <use x="2410.148438" xlink:href="#DejaVuSans-115"/>
     <use x="2462.248047" xlink:href="#DejaVuSans-98"/>
     <use x="2525.724609" xlink:href="#DejaVuSans-101"/>
     <use x="2587.248047" xlink:href="#DejaVuSans-103"/>
     <use x="2650.724609" xlink:href="#DejaVuSans-105"/>
     <use x="2678.507812" xlink:href="#DejaVuSans-110"/>
     <use x="2741.886719" xlink:href="#DejaVuSans-110"/>
    </g>
   </g>
   <g id="legend_1">
    <g id="patch_7">
     <path d="M 234.242188 38.916562 
L 254.242188 38.916562 
L 254.242188 31.916562 
L 234.242188 31.916562 
z
" style="fill:#008000;opacity:0.3;"/>
    </g>
    <g id="text_14">
     <!-- 95%-Prädiktionsintervall -->
     <defs>
      <path d="M 72.703125 32.078125 
Q 68.453125 32.078125 66.03125 28.46875 
Q 63.625 24.859375 63.625 18.40625 
Q 63.625 12.0625 66.03125 8.421875 
Q 68.453125 4.78125 72.703125 4.78125 
Q 76.859375 4.78125 79.265625 8.421875 
Q 81.6875 12.0625 81.6875 18.40625 
Q 81.6875 24.8125 79.265625 28.4375 
Q 76.859375 32.078125 72.703125 32.078125 
z
M 72.703125 38.28125 
Q 80.421875 38.28125 84.953125 32.90625 
Q 89.5 27.546875 89.5 18.40625 
Q 89.5 9.28125 84.9375 3.921875 
Q 80.375 -1.421875 72.703125 -1.421875 
Q 64.890625 -1.421875 60.34375 3.921875 
Q 55.8125 9.28125 55.8125 18.40625 
Q 55.8125 27.59375 60.375 32.9375 
Q 64.9375 38.28125 72.703125 38.28125 
z
M 22.3125 68.015625 
Q 18.109375 68.015625 15.6875 64.375 
Q 13.28125 60.75 13.28125 54.390625 
Q 13.28125 47.953125 15.671875 44.328125 
Q 18.0625 40.71875 22.3125 40.71875 
Q 26.5625 40.71875 28.96875 44.328125 
Q 31.390625 47.953125 31.390625 54.390625 
Q 31.390625 60.6875 28.953125 64.34375 
Q 26.515625 68.015625 22.3125 68.015625 
z
M 66.40625 74.21875 
L 74.21875 74.21875 
L 28.609375 -1.421875 
L 20.796875 -1.421875 
z
M 22.3125 74.21875 
Q 30.03125 74.21875 34.609375 68.875 
Q 39.203125 63.53125 39.203125 54.390625 
Q 39.203125 45.171875 34.640625 39.84375 
Q 30.078125 34.515625 22.3125 34.515625 
Q 14.546875 34.515625 10.03125 39.859375 
Q 5.515625 45.21875 5.515625 54.390625 
Q 5.515625 63.484375 10.046875 68.84375 
Q 14.59375 74.21875 22.3125 74.21875 
z
" id="DejaVuSans-37"/>
      <path d="M 19.671875 64.796875 
L 19.671875 37.40625 
L 32.078125 37.40625 
Q 38.96875 37.40625 42.71875 40.96875 
Q 46.484375 44.53125 46.484375 51.125 
Q 46.484375 57.671875 42.71875 61.234375 
Q 38.96875 64.796875 32.078125 64.796875 
z
M 9.8125 72.90625 
L 32.078125 72.90625 
Q 44.34375 72.90625 50.609375 67.359375 
Q 56.890625 61.8125 56.890625 51.125 
Q 56.890625 40.328125 50.609375 34.8125 
Q 44.34375 29.296875 32.078125 29.296875 
L 19.671875 29.296875 
L 19.671875 0 
L 9.8125 0 
z
" id="DejaVuSans-80"/>
      <path d="M 34.28125 27.484375 
Q 23.390625 27.484375 19.1875 25 
Q 14.984375 22.515625 14.984375 16.5 
Q 14.984375 11.71875 18.140625 8.90625 
Q 21.296875 6.109375 26.703125 6.109375 
Q 34.1875 6.109375 38.703125 11.40625 
Q 43.21875 16.703125 43.21875 25.484375 
L 43.21875 27.484375 
z
M 52.203125 31.203125 
L 52.203125 0 
L 43.21875 0 
L 43.21875 8.296875 
Q 40.140625 3.328125 35.546875 0.953125 
Q 30.953125 -1.421875 24.3125 -1.421875 
Q 15.921875 -1.421875 10.953125 3.296875 
Q 6 8.015625 6 15.921875 
Q 6 25.140625 12.171875 29.828125 
Q 18.359375 34.515625 30.609375 34.515625 
L 43.21875 34.515625 
L 43.21875 35.40625 
Q 43.21875 41.609375 39.140625 45 
Q 35.0625 48.390625 27.6875 48.390625 
Q 23 48.390625 18.546875 47.265625 
Q 14.109375 46.140625 10.015625 43.890625 
L 10.015625 52.203125 
Q 14.9375 54.109375 19.578125 55.046875 
Q 24.21875 56 28.609375 56 
Q 40.484375 56 46.34375 49.84375 
Q 52.203125 43.703125 52.203125 31.203125 
z
M 33.59375 75.78125 
L 43.5 75.78125 
L 43.5 65.921875 
L 33.59375 65.921875 
z
M 14.5 75.78125 
L 24.421875 75.78125 
L 24.421875 65.921875 
L 14.5 65.921875 
z
" id="DejaVuSans-228"/>
      <path d="M 2.984375 54.6875 
L 12.5 54.6875 
L 29.59375 8.796875 
L 46.6875 54.6875 
L 56.203125 54.6875 
L 35.6875 0 
L 23.484375 0 
z
" id="DejaVuSans-118"/>
     </defs>
     <g transform="translate(262.242188 38.916562)scale(0.1 -0.1)">
      <use xlink:href="#DejaVuSans-57"/>
      <use x="63.623047" xlink:href="#DejaVuSans-53"/>
      <use x="127.246094" xlink:href="#DejaVuSans-37"/>
      <use x="222.265625" xlink:href="#DejaVuSans-45"/>
      <use x="258.349609" xlink:href="#DejaVuSans-80"/>
      <use x="318.636719" xlink:href="#DejaVuSans-114"/>
      <use x="359.75" xlink:href="#DejaVuSans-228"/>
      <use x="421.029297" xlink:href="#DejaVuSans-100"/>
      <use x="484.505859" xlink:href="#DejaVuSans-105"/>
      <use x="512.289062" xlink:href="#DejaVuSans-107"/>
      <use x="570.199219" xlink:href="#DejaVuSans-116"/>
      <use x="609.408203" xlink:href="#DejaVuSans-105"/>
      <use x="637.191406" xlink:href="#DejaVuSans-111"/>
      <use x="698.373047" xlink:href="#DejaVuSans-110"/>
      <use x="761.751953" xlink:href="#DejaVuSans-115"/>
      <use x="813.851562" xlink:href="#DejaVuSans-105"/>
      <use x="841.634766" xlink:href="#DejaVuSans-110"/>
      <use x="905.013672" xlink:href="#DejaVuSans-116"/>
      <use x="944.222656" xlink:href="#DejaVuSans-101"/>
      <use x="1005.746094" xlink:href="#DejaVuSans-114"/>
      <use x="1046.859375" xlink:href="#DejaVuSans-118"/>
      <use x="1106.039062" xlink:href="#DejaVuSans-97"/>
      <use x="1167.318359" xlink:href="#DejaVuSans-108"/>
      <use x="1195.101562" xlink:href="#DejaVuSans-108"/>
     </g>
    </g>
   </g>
  </g>
  <g id="text_15">
   <!-- Datenstand: 1. August 2020 -->
   <defs>
    <path d="M 11.71875 12.40625 
L 22.015625 12.40625 
L 22.015625 0 
L 11.71875 0 
z
M 11.71875 51.703125 
L 22.015625 51.703125 
L 22.015625 39.3125 
L 11.71875 39.3125 
z
" id="DejaVuSans-58"/>
    <path d="M 10.6875 12.40625 
L 21 12.40625 
L 21 0 
L 10.6875 0 
z
" id="DejaVuSans-46"/>
   </defs>
   <g transform="translate(327.852969 216.720469)scale(0.05 -0.05)">
    <use xlink:href="#DejaVuSans-68"/>
    <use x="77.001953" xlink:href="#DejaVuSans-97"/>
    <use x="138.28125" xlink:href="#DejaVuSans-116"/>
    <use x="177.490234" xlink:href="#DejaVuSans-101"/>
    <use x="239.013672" xlink:href="#DejaVuSans-110"/>
    <use x="302.392578" xlink:href="#DejaVuSans-115"/>
    <use x="354.492188" xlink:href="#DejaVuSans-116"/>
    <use x="393.701172" xlink:href="#DejaVuSans-97"/>
    <use x="454.980469" xlink:href="#DejaVuSans-110"/>
    <use x="518.359375" xlink:href="#DejaVuSans-100"/>
    <use x="581.835938" xlink:href="#DejaVuSans-58"/>
    <use x="615.527344" xlink:href="#DejaVuSans-32"/>
    <use x="647.314453" xlink:href="#DejaVuSans-49"/>
    <use x="710.9375" xlink:href="#DejaVuSans-46"/>
    <use x="742.724609" xlink:href="#DejaVuSans-32"/>
    <use x="774.511719" xlink:href="#DejaVuSans-65"/>
    <use x="842.919922" xlink:href="#DejaVuSans-117"/>
    <use x="906.298828" xlink:href="#DejaVuSans-103"/>
    <use x="969.775391" xlink:href="#DejaVuSans-117"/>
    <use x="1033.154297" xlink:href="#DejaVuSans-115"/>
    <use x="1085.253906" xlink:href="#DejaVuSans-116"/>
    <use x="1124.462891" xlink:href="#DejaVuSans-32"/>
    <use x="1156.25" xlink:href="#DejaVuSans-50"/>
    <use x="1219.873047" xlink:href="#DejaVuSans-48"/>
    <use x="1283.496094" xlink:href="#DejaVuSans-50"/>
    <use x="1347.119141" xlink:href="#DejaVuSans-48"/>
   </g>
   <!-- Datenquelle:RKI Nowcast -->
   <defs>
    <path d="M 14.796875 27.296875 
Q 14.796875 17.390625 18.875 11.75 
Q 22.953125 6.109375 30.078125 6.109375 
Q 37.203125 6.109375 41.296875 11.75 
Q 45.40625 17.390625 45.40625 27.296875 
Q 45.40625 37.203125 41.296875 42.84375 
Q 37.203125 48.484375 30.078125 48.484375 
Q 22.953125 48.484375 18.875 42.84375 
Q 14.796875 37.203125 14.796875 27.296875 
z
M 45.40625 8.203125 
Q 42.578125 3.328125 38.25 0.953125 
Q 33.9375 -1.421875 27.875 -1.421875 
Q 17.96875 -1.421875 11.734375 6.484375 
Q 5.515625 14.40625 5.515625 27.296875 
Q 5.515625 40.1875 11.734375 48.09375 
Q 17.96875 56 27.875 56 
Q 33.9375 56 38.25 53.625 
Q 42.578125 51.265625 45.40625 46.390625 
L 45.40625 54.6875 
L 54.390625 54.6875 
L 54.390625 -20.796875 
L 45.40625 -20.796875 
z
" id="DejaVuSans-113"/>
    <path d="M 44.390625 34.1875 
Q 47.5625 33.109375 50.5625 29.59375 
Q 53.5625 26.078125 56.59375 19.921875 
L 66.609375 0 
L 56 0 
L 46.6875 18.703125 
Q 43.0625 26.03125 39.671875 28.421875 
Q 36.28125 30.8125 30.421875 30.8125 
L 19.671875 30.8125 
L 19.671875 0 
L 9.8125 0 
L 9.8125 72.90625 
L 32.078125 72.90625 
Q 44.578125 72.90625 50.734375 67.671875 
Q 56.890625 62.453125 56.890625 51.90625 
Q 56.890625 45.015625 53.6875 40.46875 
Q 50.484375 35.9375 44.390625 34.1875 
z
M 19.671875 64.796875 
L 19.671875 38.921875 
L 32.078125 38.921875 
Q 39.203125 38.921875 42.84375 42.21875 
Q 46.484375 45.515625 46.484375 51.90625 
Q 46.484375 58.296875 42.84375 61.546875 
Q 39.203125 64.796875 32.078125 64.796875 
z
" id="DejaVuSans-82"/>
    <path d="M 9.8125 72.90625 
L 19.671875 72.90625 
L 19.671875 42.09375 
L 52.390625 72.90625 
L 65.09375 72.90625 
L 28.90625 38.921875 
L 67.671875 0 
L 54.6875 0 
L 19.671875 35.109375 
L 19.671875 0 
L 9.8125 0 
z
" id="DejaVuSans-75"/>
    <path d="M 9.8125 72.90625 
L 23.09375 72.90625 
L 55.421875 11.921875 
L 55.421875 72.90625 
L 64.984375 72.90625 
L 64.984375 0 
L 51.703125 0 
L 19.390625 60.984375 
L 19.390625 0 
L 9.8125 0 
z
" id="DejaVuSans-78"/>
    <path d="M 4.203125 54.6875 
L 13.1875 54.6875 
L 24.421875 12.015625 
L 35.59375 54.6875 
L 46.1875 54.6875 
L 57.421875 12.015625 
L 68.609375 54.6875 
L 77.59375 54.6875 
L 63.28125 0 
L 52.6875 0 
L 40.921875 44.828125 
L 29.109375 0 
L 18.5 0 
z
" id="DejaVuSans-119"/>
   </defs>
   <g transform="translate(335.225625 222.319375)scale(0.05 -0.05)">
    <use xlink:href="#DejaVuSans-68"/>
    <use x="77.001953" xlink:href="#DejaVuSans-97"/>
    <use x="138.28125" xlink:href="#DejaVuSans-116"/>
    <use x="177.490234" xlink:href="#DejaVuSans-101"/>
    <use x="239.013672" xlink:href="#DejaVuSans-110"/>
    <use x="302.392578" xlink:href="#DejaVuSans-113"/>
    <use x="365.869141" xlink:href="#DejaVuSans-117"/>
    <use x="429.248047" xlink:href="#DejaVuSans-101"/>
    <use x="490.771484" xlink:href="#DejaVuSans-108"/>
    <use x="518.554688" xlink:href="#DejaVuSans-108"/>
    <use x="546.337891" xlink:href="#DejaVuSans-101"/>
    <use x="607.861328" xlink:href="#DejaVuSans-58"/>
    <use x="641.552734" xlink:href="#DejaVuSans-82"/>
    <use x="711.035156" xlink:href="#DejaVuSans-75"/>
    <use x="776.611328" xlink:href="#DejaVuSans-73"/>
    <use x="806.103516" xlink:href="#DejaVuSans-32"/>
    <use x="837.890625" xlink:href="#DejaVuSans-78"/>
    <use x="912.695312" xlink:href="#DejaVuSans-111"/>
    <use x="973.876953" xlink:href="#DejaVuSans-119"/>
    <use x="1055.664062" xlink:href="#DejaVuSans-99"/>
    <use x="1110.644531" xlink:href="#DejaVuSans-97"/>
    <use x="1171.923828" xlink:href="#DejaVuSans-115"/>
    <use x="1224.023438" xlink:href="#DejaVuSans-116"/>
   </g>
   <!-- Viz: @CorneliusRoemer -->
   <defs>
    <path d="M 37.203125 26.21875 
Q 37.203125 19.234375 40.671875 15.25 
Q 44.140625 11.28125 50.203125 11.28125 
Q 56.203125 11.28125 59.640625 15.28125 
Q 63.09375 19.28125 63.09375 26.21875 
Q 63.09375 33.0625 59.578125 37.078125 
Q 56.0625 41.109375 50.09375 41.109375 
Q 44.1875 41.109375 40.6875 37.109375 
Q 37.203125 33.109375 37.203125 26.21875 
z
M 63.8125 11.625 
Q 60.890625 7.859375 57.109375 6.078125 
Q 53.328125 4.296875 48.296875 4.296875 
Q 39.890625 4.296875 34.640625 10.375 
Q 29.390625 16.453125 29.390625 26.21875 
Q 29.390625 35.984375 34.65625 42.078125 
Q 39.9375 48.1875 48.296875 48.1875 
Q 53.328125 48.1875 57.125 46.359375 
Q 60.9375 44.53125 63.8125 40.828125 
L 63.8125 47.21875 
L 70.796875 47.21875 
L 70.796875 11.28125 
Q 77.9375 12.359375 81.953125 17.796875 
Q 85.984375 23.25 85.984375 31.890625 
Q 85.984375 37.109375 84.4375 41.703125 
Q 82.90625 46.296875 79.78125 50.203125 
Q 74.703125 56.59375 67.40625 59.984375 
Q 60.109375 63.375 51.515625 63.375 
Q 45.515625 63.375 39.984375 61.78125 
Q 34.46875 60.203125 29.78125 57.078125 
Q 22.125 52.09375 17.796875 44.015625 
Q 13.484375 35.9375 13.484375 26.515625 
Q 13.484375 18.75 16.28125 11.953125 
Q 19.09375 5.171875 24.421875 0 
Q 29.546875 -5.078125 36.28125 -7.734375 
Q 43.015625 -10.40625 50.6875 -10.40625 
Q 56.984375 -10.40625 63.0625 -8.28125 
Q 69.140625 -6.15625 74.21875 -2.203125 
L 78.609375 -7.625 
Q 72.515625 -12.359375 65.3125 -14.875 
Q 58.109375 -17.390625 50.6875 -17.390625 
Q 41.65625 -17.390625 33.640625 -14.1875 
Q 25.640625 -10.984375 19.390625 -4.890625 
Q 13.140625 1.21875 9.859375 9.25 
Q 6.59375 17.28125 6.59375 26.515625 
Q 6.59375 35.40625 9.90625 43.453125 
Q 13.234375 51.515625 19.390625 57.625 
Q 25.6875 63.8125 33.9375 67.109375 
Q 42.1875 70.40625 51.421875 70.40625 
Q 61.765625 70.40625 70.625 66.15625 
Q 79.5 61.921875 85.5 54.109375 
Q 89.15625 49.3125 91.078125 43.703125 
Q 93.015625 38.09375 93.015625 32.078125 
Q 93.015625 19.234375 85.25 11.8125 
Q 77.484375 4.390625 63.8125 4.109375 
z
" id="DejaVuSans-64"/>
   </defs>
   <g transform="translate(339.670937 227.918281)scale(0.05 -0.05)">
    <use xlink:href="#DejaVuSans-86"/>
    <use x="68.376953" xlink:href="#DejaVuSans-105"/>
    <use x="96.160156" xlink:href="#DejaVuSans-122"/>
    <use x="148.650391" xlink:href="#DejaVuSans-58"/>
    <use x="182.341797" xlink:href="#DejaVuSans-32"/>
    <use x="214.128906" xlink:href="#DejaVuSans-64"/>
    <use x="314.128906" xlink:href="#DejaVuSans-67"/>
    <use x="383.953125" xlink:href="#DejaVuSans-111"/>
    <use x="445.134766" xlink:href="#DejaVuSans-114"/>
    <use x="486.232422" xlink:href="#DejaVuSans-110"/>
    <use x="549.611328" xlink:href="#DejaVuSans-101"/>
    <use x="611.134766" xlink:href="#DejaVuSans-108"/>
    <use x="638.917969" xlink:href="#DejaVuSans-105"/>
    <use x="666.701172" xlink:href="#DejaVuSans-117"/>
    <use x="730.080078" xlink:href="#DejaVuSans-115"/>
    <use x="782.179688" xlink:href="#DejaVuSans-82"/>
    <use x="851.599609" xlink:href="#DejaVuSans-111"/>
    <use x="912.78125" xlink:href="#DejaVuSans-101"/>
    <use x="974.304688" xlink:href="#DejaVuSans-109"/>
    <use x="1071.716797" xlink:href="#DejaVuSans-101"/>
    <use x="1133.240234" xlink:href="#DejaVuSans-114"/>
   </g>
  </g>
 </g>
 <defs>
  <clipPath id="p580b4bc92d">
   <rect height="163.8" width="340.2" x="53.328125" y="22.318125"/>
  </clipPath>
 </defs>
</svg>

</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[82]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">start</span><span class="o">=</span><span class="mi">15</span>
<span class="n">locale</span><span class="o">.</span><span class="n">setlocale</span><span class="p">(</span><span class="n">locale</span><span class="o">.</span><span class="n">LC_ALL</span><span class="p">,</span> <span class="s1">&#39;de_DE&#39;</span><span class="p">)</span>
<span class="n">locale</span><span class="o">.</span><span class="n">setlocale</span><span class="p">(</span><span class="n">locale</span><span class="o">.</span><span class="n">LC_NUMERIC</span><span class="p">,</span> <span class="s1">&#39;de_DE&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">rcParams</span><span class="p">[</span><span class="s1">&#39;axes.formatter.use_locale&#39;</span><span class="p">]</span> <span class="o">=</span> <span class="kc">True</span>
<span class="n">fig</span> <span class="o">=</span> <span class="n">plt</span><span class="o">.</span><span class="n">figure</span><span class="p">(</span><span class="n">num</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span> <span class="n">figsize</span><span class="o">=</span><span class="p">(</span><span class="mi">7</span><span class="p">,</span> <span class="mf">3.5</span><span class="p">),</span> <span class="n">facecolor</span><span class="o">=</span><span class="s1">&#39;w&#39;</span><span class="p">,</span> <span class="n">edgecolor</span><span class="o">=</span><span class="s1">&#39;k&#39;</span><span class="p">)</span>
<span class="n">ax</span> <span class="o">=</span> <span class="n">nowcast</span><span class="o">.</span><span class="n">k</span><span class="p">[</span><span class="n">start</span><span class="p">:</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span><span class="o">.</span><span class="n">plot</span><span class="p">(</span><span class="n">zorder</span><span class="o">=</span><span class="mi">1</span><span class="p">)</span>
<span class="n">ax</span><span class="o">.</span><span class="n">fill_between</span><span class="p">(</span><span class="n">nowcast</span><span class="o">.</span><span class="n">index</span><span class="p">[</span><span class="n">start</span><span class="p">:</span><span class="o">-</span><span class="mi">1</span><span class="p">],</span><span class="n">nowcast</span><span class="o">.</span><span class="n">l</span><span class="p">[</span><span class="n">start</span><span class="p">:</span><span class="o">-</span><span class="mi">1</span><span class="p">],</span><span class="n">nowcast</span><span class="o">.</span><span class="n">m</span><span class="p">[</span><span class="n">start</span><span class="p">:</span><span class="o">-</span><span class="mi">1</span><span class="p">],</span><span class="n">color</span><span class="o">=</span><span class="s1">&#39;g&#39;</span><span class="p">,</span><span class="n">alpha</span><span class="o">=</span><span class="mf">0.3</span><span class="p">,</span><span class="n">lw</span><span class="o">=</span><span class="mi">0</span><span class="p">,</span><span class="n">zorder</span><span class="o">=</span><span class="mi">0</span><span class="p">)</span>
<span class="n">ax</span><span class="o">.</span><span class="n">set_xlim</span><span class="p">(</span><span class="n">right</span><span class="o">=</span><span class="n">nowcast</span><span class="o">.</span><span class="n">index</span><span class="p">[</span><span class="o">-</span><span class="mi">2</span><span class="p">]</span><span class="o">+</span><span class="n">pd</span><span class="o">.</span><span class="n">Timedelta</span><span class="p">(</span><span class="n">days</span><span class="o">=</span><span class="mi">1</span><span class="p">))</span>
<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s2">&quot;7-Tage Reproduktionszahl im Zeitverlauf (Deutschland)&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s2">&quot;7-Tage R&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s2">&quot;Datum des Erkrankungsbeginns&quot;</span><span class="p">,</span><span class="n">labelpad</span><span class="o">=</span><span class="mi">0</span><span class="p">)</span>
<span class="n">red_patch</span> <span class="o">=</span> <span class="n">mpatches</span><span class="o">.</span><span class="n">Patch</span><span class="p">(</span><span class="n">color</span><span class="o">=</span><span class="s1">&#39;green&#39;</span><span class="p">,</span> <span class="n">alpha</span><span class="o">=</span><span class="mf">0.3</span><span class="p">,</span> <span class="n">label</span><span class="o">=</span><span class="s1">&#39;95%-Prädiktionsintervall&#39;</span><span class="p">,</span><span class="n">ec</span><span class="o">=</span><span class="kc">None</span><span class="p">)</span>
<span class="n">ax</span><span class="o">.</span><span class="n">legend</span><span class="p">(</span><span class="n">handles</span><span class="o">=</span><span class="p">[</span><span class="n">red_patch</span><span class="p">],</span><span class="n">frameon</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
<span class="n">ax</span><span class="o">.</span><span class="n">axhline</span><span class="p">(</span><span class="mi">1</span><span class="p">,</span><span class="n">c</span><span class="o">=</span><span class="s1">&#39;black&#39;</span><span class="p">,</span><span class="n">ls</span><span class="o">=</span><span class="s1">&#39;:&#39;</span><span class="p">,</span><span class="n">alpha</span><span class="o">=</span><span class="mf">0.3</span><span class="p">)</span>
<span class="c1">#ax.tick_params(axis=&#39;x&#39;, which=&#39;major&#39;, pad=-10)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">grid</span><span class="p">(</span><span class="n">axis</span> <span class="o">=</span> <span class="s1">&#39;y&#39;</span><span class="p">,</span> <span class="n">b</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">which</span><span class="o">=</span><span class="s1">&#39;major&#39;</span><span class="p">,</span> <span class="n">color</span><span class="o">=</span><span class="s1">&#39;#999999&#39;</span><span class="p">,</span> <span class="n">linestyle</span><span class="o">=</span><span class="s1">&#39;-&#39;</span><span class="p">,</span> <span class="n">alpha</span><span class="o">=</span><span class="mf">0.15</span><span class="p">,</span><span class="n">zorder</span><span class="o">=-</span><span class="mi">1</span><span class="p">)</span>
<span class="n">fig</span><span class="o">.</span><span class="n">text</span><span class="p">(</span><span class="mf">0.91</span><span class="p">,</span> <span class="mf">0.04</span><span class="p">,</span> <span class="s2">&quot;Datenstand: &quot;</span> <span class="o">+</span> <span class="n">today</span> <span class="o">+</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">Datenquelle: RKI Nowcast</span><span class="se">\n</span><span class="s2">Viz: @CorneliusRoemer&quot;</span><span class="p">,</span> <span class="n">size</span><span class="o">=</span><span class="mi">6</span><span class="p">,</span> <span class="n">va</span><span class="o">=</span><span class="s2">&quot;bottom&quot;</span><span class="p">,</span> <span class="n">ha</span><span class="o">=</span><span class="s2">&quot;right&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">subplots_adjust</span><span class="p">(</span><span class="n">left</span><span class="o">=</span><span class="mf">0.15</span><span class="p">,</span> <span class="n">right</span><span class="o">=</span><span class="mf">0.9</span><span class="p">,</span> <span class="n">top</span><span class="o">=</span><span class="mf">0.9</span><span class="p">,</span> <span class="n">bottom</span><span class="o">=</span><span class="mf">0.23</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">savefig</span><span class="p">(</span><span class="s1">&#39;7rNear.png&#39;</span><span class="p">,</span><span class="n">dpi</span><span class="o">=</span><span class="mi">400</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt"></div>



<div class="output_svg output_subarea ">
<?xml version="1.0" encoding="utf-8" standalone="no"?>
<!DOCTYPE svg PUBLIC "-//W3C//DTD SVG 1.1//EN"
  "http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd">
<!-- Created with matplotlib (https://matplotlib.org/) -->
<svg height="246.238125pt" version="1.1" viewBox="0 0 434.02125 246.238125" width="434.02125pt" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
 <defs>
  <style type="text/css">
*{stroke-linecap:butt;stroke-linejoin:round;}
  </style>
 </defs>
 <g id="figure_1">
  <g id="patch_1">
   <path d="M 0 246.238125 
L 434.02125 246.238125 
L 434.02125 0 
L 0 0 
z
" style="fill:#ffffff;"/>
  </g>
  <g id="axes_1">
   <g id="patch_2">
    <path d="M 43.78125 191.158125 
L 421.78125 191.158125 
L 421.78125 22.318125 
L 43.78125 22.318125 
z
" style="fill:#ffffff;"/>
   </g>
   <g id="PolyCollection_1">
    <defs>
     <path d="M 43.78125 -216.245455 
L 43.78125 -212.675899 
L 46.623355 -184.11945 
L 49.465461 -155.563002 
L 52.307566 -137.715222 
L 55.149671 -119.867442 
L 57.991776 -109.158774 
L 60.833882 -100.234884 
L 63.675987 -94.88055 
L 66.518092 -94.88055 
L 69.360197 -93.095772 
L 72.202303 -94.88055 
L 75.044408 -96.665328 
L 77.886513 -96.665328 
L 80.728618 -100.234884 
L 83.570724 -100.234884 
L 86.412829 -102.019662 
L 89.254934 -103.80444 
L 92.097039 -102.019662 
L 94.939145 -100.234884 
L 97.78125 -94.88055 
L 100.623355 -93.095772 
L 103.465461 -89.526216 
L 106.307566 -85.95666 
L 109.149671 -82.387104 
L 111.991776 -78.817548 
L 114.833882 -80.602326 
L 117.675987 -75.247992 
L 120.518092 -75.247992 
L 123.360197 -73.463214 
L 126.202303 -69.893658 
L 129.044408 -73.463214 
L 131.886513 -77.03277 
L 134.728618 -78.817548 
L 137.570724 -84.171882 
L 140.412829 -84.171882 
L 143.254934 -82.387104 
L 146.097039 -82.387104 
L 148.939145 -78.817548 
L 151.78125 -78.817548 
L 154.623355 -80.602326 
L 157.465461 -80.602326 
L 160.307566 -80.602326 
L 163.149671 -78.817548 
L 165.991776 -78.817548 
L 168.833882 -78.817548 
L 171.675987 -80.602326 
L 174.518092 -85.95666 
L 177.360197 -87.741438 
L 180.202303 -93.095772 
L 183.044408 -94.88055 
L 185.886513 -91.310994 
L 188.728618 -93.095772 
L 191.570724 -93.095772 
L 194.412829 -89.526216 
L 197.254934 -87.741438 
L 200.097039 -85.95666 
L 202.939145 -84.171882 
L 205.78125 -84.171882 
L 208.623355 -91.310994 
L 211.465461 -96.665328 
L 214.307566 -98.450106 
L 217.149671 -103.80444 
L 219.991776 -96.665328 
L 222.833882 -96.665328 
L 225.675987 -96.665328 
L 228.518092 -84.171882 
L 231.360197 -82.387104 
L 234.202303 -78.817548 
L 237.044408 -77.03277 
L 239.886513 -87.741438 
L 242.728618 -91.310994 
L 245.570724 -93.095772 
L 248.412829 -100.234884 
L 251.254934 -96.665328 
L 254.097039 -96.665328 
L 256.939145 -89.526216 
L 259.78125 -91.310994 
L 262.623355 -91.310994 
L 265.465461 -94.88055 
L 268.307566 -100.234884 
L 271.149671 -100.234884 
L 273.991776 -103.80444 
L 276.833882 -110.943552 
L 279.675987 -114.513108 
L 282.518092 -116.297886 
L 285.360197 -121.65222 
L 288.202303 -118.082664 
L 291.044408 -121.65222 
L 293.886513 -128.791332 
L 296.728618 -143.069556 
L 299.570724 -185.904228 
L 302.412829 -194.828118 
L 305.254934 -193.04334 
L 308.097039 -185.904228 
L 310.939145 -144.854334 
L 313.78125 -134.145666 
L 316.623355 -118.082664 
L 319.465461 -80.602326 
L 322.307566 -69.893658 
L 325.149671 -62.754545 
L 327.991776 -62.754545 
L 330.833882 -80.602326 
L 333.675987 -85.95666 
L 336.518092 -89.526216 
L 339.360197 -98.450106 
L 342.202303 -100.234884 
L 345.044408 -100.234884 
L 347.886513 -96.665328 
L 350.728618 -93.095772 
L 353.570724 -96.665328 
L 356.412829 -94.88055 
L 359.254934 -94.88055 
L 362.097039 -93.095772 
L 364.939145 -96.665328 
L 367.78125 -107.373996 
L 370.623355 -121.65222 
L 373.465461 -130.57611 
L 376.307566 -141.284778 
L 379.149671 -146.639112 
L 381.991776 -153.778224 
L 384.833882 -153.778224 
L 387.675987 -144.854334 
L 390.518092 -137.715222 
L 393.360197 -130.57611 
L 396.202303 -130.57611 
L 399.044408 -132.360888 
L 401.886513 -135.930444 
L 404.728618 -135.930444 
L 407.570724 -139.5 
L 410.412829 -135.930444 
L 413.254934 -130.57611 
L 416.097039 -130.57611 
L 418.939145 -127.006554 
L 418.939145 -175.19556 
L 418.939145 -175.19556 
L 416.097039 -171.626004 
L 413.254934 -162.702114 
L 410.412829 -162.702114 
L 407.570724 -162.702114 
L 404.728618 -157.34778 
L 401.886513 -153.778224 
L 399.044408 -148.42389 
L 396.202303 -143.069556 
L 393.360197 -143.069556 
L 390.518092 -148.42389 
L 387.675987 -157.34778 
L 384.833882 -166.27167 
L 381.991776 -164.486892 
L 379.149671 -159.132558 
L 376.307566 -153.778224 
L 373.465461 -143.069556 
L 370.623355 -130.57611 
L 367.78125 -118.082664 
L 364.939145 -107.373996 
L 362.097039 -103.80444 
L 359.254934 -103.80444 
L 356.412829 -103.80444 
L 353.570724 -103.80444 
L 350.728618 -102.019662 
L 347.886513 -105.589218 
L 345.044408 -109.158774 
L 342.202303 -109.158774 
L 339.360197 -105.589218 
L 336.518092 -96.665328 
L 333.675987 -94.88055 
L 330.833882 -87.741438 
L 327.991776 -68.108879 
L 325.149671 -68.108879 
L 322.307566 -75.247992 
L 319.465461 -87.741438 
L 316.623355 -125.221776 
L 313.78125 -141.284778 
L 310.939145 -153.778224 
L 308.097039 -196.612896 
L 305.254934 -205.536786 
L 302.412829 -207.321564 
L 299.570724 -196.612896 
L 296.728618 -153.778224 
L 293.886513 -139.5 
L 291.044408 -132.360888 
L 288.202303 -128.791332 
L 285.360197 -130.57611 
L 282.518092 -125.221776 
L 279.675987 -123.436998 
L 276.833882 -119.867442 
L 273.991776 -110.943552 
L 271.149671 -109.158774 
L 268.307566 -109.158774 
L 265.465461 -103.80444 
L 262.623355 -98.450106 
L 259.78125 -98.450106 
L 256.939145 -96.665328 
L 254.097039 -105.589218 
L 251.254934 -105.589218 
L 248.412829 -107.373996 
L 245.570724 -100.234884 
L 242.728618 -98.450106 
L 239.886513 -93.095772 
L 237.044408 -84.171882 
L 234.202303 -85.95666 
L 231.360197 -87.741438 
L 228.518092 -91.310994 
L 225.675987 -102.019662 
L 222.833882 -103.80444 
L 219.991776 -103.80444 
L 217.149671 -110.943552 
L 214.307566 -105.589218 
L 211.465461 -102.019662 
L 208.623355 -96.665328 
L 205.78125 -89.526216 
L 202.939145 -89.526216 
L 200.097039 -89.526216 
L 197.254934 -93.095772 
L 194.412829 -93.095772 
L 191.570724 -96.665328 
L 188.728618 -98.450106 
L 185.886513 -98.450106 
L 183.044408 -100.234884 
L 180.202303 -96.665328 
L 177.360197 -93.095772 
L 174.518092 -89.526216 
L 171.675987 -84.171882 
L 168.833882 -82.387104 
L 165.991776 -82.387104 
L 163.149671 -82.387104 
L 160.307566 -84.171882 
L 157.465461 -84.171882 
L 154.623355 -84.171882 
L 151.78125 -82.387104 
L 148.939145 -82.387104 
L 146.097039 -85.95666 
L 143.254934 -84.171882 
L 140.412829 -87.741438 
L 137.570724 -87.741438 
L 134.728618 -82.387104 
L 131.886513 -80.602326 
L 129.044408 -77.03277 
L 126.202303 -71.678436 
L 123.360197 -75.247992 
L 120.518092 -77.03277 
L 117.675987 -77.03277 
L 114.833882 -82.387104 
L 111.991776 -80.602326 
L 109.149671 -84.171882 
L 106.307566 -87.741438 
L 103.465461 -93.095772 
L 100.623355 -94.88055 
L 97.78125 -96.665328 
L 94.939145 -102.019662 
L 92.097039 -103.80444 
L 89.254934 -105.589218 
L 86.412829 -103.80444 
L 83.570724 -102.019662 
L 80.728618 -102.019662 
L 77.886513 -98.450106 
L 75.044408 -98.450106 
L 72.202303 -96.665328 
L 69.360197 -94.88055 
L 66.518092 -96.665328 
L 63.675987 -96.665328 
L 60.833882 -100.234884 
L 57.991776 -110.943552 
L 55.149671 -121.65222 
L 52.307566 -139.5 
L 49.465461 -157.34778 
L 46.623355 -185.904228 
L 43.78125 -216.245455 
z
" id="m6796423f72"/>
    </defs>
    <g clip-path="url(#p16756ab622)">
     <use style="fill:#008000;fill-opacity:0.3;" x="0" xlink:href="#m6796423f72" y="246.238125"/>
    </g>
   </g>
   <g id="line2d_1">
    <path clip-path="url(#p16756ab622)" d="M 43.78125 31.777448 
L 46.623355 62.118675 
L 49.465461 88.890345 
L 52.307566 108.522903 
L 55.149671 124.585905 
L 60.833882 146.003241 
L 63.675987 149.572797 
L 66.518092 149.572797 
L 69.360197 153.142353 
L 72.202303 149.572797 
L 77.886513 149.572797 
L 80.728618 146.003241 
L 83.570724 144.218463 
L 86.412829 144.218463 
L 89.254934 140.648907 
L 92.097039 144.218463 
L 94.939145 146.003241 
L 97.78125 151.357575 
L 100.623355 151.357575 
L 109.149671 162.066243 
L 111.991776 167.420577 
L 114.833882 165.635799 
L 117.675987 169.205355 
L 120.518092 169.205355 
L 123.360197 170.990133 
L 126.202303 174.559689 
L 131.886513 167.420577 
L 134.728618 165.635799 
L 137.570724 160.281465 
L 140.412829 160.281465 
L 143.254934 162.066243 
L 146.097039 162.066243 
L 148.939145 165.635799 
L 151.78125 165.635799 
L 154.623355 162.066243 
L 157.465461 163.851021 
L 160.307566 163.851021 
L 163.149671 165.635799 
L 168.833882 165.635799 
L 171.675987 163.851021 
L 174.518092 158.496687 
L 177.360197 156.711909 
L 180.202303 151.357575 
L 183.044408 147.788019 
L 185.886513 151.357575 
L 188.728618 149.572797 
L 191.570724 151.357575 
L 194.412829 154.927131 
L 197.254934 154.927131 
L 200.097039 158.496687 
L 202.939145 158.496687 
L 205.78125 160.281465 
L 208.623355 151.357575 
L 211.465461 146.003241 
L 214.307566 144.218463 
L 217.149671 138.864129 
L 219.991776 146.003241 
L 222.833882 146.003241 
L 225.675987 147.788019 
L 228.518092 158.496687 
L 231.360197 162.066243 
L 237.044408 165.635799 
L 239.886513 154.927131 
L 242.728618 151.357575 
L 245.570724 149.572797 
L 248.412829 142.433685 
L 254.097039 146.003241 
L 256.939145 153.142353 
L 259.78125 151.357575 
L 262.623355 151.357575 
L 265.465461 147.788019 
L 268.307566 140.648907 
L 271.149671 140.648907 
L 273.991776 138.864129 
L 276.833882 129.940239 
L 279.675987 126.370683 
L 282.518092 124.585905 
L 285.360197 121.016349 
L 288.202303 122.801127 
L 291.044408 119.231571 
L 293.886513 112.092459 
L 296.728618 97.814235 
L 299.570724 54.979563 
L 302.412829 46.055673 
L 305.254934 46.055673 
L 308.097039 54.979563 
L 310.939145 96.029457 
L 313.78125 108.522903 
L 316.623355 124.585905 
L 319.465461 162.066243 
L 322.307566 174.559689 
L 325.149671 179.914024 
L 327.991776 181.698802 
L 330.833882 162.066243 
L 333.675987 156.711909 
L 336.518092 153.142353 
L 339.360197 144.218463 
L 342.202303 142.433685 
L 345.044408 142.433685 
L 347.886513 144.218463 
L 350.728618 149.572797 
L 353.570724 146.003241 
L 356.412829 146.003241 
L 359.254934 147.788019 
L 362.097039 147.788019 
L 364.939145 144.218463 
L 367.78125 133.509795 
L 370.623355 119.231571 
L 376.307566 97.814235 
L 379.149671 94.244679 
L 381.991776 87.105567 
L 384.833882 87.105567 
L 387.675987 96.029457 
L 393.360197 110.307681 
L 396.202303 110.307681 
L 399.044408 104.953347 
L 401.886513 101.383791 
L 404.728618 99.599013 
L 407.570724 96.029457 
L 413.254934 99.599013 
L 416.097039 94.244679 
L 418.939145 96.029457 
L 418.939145 96.029457 
" style="fill:none;stroke:#1f77b4;stroke-linecap:square;stroke-width:1.5;"/>
   </g>
   <g id="matplotlib.axis_1">
    <g id="xtick_1">
     <g id="line2d_2">
      <defs>
       <path d="M 0 0 
L 0 3.5 
" id="mc3d69031e6" style="stroke:#000000;stroke-width:0.8;"/>
      </defs>
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="43.78125" xlink:href="#mc3d69031e6" y="191.158125"/>
      </g>
     </g>
    </g>
    <g id="xtick_2">
     <g id="line2d_3">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="86.412829" xlink:href="#mc3d69031e6" y="191.158125"/>
      </g>
     </g>
     <g id="text_1">
      <!-- Apr -->
      <defs>
       <path d="M 34.1875 63.1875 
L 20.796875 26.90625 
L 47.609375 26.90625 
z
M 28.609375 72.90625 
L 39.796875 72.90625 
L 67.578125 0 
L 57.328125 0 
L 50.6875 18.703125 
L 17.828125 18.703125 
L 11.1875 0 
L 0.78125 0 
z
" id="DejaVuSans-65"/>
       <path d="M 18.109375 8.203125 
L 18.109375 -20.796875 
L 9.078125 -20.796875 
L 9.078125 54.6875 
L 18.109375 54.6875 
L 18.109375 46.390625 
Q 20.953125 51.265625 25.265625 53.625 
Q 29.59375 56 35.59375 56 
Q 45.5625 56 51.78125 48.09375 
Q 58.015625 40.1875 58.015625 27.296875 
Q 58.015625 14.40625 51.78125 6.484375 
Q 45.5625 -1.421875 35.59375 -1.421875 
Q 29.59375 -1.421875 25.265625 0.953125 
Q 20.953125 3.328125 18.109375 8.203125 
z
M 48.6875 27.296875 
Q 48.6875 37.203125 44.609375 42.84375 
Q 40.53125 48.484375 33.40625 48.484375 
Q 26.265625 48.484375 22.1875 42.84375 
Q 18.109375 37.203125 18.109375 27.296875 
Q 18.109375 17.390625 22.1875 11.75 
Q 26.265625 6.109375 33.40625 6.109375 
Q 40.53125 6.109375 44.609375 11.75 
Q 48.6875 17.390625 48.6875 27.296875 
z
" id="DejaVuSans-112"/>
       <path d="M 41.109375 46.296875 
Q 39.59375 47.171875 37.8125 47.578125 
Q 36.03125 48 33.890625 48 
Q 26.265625 48 22.1875 43.046875 
Q 18.109375 38.09375 18.109375 28.8125 
L 18.109375 0 
L 9.078125 0 
L 9.078125 54.6875 
L 18.109375 54.6875 
L 18.109375 46.1875 
Q 20.953125 51.171875 25.484375 53.578125 
Q 30.03125 56 36.53125 56 
Q 37.453125 56 38.578125 55.875 
Q 39.703125 55.765625 41.0625 55.515625 
z
" id="DejaVuSans-114"/>
      </defs>
      <g transform="translate(77.762829 205.756563)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-65"/>
       <use x="68.408203" xlink:href="#DejaVuSans-112"/>
       <use x="131.884766" xlink:href="#DejaVuSans-114"/>
      </g>
      <!-- 2020 -->
      <defs>
       <path d="M 19.1875 8.296875 
L 53.609375 8.296875 
L 53.609375 0 
L 7.328125 0 
L 7.328125 8.296875 
Q 12.9375 14.109375 22.625 23.890625 
Q 32.328125 33.6875 34.8125 36.53125 
Q 39.546875 41.84375 41.421875 45.53125 
Q 43.3125 49.21875 43.3125 52.78125 
Q 43.3125 58.59375 39.234375 62.25 
Q 35.15625 65.921875 28.609375 65.921875 
Q 23.96875 65.921875 18.8125 64.3125 
Q 13.671875 62.703125 7.8125 59.421875 
L 7.8125 69.390625 
Q 13.765625 71.78125 18.9375 73 
Q 24.125 74.21875 28.421875 74.21875 
Q 39.75 74.21875 46.484375 68.546875 
Q 53.21875 62.890625 53.21875 53.421875 
Q 53.21875 48.921875 51.53125 44.890625 
Q 49.859375 40.875 45.40625 35.40625 
Q 44.1875 33.984375 37.640625 27.21875 
Q 31.109375 20.453125 19.1875 8.296875 
z
" id="DejaVuSans-50"/>
       <path d="M 31.78125 66.40625 
Q 24.171875 66.40625 20.328125 58.90625 
Q 16.5 51.421875 16.5 36.375 
Q 16.5 21.390625 20.328125 13.890625 
Q 24.171875 6.390625 31.78125 6.390625 
Q 39.453125 6.390625 43.28125 13.890625 
Q 47.125 21.390625 47.125 36.375 
Q 47.125 51.421875 43.28125 58.90625 
Q 39.453125 66.40625 31.78125 66.40625 
z
M 31.78125 74.21875 
Q 44.046875 74.21875 50.515625 64.515625 
Q 56.984375 54.828125 56.984375 36.375 
Q 56.984375 17.96875 50.515625 8.265625 
Q 44.046875 -1.421875 31.78125 -1.421875 
Q 19.53125 -1.421875 13.0625 8.265625 
Q 6.59375 17.96875 6.59375 36.375 
Q 6.59375 54.828125 13.0625 64.515625 
Q 19.53125 74.21875 31.78125 74.21875 
z
" id="DejaVuSans-48"/>
      </defs>
      <g transform="translate(73.687829 216.954375)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
      </g>
     </g>
    </g>
    <g id="xtick_3">
     <g id="line2d_4">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="171.675987" xlink:href="#mc3d69031e6" y="191.158125"/>
      </g>
     </g>
     <g id="text_2">
      <!-- Mai -->
      <defs>
       <path d="M 9.8125 72.90625 
L 24.515625 72.90625 
L 43.109375 23.296875 
L 61.8125 72.90625 
L 76.515625 72.90625 
L 76.515625 0 
L 66.890625 0 
L 66.890625 64.015625 
L 48.09375 14.015625 
L 38.1875 14.015625 
L 19.390625 64.015625 
L 19.390625 0 
L 9.8125 0 
z
" id="DejaVuSans-77"/>
       <path d="M 34.28125 27.484375 
Q 23.390625 27.484375 19.1875 25 
Q 14.984375 22.515625 14.984375 16.5 
Q 14.984375 11.71875 18.140625 8.90625 
Q 21.296875 6.109375 26.703125 6.109375 
Q 34.1875 6.109375 38.703125 11.40625 
Q 43.21875 16.703125 43.21875 25.484375 
L 43.21875 27.484375 
z
M 52.203125 31.203125 
L 52.203125 0 
L 43.21875 0 
L 43.21875 8.296875 
Q 40.140625 3.328125 35.546875 0.953125 
Q 30.953125 -1.421875 24.3125 -1.421875 
Q 15.921875 -1.421875 10.953125 3.296875 
Q 6 8.015625 6 15.921875 
Q 6 25.140625 12.171875 29.828125 
Q 18.359375 34.515625 30.609375 34.515625 
L 43.21875 34.515625 
L 43.21875 35.40625 
Q 43.21875 41.609375 39.140625 45 
Q 35.0625 48.390625 27.6875 48.390625 
Q 23 48.390625 18.546875 47.265625 
Q 14.109375 46.140625 10.015625 43.890625 
L 10.015625 52.203125 
Q 14.9375 54.109375 19.578125 55.046875 
Q 24.21875 56 28.609375 56 
Q 40.484375 56 46.34375 49.84375 
Q 52.203125 43.703125 52.203125 31.203125 
z
" id="DejaVuSans-97"/>
       <path d="M 9.421875 54.6875 
L 18.40625 54.6875 
L 18.40625 0 
L 9.421875 0 
z
M 9.421875 75.984375 
L 18.40625 75.984375 
L 18.40625 64.59375 
L 9.421875 64.59375 
z
" id="DejaVuSans-105"/>
      </defs>
      <g transform="translate(162.908799 205.756563)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-77"/>
       <use x="86.279297" xlink:href="#DejaVuSans-97"/>
       <use x="147.558594" xlink:href="#DejaVuSans-105"/>
      </g>
     </g>
    </g>
    <g id="xtick_4">
     <g id="line2d_5">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="259.78125" xlink:href="#mc3d69031e6" y="191.158125"/>
      </g>
     </g>
     <g id="text_3">
      <!-- Jun -->
      <defs>
       <path d="M 9.8125 72.90625 
L 19.671875 72.90625 
L 19.671875 5.078125 
Q 19.671875 -8.109375 14.671875 -14.0625 
Q 9.671875 -20.015625 -1.421875 -20.015625 
L -5.171875 -20.015625 
L -5.171875 -11.71875 
L -2.09375 -11.71875 
Q 4.4375 -11.71875 7.125 -8.046875 
Q 9.8125 -4.390625 9.8125 5.078125 
z
" id="DejaVuSans-74"/>
       <path d="M 8.5 21.578125 
L 8.5 54.6875 
L 17.484375 54.6875 
L 17.484375 21.921875 
Q 17.484375 14.15625 20.5 10.265625 
Q 23.53125 6.390625 29.59375 6.390625 
Q 36.859375 6.390625 41.078125 11.03125 
Q 45.3125 15.671875 45.3125 23.6875 
L 45.3125 54.6875 
L 54.296875 54.6875 
L 54.296875 0 
L 45.3125 0 
L 45.3125 8.40625 
Q 42.046875 3.421875 37.71875 1 
Q 33.40625 -1.421875 27.6875 -1.421875 
Q 18.265625 -1.421875 13.375 4.4375 
Q 8.5 10.296875 8.5 21.578125 
z
M 31.109375 56 
z
" id="DejaVuSans-117"/>
       <path d="M 54.890625 33.015625 
L 54.890625 0 
L 45.90625 0 
L 45.90625 32.71875 
Q 45.90625 40.484375 42.875 44.328125 
Q 39.84375 48.1875 33.796875 48.1875 
Q 26.515625 48.1875 22.3125 43.546875 
Q 18.109375 38.921875 18.109375 30.90625 
L 18.109375 0 
L 9.078125 0 
L 9.078125 54.6875 
L 18.109375 54.6875 
L 18.109375 46.1875 
Q 21.34375 51.125 25.703125 53.5625 
Q 30.078125 56 35.796875 56 
Q 45.21875 56 50.046875 50.171875 
Q 54.890625 44.34375 54.890625 33.015625 
z
" id="DejaVuSans-110"/>
      </defs>
      <g transform="translate(251.96875 205.756563)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-74"/>
       <use x="29.492188" xlink:href="#DejaVuSans-117"/>
       <use x="92.871094" xlink:href="#DejaVuSans-110"/>
      </g>
     </g>
    </g>
    <g id="xtick_5">
     <g id="line2d_6">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="345.044408" xlink:href="#mc3d69031e6" y="191.158125"/>
      </g>
     </g>
     <g id="text_4">
      <!-- Jul -->
      <defs>
       <path d="M 9.421875 75.984375 
L 18.40625 75.984375 
L 18.40625 0 
L 9.421875 0 
z
" id="DejaVuSans-108"/>
      </defs>
      <g transform="translate(339.011595 205.756563)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-74"/>
       <use x="29.492188" xlink:href="#DejaVuSans-117"/>
       <use x="92.871094" xlink:href="#DejaVuSans-108"/>
      </g>
     </g>
    </g>
    <g id="xtick_6">
     <g id="line2d_7">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="421.78125" xlink:href="#mc3d69031e6" y="191.158125"/>
      </g>
     </g>
    </g>
    <g id="xtick_7">
     <g id="line2d_8">
      <defs>
       <path d="M 0 0 
L 0 2 
" id="md9351a71b5" style="stroke:#000000;stroke-width:0.6;"/>
      </defs>
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="60.833882" xlink:href="#md9351a71b5" y="191.158125"/>
      </g>
     </g>
    </g>
    <g id="xtick_8">
     <g id="line2d_9">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="80.728618" xlink:href="#md9351a71b5" y="191.158125"/>
      </g>
     </g>
    </g>
    <g id="xtick_9">
     <g id="line2d_10">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="100.623355" xlink:href="#md9351a71b5" y="191.158125"/>
      </g>
     </g>
    </g>
    <g id="xtick_10">
     <g id="line2d_11">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="120.518092" xlink:href="#md9351a71b5" y="191.158125"/>
      </g>
     </g>
    </g>
    <g id="xtick_11">
     <g id="line2d_12">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="140.412829" xlink:href="#md9351a71b5" y="191.158125"/>
      </g>
     </g>
    </g>
    <g id="xtick_12">
     <g id="line2d_13">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="160.307566" xlink:href="#md9351a71b5" y="191.158125"/>
      </g>
     </g>
    </g>
    <g id="xtick_13">
     <g id="line2d_14">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="180.202303" xlink:href="#md9351a71b5" y="191.158125"/>
      </g>
     </g>
    </g>
    <g id="xtick_14">
     <g id="line2d_15">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="200.097039" xlink:href="#md9351a71b5" y="191.158125"/>
      </g>
     </g>
    </g>
    <g id="xtick_15">
     <g id="line2d_16">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="219.991776" xlink:href="#md9351a71b5" y="191.158125"/>
      </g>
     </g>
    </g>
    <g id="xtick_16">
     <g id="line2d_17">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="239.886513" xlink:href="#md9351a71b5" y="191.158125"/>
      </g>
     </g>
    </g>
    <g id="xtick_17">
     <g id="line2d_18">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="279.675987" xlink:href="#md9351a71b5" y="191.158125"/>
      </g>
     </g>
    </g>
    <g id="xtick_18">
     <g id="line2d_19">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="299.570724" xlink:href="#md9351a71b5" y="191.158125"/>
      </g>
     </g>
    </g>
    <g id="xtick_19">
     <g id="line2d_20">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="319.465461" xlink:href="#md9351a71b5" y="191.158125"/>
      </g>
     </g>
    </g>
    <g id="xtick_20">
     <g id="line2d_21">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="339.360197" xlink:href="#md9351a71b5" y="191.158125"/>
      </g>
     </g>
    </g>
    <g id="xtick_21">
     <g id="line2d_22">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="359.254934" xlink:href="#md9351a71b5" y="191.158125"/>
      </g>
     </g>
    </g>
    <g id="xtick_22">
     <g id="line2d_23">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="379.149671" xlink:href="#md9351a71b5" y="191.158125"/>
      </g>
     </g>
    </g>
    <g id="xtick_23">
     <g id="line2d_24">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="399.044408" xlink:href="#md9351a71b5" y="191.158125"/>
      </g>
     </g>
    </g>
    <g id="xtick_24">
     <g id="line2d_25">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="418.939145" xlink:href="#md9351a71b5" y="191.158125"/>
      </g>
     </g>
    </g>
    <g id="text_5">
     <!-- Datum des Erkrankungsbeginns -->
     <defs>
      <path d="M 19.671875 64.796875 
L 19.671875 8.109375 
L 31.59375 8.109375 
Q 46.6875 8.109375 53.6875 14.9375 
Q 60.6875 21.78125 60.6875 36.53125 
Q 60.6875 51.171875 53.6875 57.984375 
Q 46.6875 64.796875 31.59375 64.796875 
z
M 9.8125 72.90625 
L 30.078125 72.90625 
Q 51.265625 72.90625 61.171875 64.09375 
Q 71.09375 55.28125 71.09375 36.53125 
Q 71.09375 17.671875 61.125 8.828125 
Q 51.171875 0 30.078125 0 
L 9.8125 0 
z
" id="DejaVuSans-68"/>
      <path d="M 18.3125 70.21875 
L 18.3125 54.6875 
L 36.8125 54.6875 
L 36.8125 47.703125 
L 18.3125 47.703125 
L 18.3125 18.015625 
Q 18.3125 11.328125 20.140625 9.421875 
Q 21.96875 7.515625 27.59375 7.515625 
L 36.8125 7.515625 
L 36.8125 0 
L 27.59375 0 
Q 17.1875 0 13.234375 3.875 
Q 9.28125 7.765625 9.28125 18.015625 
L 9.28125 47.703125 
L 2.6875 47.703125 
L 2.6875 54.6875 
L 9.28125 54.6875 
L 9.28125 70.21875 
z
" id="DejaVuSans-116"/>
      <path d="M 52 44.1875 
Q 55.375 50.25 60.0625 53.125 
Q 64.75 56 71.09375 56 
Q 79.640625 56 84.28125 50.015625 
Q 88.921875 44.046875 88.921875 33.015625 
L 88.921875 0 
L 79.890625 0 
L 79.890625 32.71875 
Q 79.890625 40.578125 77.09375 44.375 
Q 74.3125 48.1875 68.609375 48.1875 
Q 61.625 48.1875 57.5625 43.546875 
Q 53.515625 38.921875 53.515625 30.90625 
L 53.515625 0 
L 44.484375 0 
L 44.484375 32.71875 
Q 44.484375 40.625 41.703125 44.40625 
Q 38.921875 48.1875 33.109375 48.1875 
Q 26.21875 48.1875 22.15625 43.53125 
Q 18.109375 38.875 18.109375 30.90625 
L 18.109375 0 
L 9.078125 0 
L 9.078125 54.6875 
L 18.109375 54.6875 
L 18.109375 46.1875 
Q 21.1875 51.21875 25.484375 53.609375 
Q 29.78125 56 35.6875 56 
Q 41.65625 56 45.828125 52.96875 
Q 50 49.953125 52 44.1875 
z
" id="DejaVuSans-109"/>
      <path id="DejaVuSans-32"/>
      <path d="M 45.40625 46.390625 
L 45.40625 75.984375 
L 54.390625 75.984375 
L 54.390625 0 
L 45.40625 0 
L 45.40625 8.203125 
Q 42.578125 3.328125 38.25 0.953125 
Q 33.9375 -1.421875 27.875 -1.421875 
Q 17.96875 -1.421875 11.734375 6.484375 
Q 5.515625 14.40625 5.515625 27.296875 
Q 5.515625 40.1875 11.734375 48.09375 
Q 17.96875 56 27.875 56 
Q 33.9375 56 38.25 53.625 
Q 42.578125 51.265625 45.40625 46.390625 
z
M 14.796875 27.296875 
Q 14.796875 17.390625 18.875 11.75 
Q 22.953125 6.109375 30.078125 6.109375 
Q 37.203125 6.109375 41.296875 11.75 
Q 45.40625 17.390625 45.40625 27.296875 
Q 45.40625 37.203125 41.296875 42.84375 
Q 37.203125 48.484375 30.078125 48.484375 
Q 22.953125 48.484375 18.875 42.84375 
Q 14.796875 37.203125 14.796875 27.296875 
z
" id="DejaVuSans-100"/>
      <path d="M 56.203125 29.59375 
L 56.203125 25.203125 
L 14.890625 25.203125 
Q 15.484375 15.921875 20.484375 11.0625 
Q 25.484375 6.203125 34.421875 6.203125 
Q 39.59375 6.203125 44.453125 7.46875 
Q 49.3125 8.734375 54.109375 11.28125 
L 54.109375 2.78125 
Q 49.265625 0.734375 44.1875 -0.34375 
Q 39.109375 -1.421875 33.890625 -1.421875 
Q 20.796875 -1.421875 13.15625 6.1875 
Q 5.515625 13.8125 5.515625 26.8125 
Q 5.515625 40.234375 12.765625 48.109375 
Q 20.015625 56 32.328125 56 
Q 43.359375 56 49.78125 48.890625 
Q 56.203125 41.796875 56.203125 29.59375 
z
M 47.21875 32.234375 
Q 47.125 39.59375 43.09375 43.984375 
Q 39.0625 48.390625 32.421875 48.390625 
Q 24.90625 48.390625 20.390625 44.140625 
Q 15.875 39.890625 15.1875 32.171875 
z
" id="DejaVuSans-101"/>
      <path d="M 44.28125 53.078125 
L 44.28125 44.578125 
Q 40.484375 46.53125 36.375 47.5 
Q 32.28125 48.484375 27.875 48.484375 
Q 21.1875 48.484375 17.84375 46.4375 
Q 14.5 44.390625 14.5 40.28125 
Q 14.5 37.15625 16.890625 35.375 
Q 19.28125 33.59375 26.515625 31.984375 
L 29.59375 31.296875 
Q 39.15625 29.25 43.1875 25.515625 
Q 47.21875 21.78125 47.21875 15.09375 
Q 47.21875 7.46875 41.1875 3.015625 
Q 35.15625 -1.421875 24.609375 -1.421875 
Q 20.21875 -1.421875 15.453125 -0.5625 
Q 10.6875 0.296875 5.421875 2 
L 5.421875 11.28125 
Q 10.40625 8.6875 15.234375 7.390625 
Q 20.0625 6.109375 24.8125 6.109375 
Q 31.15625 6.109375 34.5625 8.28125 
Q 37.984375 10.453125 37.984375 14.40625 
Q 37.984375 18.0625 35.515625 20.015625 
Q 33.0625 21.96875 24.703125 23.78125 
L 21.578125 24.515625 
Q 13.234375 26.265625 9.515625 29.90625 
Q 5.8125 33.546875 5.8125 39.890625 
Q 5.8125 47.609375 11.28125 51.796875 
Q 16.75 56 26.8125 56 
Q 31.78125 56 36.171875 55.265625 
Q 40.578125 54.546875 44.28125 53.078125 
z
" id="DejaVuSans-115"/>
      <path d="M 9.8125 72.90625 
L 55.90625 72.90625 
L 55.90625 64.59375 
L 19.671875 64.59375 
L 19.671875 43.015625 
L 54.390625 43.015625 
L 54.390625 34.71875 
L 19.671875 34.71875 
L 19.671875 8.296875 
L 56.78125 8.296875 
L 56.78125 0 
L 9.8125 0 
z
" id="DejaVuSans-69"/>
      <path d="M 9.078125 75.984375 
L 18.109375 75.984375 
L 18.109375 31.109375 
L 44.921875 54.6875 
L 56.390625 54.6875 
L 27.390625 29.109375 
L 57.625 0 
L 45.90625 0 
L 18.109375 26.703125 
L 18.109375 0 
L 9.078125 0 
z
" id="DejaVuSans-107"/>
      <path d="M 45.40625 27.984375 
Q 45.40625 37.75 41.375 43.109375 
Q 37.359375 48.484375 30.078125 48.484375 
Q 22.859375 48.484375 18.828125 43.109375 
Q 14.796875 37.75 14.796875 27.984375 
Q 14.796875 18.265625 18.828125 12.890625 
Q 22.859375 7.515625 30.078125 7.515625 
Q 37.359375 7.515625 41.375 12.890625 
Q 45.40625 18.265625 45.40625 27.984375 
z
M 54.390625 6.78125 
Q 54.390625 -7.171875 48.1875 -13.984375 
Q 42 -20.796875 29.203125 -20.796875 
Q 24.46875 -20.796875 20.265625 -20.09375 
Q 16.0625 -19.390625 12.109375 -17.921875 
L 12.109375 -9.1875 
Q 16.0625 -11.328125 19.921875 -12.34375 
Q 23.78125 -13.375 27.78125 -13.375 
Q 36.625 -13.375 41.015625 -8.765625 
Q 45.40625 -4.15625 45.40625 5.171875 
L 45.40625 9.625 
Q 42.625 4.78125 38.28125 2.390625 
Q 33.9375 0 27.875 0 
Q 17.828125 0 11.671875 7.65625 
Q 5.515625 15.328125 5.515625 27.984375 
Q 5.515625 40.671875 11.671875 48.328125 
Q 17.828125 56 27.875 56 
Q 33.9375 56 38.28125 53.609375 
Q 42.625 51.21875 45.40625 46.390625 
L 45.40625 54.6875 
L 54.390625 54.6875 
z
" id="DejaVuSans-103"/>
      <path d="M 48.6875 27.296875 
Q 48.6875 37.203125 44.609375 42.84375 
Q 40.53125 48.484375 33.40625 48.484375 
Q 26.265625 48.484375 22.1875 42.84375 
Q 18.109375 37.203125 18.109375 27.296875 
Q 18.109375 17.390625 22.1875 11.75 
Q 26.265625 6.109375 33.40625 6.109375 
Q 40.53125 6.109375 44.609375 11.75 
Q 48.6875 17.390625 48.6875 27.296875 
z
M 18.109375 46.390625 
Q 20.953125 51.265625 25.265625 53.625 
Q 29.59375 56 35.59375 56 
Q 45.5625 56 51.78125 48.09375 
Q 58.015625 40.1875 58.015625 27.296875 
Q 58.015625 14.40625 51.78125 6.484375 
Q 45.5625 -1.421875 35.59375 -1.421875 
Q 29.59375 -1.421875 25.265625 0.953125 
Q 20.953125 3.328125 18.109375 8.203125 
L 18.109375 0 
L 9.078125 0 
L 9.078125 75.984375 
L 18.109375 75.984375 
z
" id="DejaVuSans-98"/>
     </defs>
     <g transform="translate(152.670313 226.6325)scale(0.1 -0.1)">
      <use xlink:href="#DejaVuSans-68"/>
      <use x="77.001953" xlink:href="#DejaVuSans-97"/>
      <use x="138.28125" xlink:href="#DejaVuSans-116"/>
      <use x="177.490234" xlink:href="#DejaVuSans-117"/>
      <use x="240.869141" xlink:href="#DejaVuSans-109"/>
      <use x="338.28125" xlink:href="#DejaVuSans-32"/>
      <use x="370.068359" xlink:href="#DejaVuSans-100"/>
      <use x="433.544922" xlink:href="#DejaVuSans-101"/>
      <use x="495.068359" xlink:href="#DejaVuSans-115"/>
      <use x="547.167969" xlink:href="#DejaVuSans-32"/>
      <use x="578.955078" xlink:href="#DejaVuSans-69"/>
      <use x="642.138672" xlink:href="#DejaVuSans-114"/>
      <use x="683.251953" xlink:href="#DejaVuSans-107"/>
      <use x="741.162109" xlink:href="#DejaVuSans-114"/>
      <use x="782.275391" xlink:href="#DejaVuSans-97"/>
      <use x="843.554688" xlink:href="#DejaVuSans-110"/>
      <use x="906.933594" xlink:href="#DejaVuSans-107"/>
      <use x="964.796875" xlink:href="#DejaVuSans-117"/>
      <use x="1028.175781" xlink:href="#DejaVuSans-110"/>
      <use x="1091.554688" xlink:href="#DejaVuSans-103"/>
      <use x="1155.03125" xlink:href="#DejaVuSans-115"/>
      <use x="1207.130859" xlink:href="#DejaVuSans-98"/>
      <use x="1270.607422" xlink:href="#DejaVuSans-101"/>
      <use x="1332.130859" xlink:href="#DejaVuSans-103"/>
      <use x="1395.607422" xlink:href="#DejaVuSans-105"/>
      <use x="1423.390625" xlink:href="#DejaVuSans-110"/>
      <use x="1486.769531" xlink:href="#DejaVuSans-110"/>
      <use x="1550.148438" xlink:href="#DejaVuSans-115"/>
     </g>
    </g>
   </g>
   <g id="matplotlib.axis_2">
    <g id="ytick_1">
     <g id="line2d_26">
      <path clip-path="url(#p16756ab622)" d="M 43.78125 167.420577 
L 421.78125 167.420577 
" style="fill:none;stroke:#999999;stroke-linecap:square;stroke-opacity:0.15;stroke-width:0.8;"/>
     </g>
     <g id="line2d_27">
      <defs>
       <path d="M 0 0 
L -3.5 0 
" id="m3d91269e3d" style="stroke:#000000;stroke-width:0.8;"/>
      </defs>
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="43.78125" xlink:href="#m3d91269e3d" y="167.420577"/>
      </g>
     </g>
     <g id="text_6">
      <!-- 0,8 -->
      <defs>
       <path d="M 11.71875 12.40625 
L 22.015625 12.40625 
L 22.015625 4 
L 14.015625 -11.625 
L 7.71875 -11.625 
L 11.71875 4 
z
" id="DejaVuSans-44"/>
       <path d="M 31.78125 34.625 
Q 24.75 34.625 20.71875 30.859375 
Q 16.703125 27.09375 16.703125 20.515625 
Q 16.703125 13.921875 20.71875 10.15625 
Q 24.75 6.390625 31.78125 6.390625 
Q 38.8125 6.390625 42.859375 10.171875 
Q 46.921875 13.96875 46.921875 20.515625 
Q 46.921875 27.09375 42.890625 30.859375 
Q 38.875 34.625 31.78125 34.625 
z
M 21.921875 38.8125 
Q 15.578125 40.375 12.03125 44.71875 
Q 8.5 49.078125 8.5 55.328125 
Q 8.5 64.0625 14.71875 69.140625 
Q 20.953125 74.21875 31.78125 74.21875 
Q 42.671875 74.21875 48.875 69.140625 
Q 55.078125 64.0625 55.078125 55.328125 
Q 55.078125 49.078125 51.53125 44.71875 
Q 48 40.375 41.703125 38.8125 
Q 48.828125 37.15625 52.796875 32.3125 
Q 56.78125 27.484375 56.78125 20.515625 
Q 56.78125 9.90625 50.3125 4.234375 
Q 43.84375 -1.421875 31.78125 -1.421875 
Q 19.734375 -1.421875 13.25 4.234375 
Q 6.78125 9.90625 6.78125 20.515625 
Q 6.78125 27.484375 10.78125 32.3125 
Q 14.796875 37.15625 21.921875 38.8125 
z
M 18.3125 54.390625 
Q 18.3125 48.734375 21.84375 45.5625 
Q 25.390625 42.390625 31.78125 42.390625 
Q 38.140625 42.390625 41.71875 45.5625 
Q 45.3125 48.734375 45.3125 54.390625 
Q 45.3125 60.0625 41.71875 63.234375 
Q 38.140625 66.40625 31.78125 66.40625 
Q 25.390625 66.40625 21.84375 63.234375 
Q 18.3125 60.0625 18.3125 54.390625 
z
" id="DejaVuSans-56"/>
      </defs>
      <g transform="translate(20.878125 171.219796)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-48"/>
       <use x="63.623047" xlink:href="#DejaVuSans-44"/>
       <use x="95.410156" xlink:href="#DejaVuSans-56"/>
      </g>
     </g>
    </g>
    <g id="ytick_2">
     <g id="line2d_28">
      <path clip-path="url(#p16756ab622)" d="M 43.78125 131.725017 
L 421.78125 131.725017 
" style="fill:none;stroke:#999999;stroke-linecap:square;stroke-opacity:0.15;stroke-width:0.8;"/>
     </g>
     <g id="line2d_29">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="43.78125" xlink:href="#m3d91269e3d" y="131.725017"/>
      </g>
     </g>
     <g id="text_7">
      <!-- 1,0 -->
      <defs>
       <path d="M 12.40625 8.296875 
L 28.515625 8.296875 
L 28.515625 63.921875 
L 10.984375 60.40625 
L 10.984375 69.390625 
L 28.421875 72.90625 
L 38.28125 72.90625 
L 38.28125 8.296875 
L 54.390625 8.296875 
L 54.390625 0 
L 12.40625 0 
z
" id="DejaVuSans-49"/>
      </defs>
      <g transform="translate(20.878125 135.524236)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-49"/>
       <use x="63.623047" xlink:href="#DejaVuSans-44"/>
       <use x="95.410156" xlink:href="#DejaVuSans-48"/>
      </g>
     </g>
    </g>
    <g id="ytick_3">
     <g id="line2d_30">
      <path clip-path="url(#p16756ab622)" d="M 43.78125 96.029457 
L 421.78125 96.029457 
" style="fill:none;stroke:#999999;stroke-linecap:square;stroke-opacity:0.15;stroke-width:0.8;"/>
     </g>
     <g id="line2d_31">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="43.78125" xlink:href="#m3d91269e3d" y="96.029457"/>
      </g>
     </g>
     <g id="text_8">
      <!-- 1,2 -->
      <g transform="translate(20.878125 99.828676)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-49"/>
       <use x="63.623047" xlink:href="#DejaVuSans-44"/>
       <use x="95.410156" xlink:href="#DejaVuSans-50"/>
      </g>
     </g>
    </g>
    <g id="ytick_4">
     <g id="line2d_32">
      <path clip-path="url(#p16756ab622)" d="M 43.78125 60.333897 
L 421.78125 60.333897 
" style="fill:none;stroke:#999999;stroke-linecap:square;stroke-opacity:0.15;stroke-width:0.8;"/>
     </g>
     <g id="line2d_33">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="43.78125" xlink:href="#m3d91269e3d" y="60.333897"/>
      </g>
     </g>
     <g id="text_9">
      <!-- 1,4 -->
      <defs>
       <path d="M 37.796875 64.3125 
L 12.890625 25.390625 
L 37.796875 25.390625 
z
M 35.203125 72.90625 
L 47.609375 72.90625 
L 47.609375 25.390625 
L 58.015625 25.390625 
L 58.015625 17.1875 
L 47.609375 17.1875 
L 47.609375 0 
L 37.796875 0 
L 37.796875 17.1875 
L 4.890625 17.1875 
L 4.890625 26.703125 
z
" id="DejaVuSans-52"/>
      </defs>
      <g transform="translate(20.878125 64.133115)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-49"/>
       <use x="63.623047" xlink:href="#DejaVuSans-44"/>
       <use x="95.410156" xlink:href="#DejaVuSans-52"/>
      </g>
     </g>
    </g>
    <g id="ytick_5">
     <g id="line2d_34">
      <path clip-path="url(#p16756ab622)" d="M 43.78125 24.638336 
L 421.78125 24.638336 
" style="fill:none;stroke:#999999;stroke-linecap:square;stroke-opacity:0.15;stroke-width:0.8;"/>
     </g>
     <g id="line2d_35">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="43.78125" xlink:href="#m3d91269e3d" y="24.638336"/>
      </g>
     </g>
     <g id="text_10">
      <!-- 1,6 -->
      <defs>
       <path d="M 33.015625 40.375 
Q 26.375 40.375 22.484375 35.828125 
Q 18.609375 31.296875 18.609375 23.390625 
Q 18.609375 15.53125 22.484375 10.953125 
Q 26.375 6.390625 33.015625 6.390625 
Q 39.65625 6.390625 43.53125 10.953125 
Q 47.40625 15.53125 47.40625 23.390625 
Q 47.40625 31.296875 43.53125 35.828125 
Q 39.65625 40.375 33.015625 40.375 
z
M 52.59375 71.296875 
L 52.59375 62.3125 
Q 48.875 64.0625 45.09375 64.984375 
Q 41.3125 65.921875 37.59375 65.921875 
Q 27.828125 65.921875 22.671875 59.328125 
Q 17.53125 52.734375 16.796875 39.40625 
Q 19.671875 43.65625 24.015625 45.921875 
Q 28.375 48.1875 33.59375 48.1875 
Q 44.578125 48.1875 50.953125 41.515625 
Q 57.328125 34.859375 57.328125 23.390625 
Q 57.328125 12.15625 50.6875 5.359375 
Q 44.046875 -1.421875 33.015625 -1.421875 
Q 20.359375 -1.421875 13.671875 8.265625 
Q 6.984375 17.96875 6.984375 36.375 
Q 6.984375 53.65625 15.1875 63.9375 
Q 23.390625 74.21875 37.203125 74.21875 
Q 40.921875 74.21875 44.703125 73.484375 
Q 48.484375 72.75 52.59375 71.296875 
z
" id="DejaVuSans-54"/>
      </defs>
      <g transform="translate(20.878125 28.437555)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-49"/>
       <use x="63.623047" xlink:href="#DejaVuSans-44"/>
       <use x="95.410156" xlink:href="#DejaVuSans-54"/>
      </g>
     </g>
    </g>
    <g id="text_11">
     <!-- 7-Tage R -->
     <defs>
      <path d="M 8.203125 72.90625 
L 55.078125 72.90625 
L 55.078125 68.703125 
L 28.609375 0 
L 18.3125 0 
L 43.21875 64.59375 
L 8.203125 64.59375 
z
" id="DejaVuSans-55"/>
      <path d="M 4.890625 31.390625 
L 31.203125 31.390625 
L 31.203125 23.390625 
L 4.890625 23.390625 
z
" id="DejaVuSans-45"/>
      <path d="M -0.296875 72.90625 
L 61.375 72.90625 
L 61.375 64.59375 
L 35.5 64.59375 
L 35.5 0 
L 25.59375 0 
L 25.59375 64.59375 
L -0.296875 64.59375 
z
" id="DejaVuSans-84"/>
      <path d="M 44.390625 34.1875 
Q 47.5625 33.109375 50.5625 29.59375 
Q 53.5625 26.078125 56.59375 19.921875 
L 66.609375 0 
L 56 0 
L 46.6875 18.703125 
Q 43.0625 26.03125 39.671875 28.421875 
Q 36.28125 30.8125 30.421875 30.8125 
L 19.671875 30.8125 
L 19.671875 0 
L 9.8125 0 
L 9.8125 72.90625 
L 32.078125 72.90625 
Q 44.578125 72.90625 50.734375 67.671875 
Q 56.890625 62.453125 56.890625 51.90625 
Q 56.890625 45.015625 53.6875 40.46875 
Q 50.484375 35.9375 44.390625 34.1875 
z
M 19.671875 64.796875 
L 19.671875 38.921875 
L 32.078125 38.921875 
Q 39.203125 38.921875 42.84375 42.21875 
Q 46.484375 45.515625 46.484375 51.90625 
Q 46.484375 58.296875 42.84375 61.546875 
Q 39.203125 64.796875 32.078125 64.796875 
z
" id="DejaVuSans-82"/>
     </defs>
     <g transform="translate(14.798437 129.135781)rotate(-90)scale(0.1 -0.1)">
      <use xlink:href="#DejaVuSans-55"/>
      <use x="63.623047" xlink:href="#DejaVuSans-45"/>
      <use x="99.566406" xlink:href="#DejaVuSans-84"/>
      <use x="160.400391" xlink:href="#DejaVuSans-97"/>
      <use x="221.679688" xlink:href="#DejaVuSans-103"/>
      <use x="285.15625" xlink:href="#DejaVuSans-101"/>
      <use x="346.679688" xlink:href="#DejaVuSans-32"/>
      <use x="378.466797" xlink:href="#DejaVuSans-82"/>
     </g>
    </g>
   </g>
   <g id="line2d_36">
    <path clip-path="url(#p16756ab622)" d="M 43.78125 131.725017 
L 421.78125 131.725017 
" style="fill:none;stroke:#000000;stroke-dasharray:1.5,2.475;stroke-dashoffset:0;stroke-opacity:0.3;stroke-width:1.5;"/>
   </g>
   <g id="patch_3">
    <path d="M 43.78125 191.158125 
L 43.78125 22.318125 
" style="fill:none;stroke:#000000;stroke-linecap:square;stroke-linejoin:miter;stroke-width:0.8;"/>
   </g>
   <g id="patch_4">
    <path d="M 421.78125 191.158125 
L 421.78125 22.318125 
" style="fill:none;stroke:#000000;stroke-linecap:square;stroke-linejoin:miter;stroke-width:0.8;"/>
   </g>
   <g id="patch_5">
    <path d="M 43.78125 191.158125 
L 421.78125 191.158125 
" style="fill:none;stroke:#000000;stroke-linecap:square;stroke-linejoin:miter;stroke-width:0.8;"/>
   </g>
   <g id="patch_6">
    <path d="M 43.78125 22.318125 
L 421.78125 22.318125 
" style="fill:none;stroke:#000000;stroke-linecap:square;stroke-linejoin:miter;stroke-width:0.8;"/>
   </g>
   <g id="text_12">
    <!-- 7-Tage Reproduktionszahl im Zeitverlauf (Deutschland) -->
    <defs>
     <path d="M 30.609375 48.390625 
Q 23.390625 48.390625 19.1875 42.75 
Q 14.984375 37.109375 14.984375 27.296875 
Q 14.984375 17.484375 19.15625 11.84375 
Q 23.34375 6.203125 30.609375 6.203125 
Q 37.796875 6.203125 41.984375 11.859375 
Q 46.1875 17.53125 46.1875 27.296875 
Q 46.1875 37.015625 41.984375 42.703125 
Q 37.796875 48.390625 30.609375 48.390625 
z
M 30.609375 56 
Q 42.328125 56 49.015625 48.375 
Q 55.71875 40.765625 55.71875 27.296875 
Q 55.71875 13.875 49.015625 6.21875 
Q 42.328125 -1.421875 30.609375 -1.421875 
Q 18.84375 -1.421875 12.171875 6.21875 
Q 5.515625 13.875 5.515625 27.296875 
Q 5.515625 40.765625 12.171875 48.375 
Q 18.84375 56 30.609375 56 
z
" id="DejaVuSans-111"/>
     <path d="M 5.515625 54.6875 
L 48.1875 54.6875 
L 48.1875 46.484375 
L 14.40625 7.171875 
L 48.1875 7.171875 
L 48.1875 0 
L 4.296875 0 
L 4.296875 8.203125 
L 38.09375 47.515625 
L 5.515625 47.515625 
z
" id="DejaVuSans-122"/>
     <path d="M 54.890625 33.015625 
L 54.890625 0 
L 45.90625 0 
L 45.90625 32.71875 
Q 45.90625 40.484375 42.875 44.328125 
Q 39.84375 48.1875 33.796875 48.1875 
Q 26.515625 48.1875 22.3125 43.546875 
Q 18.109375 38.921875 18.109375 30.90625 
L 18.109375 0 
L 9.078125 0 
L 9.078125 75.984375 
L 18.109375 75.984375 
L 18.109375 46.1875 
Q 21.34375 51.125 25.703125 53.5625 
Q 30.078125 56 35.796875 56 
Q 45.21875 56 50.046875 50.171875 
Q 54.890625 44.34375 54.890625 33.015625 
z
" id="DejaVuSans-104"/>
     <path d="M 5.609375 72.90625 
L 62.890625 72.90625 
L 62.890625 65.375 
L 16.796875 8.296875 
L 64.015625 8.296875 
L 64.015625 0 
L 4.5 0 
L 4.5 7.515625 
L 50.59375 64.59375 
L 5.609375 64.59375 
z
" id="DejaVuSans-90"/>
     <path d="M 2.984375 54.6875 
L 12.5 54.6875 
L 29.59375 8.796875 
L 46.6875 54.6875 
L 56.203125 54.6875 
L 35.6875 0 
L 23.484375 0 
z
" id="DejaVuSans-118"/>
     <path d="M 37.109375 75.984375 
L 37.109375 68.5 
L 28.515625 68.5 
Q 23.6875 68.5 21.796875 66.546875 
Q 19.921875 64.59375 19.921875 59.515625 
L 19.921875 54.6875 
L 34.71875 54.6875 
L 34.71875 47.703125 
L 19.921875 47.703125 
L 19.921875 0 
L 10.890625 0 
L 10.890625 47.703125 
L 2.296875 47.703125 
L 2.296875 54.6875 
L 10.890625 54.6875 
L 10.890625 58.5 
Q 10.890625 67.625 15.140625 71.796875 
Q 19.390625 75.984375 28.609375 75.984375 
z
" id="DejaVuSans-102"/>
     <path d="M 31 75.875 
Q 24.46875 64.65625 21.28125 53.65625 
Q 18.109375 42.671875 18.109375 31.390625 
Q 18.109375 20.125 21.3125 9.0625 
Q 24.515625 -2 31 -13.1875 
L 23.1875 -13.1875 
Q 15.875 -1.703125 12.234375 9.375 
Q 8.59375 20.453125 8.59375 31.390625 
Q 8.59375 42.28125 12.203125 53.3125 
Q 15.828125 64.359375 23.1875 75.875 
z
" id="DejaVuSans-40"/>
     <path d="M 48.78125 52.59375 
L 48.78125 44.1875 
Q 44.96875 46.296875 41.140625 47.34375 
Q 37.3125 48.390625 33.40625 48.390625 
Q 24.65625 48.390625 19.8125 42.84375 
Q 14.984375 37.3125 14.984375 27.296875 
Q 14.984375 17.28125 19.8125 11.734375 
Q 24.65625 6.203125 33.40625 6.203125 
Q 37.3125 6.203125 41.140625 7.25 
Q 44.96875 8.296875 48.78125 10.40625 
L 48.78125 2.09375 
Q 45.015625 0.34375 40.984375 -0.53125 
Q 36.96875 -1.421875 32.421875 -1.421875 
Q 20.0625 -1.421875 12.78125 6.34375 
Q 5.515625 14.109375 5.515625 27.296875 
Q 5.515625 40.671875 12.859375 48.328125 
Q 20.21875 56 33.015625 56 
Q 37.15625 56 41.109375 55.140625 
Q 45.0625 54.296875 48.78125 52.59375 
z
" id="DejaVuSans-99"/>
     <path d="M 8.015625 75.875 
L 15.828125 75.875 
Q 23.140625 64.359375 26.78125 53.3125 
Q 30.421875 42.28125 30.421875 31.390625 
Q 30.421875 20.453125 26.78125 9.375 
Q 23.140625 -1.703125 15.828125 -13.1875 
L 8.015625 -13.1875 
Q 14.5 -2 17.703125 9.0625 
Q 20.90625 20.125 20.90625 31.390625 
Q 20.90625 42.671875 17.703125 53.65625 
Q 14.5 64.65625 8.015625 75.875 
z
" id="DejaVuSans-41"/>
    </defs>
    <g transform="translate(65.919375 16.318125)scale(0.12 -0.12)">
     <use xlink:href="#DejaVuSans-55"/>
     <use x="63.623047" xlink:href="#DejaVuSans-45"/>
     <use x="99.566406" xlink:href="#DejaVuSans-84"/>
     <use x="160.400391" xlink:href="#DejaVuSans-97"/>
     <use x="221.679688" xlink:href="#DejaVuSans-103"/>
     <use x="285.15625" xlink:href="#DejaVuSans-101"/>
     <use x="346.679688" xlink:href="#DejaVuSans-32"/>
     <use x="378.466797" xlink:href="#DejaVuSans-82"/>
     <use x="447.886719" xlink:href="#DejaVuSans-101"/>
     <use x="509.410156" xlink:href="#DejaVuSans-112"/>
     <use x="572.886719" xlink:href="#DejaVuSans-114"/>
     <use x="613.96875" xlink:href="#DejaVuSans-111"/>
     <use x="675.150391" xlink:href="#DejaVuSans-100"/>
     <use x="738.626953" xlink:href="#DejaVuSans-117"/>
     <use x="802.005859" xlink:href="#DejaVuSans-107"/>
     <use x="859.916016" xlink:href="#DejaVuSans-116"/>
     <use x="899.125" xlink:href="#DejaVuSans-105"/>
     <use x="926.908203" xlink:href="#DejaVuSans-111"/>
     <use x="988.089844" xlink:href="#DejaVuSans-110"/>
     <use x="1051.46875" xlink:href="#DejaVuSans-115"/>
     <use x="1103.568359" xlink:href="#DejaVuSans-122"/>
     <use x="1156.058594" xlink:href="#DejaVuSans-97"/>
     <use x="1217.337891" xlink:href="#DejaVuSans-104"/>
     <use x="1280.716797" xlink:href="#DejaVuSans-108"/>
     <use x="1308.5" xlink:href="#DejaVuSans-32"/>
     <use x="1340.287109" xlink:href="#DejaVuSans-105"/>
     <use x="1368.070312" xlink:href="#DejaVuSans-109"/>
     <use x="1465.482422" xlink:href="#DejaVuSans-32"/>
     <use x="1497.269531" xlink:href="#DejaVuSans-90"/>
     <use x="1565.775391" xlink:href="#DejaVuSans-101"/>
     <use x="1627.298828" xlink:href="#DejaVuSans-105"/>
     <use x="1655.082031" xlink:href="#DejaVuSans-116"/>
     <use x="1694.291016" xlink:href="#DejaVuSans-118"/>
     <use x="1753.470703" xlink:href="#DejaVuSans-101"/>
     <use x="1814.994141" xlink:href="#DejaVuSans-114"/>
     <use x="1856.107422" xlink:href="#DejaVuSans-108"/>
     <use x="1883.890625" xlink:href="#DejaVuSans-97"/>
     <use x="1945.169922" xlink:href="#DejaVuSans-117"/>
     <use x="2008.548828" xlink:href="#DejaVuSans-102"/>
     <use x="2043.753906" xlink:href="#DejaVuSans-32"/>
     <use x="2075.541016" xlink:href="#DejaVuSans-40"/>
     <use x="2114.554688" xlink:href="#DejaVuSans-68"/>
     <use x="2191.556641" xlink:href="#DejaVuSans-101"/>
     <use x="2253.080078" xlink:href="#DejaVuSans-117"/>
     <use x="2316.458984" xlink:href="#DejaVuSans-116"/>
     <use x="2355.667969" xlink:href="#DejaVuSans-115"/>
     <use x="2407.767578" xlink:href="#DejaVuSans-99"/>
     <use x="2462.748047" xlink:href="#DejaVuSans-104"/>
     <use x="2526.126953" xlink:href="#DejaVuSans-108"/>
     <use x="2553.910156" xlink:href="#DejaVuSans-97"/>
     <use x="2615.189453" xlink:href="#DejaVuSans-110"/>
     <use x="2678.568359" xlink:href="#DejaVuSans-100"/>
     <use x="2742.044922" xlink:href="#DejaVuSans-41"/>
    </g>
   </g>
   <g id="legend_1">
    <g id="patch_7">
     <path d="M 262.495313 38.916562 
L 282.495313 38.916562 
L 282.495313 31.916562 
L 262.495313 31.916562 
z
" style="fill:#008000;opacity:0.3;"/>
    </g>
    <g id="text_13">
     <!-- 95%-Prädiktionsintervall -->
     <defs>
      <path d="M 10.984375 1.515625 
L 10.984375 10.5 
Q 14.703125 8.734375 18.5 7.8125 
Q 22.3125 6.890625 25.984375 6.890625 
Q 35.75 6.890625 40.890625 13.453125 
Q 46.046875 20.015625 46.78125 33.40625 
Q 43.953125 29.203125 39.59375 26.953125 
Q 35.25 24.703125 29.984375 24.703125 
Q 19.046875 24.703125 12.671875 31.3125 
Q 6.296875 37.9375 6.296875 49.421875 
Q 6.296875 60.640625 12.9375 67.421875 
Q 19.578125 74.21875 30.609375 74.21875 
Q 43.265625 74.21875 49.921875 64.515625 
Q 56.59375 54.828125 56.59375 36.375 
Q 56.59375 19.140625 48.40625 8.859375 
Q 40.234375 -1.421875 26.421875 -1.421875 
Q 22.703125 -1.421875 18.890625 -0.6875 
Q 15.09375 0.046875 10.984375 1.515625 
z
M 30.609375 32.421875 
Q 37.25 32.421875 41.125 36.953125 
Q 45.015625 41.5 45.015625 49.421875 
Q 45.015625 57.28125 41.125 61.84375 
Q 37.25 66.40625 30.609375 66.40625 
Q 23.96875 66.40625 20.09375 61.84375 
Q 16.21875 57.28125 16.21875 49.421875 
Q 16.21875 41.5 20.09375 36.953125 
Q 23.96875 32.421875 30.609375 32.421875 
z
" id="DejaVuSans-57"/>
      <path d="M 10.796875 72.90625 
L 49.515625 72.90625 
L 49.515625 64.59375 
L 19.828125 64.59375 
L 19.828125 46.734375 
Q 21.96875 47.46875 24.109375 47.828125 
Q 26.265625 48.1875 28.421875 48.1875 
Q 40.625 48.1875 47.75 41.5 
Q 54.890625 34.8125 54.890625 23.390625 
Q 54.890625 11.625 47.5625 5.09375 
Q 40.234375 -1.421875 26.90625 -1.421875 
Q 22.3125 -1.421875 17.546875 -0.640625 
Q 12.796875 0.140625 7.71875 1.703125 
L 7.71875 11.625 
Q 12.109375 9.234375 16.796875 8.0625 
Q 21.484375 6.890625 26.703125 6.890625 
Q 35.15625 6.890625 40.078125 11.328125 
Q 45.015625 15.765625 45.015625 23.390625 
Q 45.015625 31 40.078125 35.4375 
Q 35.15625 39.890625 26.703125 39.890625 
Q 22.75 39.890625 18.8125 39.015625 
Q 14.890625 38.140625 10.796875 36.28125 
z
" id="DejaVuSans-53"/>
      <path d="M 72.703125 32.078125 
Q 68.453125 32.078125 66.03125 28.46875 
Q 63.625 24.859375 63.625 18.40625 
Q 63.625 12.0625 66.03125 8.421875 
Q 68.453125 4.78125 72.703125 4.78125 
Q 76.859375 4.78125 79.265625 8.421875 
Q 81.6875 12.0625 81.6875 18.40625 
Q 81.6875 24.8125 79.265625 28.4375 
Q 76.859375 32.078125 72.703125 32.078125 
z
M 72.703125 38.28125 
Q 80.421875 38.28125 84.953125 32.90625 
Q 89.5 27.546875 89.5 18.40625 
Q 89.5 9.28125 84.9375 3.921875 
Q 80.375 -1.421875 72.703125 -1.421875 
Q 64.890625 -1.421875 60.34375 3.921875 
Q 55.8125 9.28125 55.8125 18.40625 
Q 55.8125 27.59375 60.375 32.9375 
Q 64.9375 38.28125 72.703125 38.28125 
z
M 22.3125 68.015625 
Q 18.109375 68.015625 15.6875 64.375 
Q 13.28125 60.75 13.28125 54.390625 
Q 13.28125 47.953125 15.671875 44.328125 
Q 18.0625 40.71875 22.3125 40.71875 
Q 26.5625 40.71875 28.96875 44.328125 
Q 31.390625 47.953125 31.390625 54.390625 
Q 31.390625 60.6875 28.953125 64.34375 
Q 26.515625 68.015625 22.3125 68.015625 
z
M 66.40625 74.21875 
L 74.21875 74.21875 
L 28.609375 -1.421875 
L 20.796875 -1.421875 
z
M 22.3125 74.21875 
Q 30.03125 74.21875 34.609375 68.875 
Q 39.203125 63.53125 39.203125 54.390625 
Q 39.203125 45.171875 34.640625 39.84375 
Q 30.078125 34.515625 22.3125 34.515625 
Q 14.546875 34.515625 10.03125 39.859375 
Q 5.515625 45.21875 5.515625 54.390625 
Q 5.515625 63.484375 10.046875 68.84375 
Q 14.59375 74.21875 22.3125 74.21875 
z
" id="DejaVuSans-37"/>
      <path d="M 19.671875 64.796875 
L 19.671875 37.40625 
L 32.078125 37.40625 
Q 38.96875 37.40625 42.71875 40.96875 
Q 46.484375 44.53125 46.484375 51.125 
Q 46.484375 57.671875 42.71875 61.234375 
Q 38.96875 64.796875 32.078125 64.796875 
z
M 9.8125 72.90625 
L 32.078125 72.90625 
Q 44.34375 72.90625 50.609375 67.359375 
Q 56.890625 61.8125 56.890625 51.125 
Q 56.890625 40.328125 50.609375 34.8125 
Q 44.34375 29.296875 32.078125 29.296875 
L 19.671875 29.296875 
L 19.671875 0 
L 9.8125 0 
z
" id="DejaVuSans-80"/>
      <path d="M 34.28125 27.484375 
Q 23.390625 27.484375 19.1875 25 
Q 14.984375 22.515625 14.984375 16.5 
Q 14.984375 11.71875 18.140625 8.90625 
Q 21.296875 6.109375 26.703125 6.109375 
Q 34.1875 6.109375 38.703125 11.40625 
Q 43.21875 16.703125 43.21875 25.484375 
L 43.21875 27.484375 
z
M 52.203125 31.203125 
L 52.203125 0 
L 43.21875 0 
L 43.21875 8.296875 
Q 40.140625 3.328125 35.546875 0.953125 
Q 30.953125 -1.421875 24.3125 -1.421875 
Q 15.921875 -1.421875 10.953125 3.296875 
Q 6 8.015625 6 15.921875 
Q 6 25.140625 12.171875 29.828125 
Q 18.359375 34.515625 30.609375 34.515625 
L 43.21875 34.515625 
L 43.21875 35.40625 
Q 43.21875 41.609375 39.140625 45 
Q 35.0625 48.390625 27.6875 48.390625 
Q 23 48.390625 18.546875 47.265625 
Q 14.109375 46.140625 10.015625 43.890625 
L 10.015625 52.203125 
Q 14.9375 54.109375 19.578125 55.046875 
Q 24.21875 56 28.609375 56 
Q 40.484375 56 46.34375 49.84375 
Q 52.203125 43.703125 52.203125 31.203125 
z
M 33.59375 75.78125 
L 43.5 75.78125 
L 43.5 65.921875 
L 33.59375 65.921875 
z
M 14.5 75.78125 
L 24.421875 75.78125 
L 24.421875 65.921875 
L 14.5 65.921875 
z
" id="DejaVuSans-228"/>
     </defs>
     <g transform="translate(290.495313 38.916562)scale(0.1 -0.1)">
      <use xlink:href="#DejaVuSans-57"/>
      <use x="63.623047" xlink:href="#DejaVuSans-53"/>
      <use x="127.246094" xlink:href="#DejaVuSans-37"/>
      <use x="222.265625" xlink:href="#DejaVuSans-45"/>
      <use x="258.349609" xlink:href="#DejaVuSans-80"/>
      <use x="318.636719" xlink:href="#DejaVuSans-114"/>
      <use x="359.75" xlink:href="#DejaVuSans-228"/>
      <use x="421.029297" xlink:href="#DejaVuSans-100"/>
      <use x="484.505859" xlink:href="#DejaVuSans-105"/>
      <use x="512.289062" xlink:href="#DejaVuSans-107"/>
      <use x="570.199219" xlink:href="#DejaVuSans-116"/>
      <use x="609.408203" xlink:href="#DejaVuSans-105"/>
      <use x="637.191406" xlink:href="#DejaVuSans-111"/>
      <use x="698.373047" xlink:href="#DejaVuSans-110"/>
      <use x="761.751953" xlink:href="#DejaVuSans-115"/>
      <use x="813.851562" xlink:href="#DejaVuSans-105"/>
      <use x="841.634766" xlink:href="#DejaVuSans-110"/>
      <use x="905.013672" xlink:href="#DejaVuSans-116"/>
      <use x="944.222656" xlink:href="#DejaVuSans-101"/>
      <use x="1005.746094" xlink:href="#DejaVuSans-114"/>
      <use x="1046.859375" xlink:href="#DejaVuSans-118"/>
      <use x="1106.039062" xlink:href="#DejaVuSans-97"/>
      <use x="1167.318359" xlink:href="#DejaVuSans-108"/>
      <use x="1195.101562" xlink:href="#DejaVuSans-108"/>
     </g>
    </g>
   </g>
  </g>
  <g id="text_14">
   <!-- Datenstand: 1. August 2020 -->
   <defs>
    <path d="M 11.71875 12.40625 
L 22.015625 12.40625 
L 22.015625 0 
L 11.71875 0 
z
M 11.71875 51.703125 
L 22.015625 51.703125 
L 22.015625 39.3125 
L 11.71875 39.3125 
z
" id="DejaVuSans-58"/>
    <path d="M 10.6875 12.40625 
L 21 12.40625 
L 21 0 
L 10.6875 0 
z
" id="DejaVuSans-46"/>
   </defs>
   <g transform="translate(342.179063 224.352937)scale(0.06 -0.06)">
    <use xlink:href="#DejaVuSans-68"/>
    <use x="77.001953" xlink:href="#DejaVuSans-97"/>
    <use x="138.28125" xlink:href="#DejaVuSans-116"/>
    <use x="177.490234" xlink:href="#DejaVuSans-101"/>
    <use x="239.013672" xlink:href="#DejaVuSans-110"/>
    <use x="302.392578" xlink:href="#DejaVuSans-115"/>
    <use x="354.492188" xlink:href="#DejaVuSans-116"/>
    <use x="393.701172" xlink:href="#DejaVuSans-97"/>
    <use x="454.980469" xlink:href="#DejaVuSans-110"/>
    <use x="518.359375" xlink:href="#DejaVuSans-100"/>
    <use x="581.835938" xlink:href="#DejaVuSans-58"/>
    <use x="615.527344" xlink:href="#DejaVuSans-32"/>
    <use x="647.314453" xlink:href="#DejaVuSans-49"/>
    <use x="710.9375" xlink:href="#DejaVuSans-46"/>
    <use x="742.724609" xlink:href="#DejaVuSans-32"/>
    <use x="774.511719" xlink:href="#DejaVuSans-65"/>
    <use x="842.919922" xlink:href="#DejaVuSans-117"/>
    <use x="906.298828" xlink:href="#DejaVuSans-103"/>
    <use x="969.775391" xlink:href="#DejaVuSans-117"/>
    <use x="1033.154297" xlink:href="#DejaVuSans-115"/>
    <use x="1085.253906" xlink:href="#DejaVuSans-116"/>
    <use x="1124.462891" xlink:href="#DejaVuSans-32"/>
    <use x="1156.25" xlink:href="#DejaVuSans-50"/>
    <use x="1219.873047" xlink:href="#DejaVuSans-48"/>
    <use x="1283.496094" xlink:href="#DejaVuSans-50"/>
    <use x="1347.119141" xlink:href="#DejaVuSans-48"/>
   </g>
   <!-- Datenquelle: RKI Nowcast -->
   <defs>
    <path d="M 14.796875 27.296875 
Q 14.796875 17.390625 18.875 11.75 
Q 22.953125 6.109375 30.078125 6.109375 
Q 37.203125 6.109375 41.296875 11.75 
Q 45.40625 17.390625 45.40625 27.296875 
Q 45.40625 37.203125 41.296875 42.84375 
Q 37.203125 48.484375 30.078125 48.484375 
Q 22.953125 48.484375 18.875 42.84375 
Q 14.796875 37.203125 14.796875 27.296875 
z
M 45.40625 8.203125 
Q 42.578125 3.328125 38.25 0.953125 
Q 33.9375 -1.421875 27.875 -1.421875 
Q 17.96875 -1.421875 11.734375 6.484375 
Q 5.515625 14.40625 5.515625 27.296875 
Q 5.515625 40.1875 11.734375 48.09375 
Q 17.96875 56 27.875 56 
Q 33.9375 56 38.25 53.625 
Q 42.578125 51.265625 45.40625 46.390625 
L 45.40625 54.6875 
L 54.390625 54.6875 
L 54.390625 -20.796875 
L 45.40625 -20.796875 
z
" id="DejaVuSans-113"/>
    <path d="M 9.8125 72.90625 
L 19.671875 72.90625 
L 19.671875 42.09375 
L 52.390625 72.90625 
L 65.09375 72.90625 
L 28.90625 38.921875 
L 67.671875 0 
L 54.6875 0 
L 19.671875 35.109375 
L 19.671875 0 
L 9.8125 0 
z
" id="DejaVuSans-75"/>
    <path d="M 9.8125 72.90625 
L 19.671875 72.90625 
L 19.671875 0 
L 9.8125 0 
z
" id="DejaVuSans-73"/>
    <path d="M 9.8125 72.90625 
L 23.09375 72.90625 
L 55.421875 11.921875 
L 55.421875 72.90625 
L 64.984375 72.90625 
L 64.984375 0 
L 51.703125 0 
L 19.390625 60.984375 
L 19.390625 0 
L 9.8125 0 
z
" id="DejaVuSans-78"/>
    <path d="M 4.203125 54.6875 
L 13.1875 54.6875 
L 24.421875 12.015625 
L 35.59375 54.6875 
L 46.1875 54.6875 
L 57.421875 12.015625 
L 68.609375 54.6875 
L 77.59375 54.6875 
L 63.28125 0 
L 52.6875 0 
L 40.921875 44.828125 
L 29.109375 0 
L 18.5 0 
z
" id="DejaVuSans-119"/>
   </defs>
   <g transform="translate(349.119375 231.071625)scale(0.06 -0.06)">
    <use xlink:href="#DejaVuSans-68"/>
    <use x="77.001953" xlink:href="#DejaVuSans-97"/>
    <use x="138.28125" xlink:href="#DejaVuSans-116"/>
    <use x="177.490234" xlink:href="#DejaVuSans-101"/>
    <use x="239.013672" xlink:href="#DejaVuSans-110"/>
    <use x="302.392578" xlink:href="#DejaVuSans-113"/>
    <use x="365.869141" xlink:href="#DejaVuSans-117"/>
    <use x="429.248047" xlink:href="#DejaVuSans-101"/>
    <use x="490.771484" xlink:href="#DejaVuSans-108"/>
    <use x="518.554688" xlink:href="#DejaVuSans-108"/>
    <use x="546.337891" xlink:href="#DejaVuSans-101"/>
    <use x="607.861328" xlink:href="#DejaVuSans-58"/>
    <use x="641.552734" xlink:href="#DejaVuSans-32"/>
    <use x="673.339844" xlink:href="#DejaVuSans-82"/>
    <use x="742.822266" xlink:href="#DejaVuSans-75"/>
    <use x="808.398438" xlink:href="#DejaVuSans-73"/>
    <use x="837.890625" xlink:href="#DejaVuSans-32"/>
    <use x="869.677734" xlink:href="#DejaVuSans-78"/>
    <use x="944.482422" xlink:href="#DejaVuSans-111"/>
    <use x="1005.664062" xlink:href="#DejaVuSans-119"/>
    <use x="1087.451172" xlink:href="#DejaVuSans-99"/>
    <use x="1142.431641" xlink:href="#DejaVuSans-97"/>
    <use x="1203.710938" xlink:href="#DejaVuSans-115"/>
    <use x="1255.810547" xlink:href="#DejaVuSans-116"/>
   </g>
   <!-- Viz: @CorneliusRoemer -->
   <defs>
    <path d="M 28.609375 0 
L 0.78125 72.90625 
L 11.078125 72.90625 
L 34.1875 11.53125 
L 57.328125 72.90625 
L 67.578125 72.90625 
L 39.796875 0 
z
" id="DejaVuSans-86"/>
    <path d="M 37.203125 26.21875 
Q 37.203125 19.234375 40.671875 15.25 
Q 44.140625 11.28125 50.203125 11.28125 
Q 56.203125 11.28125 59.640625 15.28125 
Q 63.09375 19.28125 63.09375 26.21875 
Q 63.09375 33.0625 59.578125 37.078125 
Q 56.0625 41.109375 50.09375 41.109375 
Q 44.1875 41.109375 40.6875 37.109375 
Q 37.203125 33.109375 37.203125 26.21875 
z
M 63.8125 11.625 
Q 60.890625 7.859375 57.109375 6.078125 
Q 53.328125 4.296875 48.296875 4.296875 
Q 39.890625 4.296875 34.640625 10.375 
Q 29.390625 16.453125 29.390625 26.21875 
Q 29.390625 35.984375 34.65625 42.078125 
Q 39.9375 48.1875 48.296875 48.1875 
Q 53.328125 48.1875 57.125 46.359375 
Q 60.9375 44.53125 63.8125 40.828125 
L 63.8125 47.21875 
L 70.796875 47.21875 
L 70.796875 11.28125 
Q 77.9375 12.359375 81.953125 17.796875 
Q 85.984375 23.25 85.984375 31.890625 
Q 85.984375 37.109375 84.4375 41.703125 
Q 82.90625 46.296875 79.78125 50.203125 
Q 74.703125 56.59375 67.40625 59.984375 
Q 60.109375 63.375 51.515625 63.375 
Q 45.515625 63.375 39.984375 61.78125 
Q 34.46875 60.203125 29.78125 57.078125 
Q 22.125 52.09375 17.796875 44.015625 
Q 13.484375 35.9375 13.484375 26.515625 
Q 13.484375 18.75 16.28125 11.953125 
Q 19.09375 5.171875 24.421875 0 
Q 29.546875 -5.078125 36.28125 -7.734375 
Q 43.015625 -10.40625 50.6875 -10.40625 
Q 56.984375 -10.40625 63.0625 -8.28125 
Q 69.140625 -6.15625 74.21875 -2.203125 
L 78.609375 -7.625 
Q 72.515625 -12.359375 65.3125 -14.875 
Q 58.109375 -17.390625 50.6875 -17.390625 
Q 41.65625 -17.390625 33.640625 -14.1875 
Q 25.640625 -10.984375 19.390625 -4.890625 
Q 13.140625 1.21875 9.859375 9.25 
Q 6.59375 17.28125 6.59375 26.515625 
Q 6.59375 35.40625 9.90625 43.453125 
Q 13.234375 51.515625 19.390625 57.625 
Q 25.6875 63.8125 33.9375 67.109375 
Q 42.1875 70.40625 51.421875 70.40625 
Q 61.765625 70.40625 70.625 66.15625 
Q 79.5 61.921875 85.5 54.109375 
Q 89.15625 49.3125 91.078125 43.703125 
Q 93.015625 38.09375 93.015625 32.078125 
Q 93.015625 19.234375 85.25 11.8125 
Q 77.484375 4.390625 63.8125 4.109375 
z
" id="DejaVuSans-64"/>
    <path d="M 64.40625 67.28125 
L 64.40625 56.890625 
Q 59.421875 61.53125 53.78125 63.8125 
Q 48.140625 66.109375 41.796875 66.109375 
Q 29.296875 66.109375 22.65625 58.46875 
Q 16.015625 50.828125 16.015625 36.375 
Q 16.015625 21.96875 22.65625 14.328125 
Q 29.296875 6.6875 41.796875 6.6875 
Q 48.140625 6.6875 53.78125 8.984375 
Q 59.421875 11.28125 64.40625 15.921875 
L 64.40625 5.609375 
Q 59.234375 2.09375 53.4375 0.328125 
Q 47.65625 -1.421875 41.21875 -1.421875 
Q 24.65625 -1.421875 15.125 8.703125 
Q 5.609375 18.84375 5.609375 36.375 
Q 5.609375 53.953125 15.125 64.078125 
Q 24.65625 74.21875 41.21875 74.21875 
Q 47.75 74.21875 53.53125 72.484375 
Q 59.328125 70.75 64.40625 67.28125 
z
" id="DejaVuSans-67"/>
   </defs>
   <g transform="translate(356.360625 237.790312)scale(0.06 -0.06)">
    <use xlink:href="#DejaVuSans-86"/>
    <use x="68.376953" xlink:href="#DejaVuSans-105"/>
    <use x="96.160156" xlink:href="#DejaVuSans-122"/>
    <use x="148.650391" xlink:href="#DejaVuSans-58"/>
    <use x="182.341797" xlink:href="#DejaVuSans-32"/>
    <use x="214.128906" xlink:href="#DejaVuSans-64"/>
    <use x="314.128906" xlink:href="#DejaVuSans-67"/>
    <use x="383.953125" xlink:href="#DejaVuSans-111"/>
    <use x="445.134766" xlink:href="#DejaVuSans-114"/>
    <use x="486.232422" xlink:href="#DejaVuSans-110"/>
    <use x="549.611328" xlink:href="#DejaVuSans-101"/>
    <use x="611.134766" xlink:href="#DejaVuSans-108"/>
    <use x="638.917969" xlink:href="#DejaVuSans-105"/>
    <use x="666.701172" xlink:href="#DejaVuSans-117"/>
    <use x="730.080078" xlink:href="#DejaVuSans-115"/>
    <use x="782.179688" xlink:href="#DejaVuSans-82"/>
    <use x="851.599609" xlink:href="#DejaVuSans-111"/>
    <use x="912.78125" xlink:href="#DejaVuSans-101"/>
    <use x="974.304688" xlink:href="#DejaVuSans-109"/>
    <use x="1071.716797" xlink:href="#DejaVuSans-101"/>
    <use x="1133.240234" xlink:href="#DejaVuSans-114"/>
   </g>
  </g>
 </g>
 <defs>
  <clipPath id="p16756ab622">
   <rect height="168.84" width="378" x="43.78125" y="22.318125"/>
  </clipPath>
 </defs>
</svg>

</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[83]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">adjusted_b</span> <span class="o">=</span> <span class="n">result_b</span><span class="o">.</span><span class="n">observed</span> <span class="o">/</span> <span class="n">result_b</span><span class="o">.</span><span class="n">seasonal</span>
<span class="n">adjusted_c</span> <span class="o">=</span> <span class="n">nowcast</span><span class="o">.</span><span class="n">c</span><span class="p">[</span><span class="mi">0</span><span class="p">:]</span> <span class="o">/</span> <span class="n">result_b</span><span class="o">.</span><span class="n">seasonal</span>
<span class="n">adjusted_d</span> <span class="o">=</span> <span class="n">nowcast</span><span class="o">.</span><span class="n">d</span><span class="p">[</span><span class="mi">0</span><span class="p">:]</span> <span class="o">/</span> <span class="n">result_b</span><span class="o">.</span><span class="n">seasonal</span>

<span class="n">locale</span><span class="o">.</span><span class="n">setlocale</span><span class="p">(</span><span class="n">locale</span><span class="o">.</span><span class="n">LC_ALL</span><span class="p">,</span> <span class="s1">&#39;de_DE&#39;</span><span class="p">)</span>

<span class="n">fig</span> <span class="o">=</span> <span class="n">plt</span><span class="o">.</span><span class="n">figure</span><span class="p">(</span><span class="n">num</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span> <span class="n">figsize</span><span class="o">=</span><span class="p">(</span><span class="mf">6.75</span><span class="p">,</span> <span class="mf">3.5</span><span class="p">),</span> <span class="n">facecolor</span><span class="o">=</span><span class="s1">&#39;w&#39;</span><span class="p">,</span> <span class="n">edgecolor</span><span class="o">=</span><span class="s1">&#39;k&#39;</span><span class="p">)</span>

<span class="n">ax</span> <span class="o">=</span> <span class="n">adjusted_b</span><span class="p">[</span><span class="mi">0</span><span class="p">:]</span><span class="o">.</span><span class="n">plot</span><span class="p">()</span>
<span class="n">ax</span><span class="o">.</span><span class="n">fill_between</span><span class="p">(</span><span class="n">adjusted_b</span><span class="o">.</span><span class="n">index</span><span class="p">,</span><span class="n">adjusted_c</span><span class="p">,</span><span class="n">adjusted_d</span><span class="p">,</span><span class="n">color</span><span class="o">=</span><span class="s1">&#39;g&#39;</span><span class="p">,</span><span class="n">alpha</span><span class="o">=</span><span class="mf">0.3</span><span class="p">,</span><span class="n">lw</span><span class="o">=</span><span class="mi">0</span><span class="p">,</span><span class="n">zorder</span><span class="o">=</span><span class="mi">0</span><span class="p">)</span>
<span class="c1">#ax.set_xlim(left=nowcast.index[1])</span>
<span class="n">ax</span><span class="o">.</span><span class="n">set_xlim</span><span class="p">(</span><span class="n">left</span><span class="o">=</span><span class="n">nowcast</span><span class="o">.</span><span class="n">index</span><span class="p">[</span><span class="mi">1</span><span class="p">],</span><span class="n">right</span><span class="o">=</span><span class="n">nowcast</span><span class="o">.</span><span class="n">index</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span><span class="o">+</span><span class="n">pd</span><span class="o">.</span><span class="n">Timedelta</span><span class="p">(</span><span class="n">days</span><span class="o">=</span><span class="mi">1</span><span class="p">))</span>
<span class="c1">#ax.set_ylim(top=1500,bottom=0)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">yscale</span><span class="p">(</span><span class="s1">&#39;log&#39;</span><span class="p">)</span>
<span class="n">red_patch</span> <span class="o">=</span> <span class="n">mpatches</span><span class="o">.</span><span class="n">Patch</span><span class="p">(</span><span class="n">color</span><span class="o">=</span><span class="s1">&#39;green&#39;</span><span class="p">,</span> <span class="n">alpha</span><span class="o">=</span><span class="mf">0.3</span><span class="p">,</span> <span class="n">label</span><span class="o">=</span><span class="s1">&#39;95%-Prädiktionsintervall&#39;</span><span class="p">,</span><span class="n">ec</span><span class="o">=</span><span class="kc">None</span><span class="p">)</span>
<span class="n">ax</span><span class="o">.</span><span class="n">legend</span><span class="p">(</span><span class="n">handles</span><span class="o">=</span><span class="p">[</span><span class="n">red_patch</span><span class="p">],</span><span class="n">frameon</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s2">&quot;Logarithmische Darstellung der deutschen Fallzahlen&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s2">&quot;Saisonal bereinigte Fallzahlen&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s2">&quot;Datum des Erkrankungsbeginns&quot;</span><span class="p">)</span>
<span class="n">ax</span><span class="o">.</span><span class="n">tick_params</span><span class="p">(</span><span class="n">axis</span><span class="o">=</span><span class="s1">&#39;x&#39;</span><span class="p">,</span> <span class="n">which</span><span class="o">=</span><span class="s1">&#39;major&#39;</span><span class="p">,</span> <span class="n">pad</span><span class="o">=</span><span class="mi">5</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">grid</span><span class="p">(</span><span class="n">axis</span> <span class="o">=</span> <span class="s1">&#39;y&#39;</span><span class="p">,</span> <span class="n">b</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">which</span><span class="o">=</span><span class="s1">&#39;both&#39;</span><span class="p">,</span> <span class="n">color</span><span class="o">=</span><span class="s1">&#39;#999999&#39;</span><span class="p">,</span> <span class="n">linestyle</span><span class="o">=</span><span class="s1">&#39;-&#39;</span><span class="p">,</span> <span class="n">alpha</span><span class="o">=</span><span class="mf">0.15</span><span class="p">,</span><span class="n">zorder</span><span class="o">=-</span><span class="mi">1</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">subplots_adjust</span><span class="p">(</span><span class="n">left</span><span class="o">=</span><span class="mf">0.2</span><span class="p">,</span> <span class="n">right</span><span class="o">=</span><span class="mf">0.9</span><span class="p">,</span> <span class="n">top</span><span class="o">=</span><span class="mf">0.9</span><span class="p">,</span> <span class="n">bottom</span><span class="o">=</span><span class="mf">0.25</span><span class="p">)</span>
<span class="n">fig</span><span class="o">.</span><span class="n">text</span><span class="p">(</span><span class="mf">0.90</span><span class="p">,</span> <span class="mf">0.06</span><span class="p">,</span> <span class="s2">&quot;Datenstand: &quot;</span> <span class="o">+</span> <span class="n">today</span> <span class="o">+</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">Datenquelle: RKI Nowcast</span><span class="se">\n</span><span class="s2">Viz: @CorneliusRoemer&quot;</span><span class="p">,</span> <span class="n">size</span><span class="o">=</span><span class="mi">5</span><span class="p">,</span> <span class="n">va</span><span class="o">=</span><span class="s2">&quot;bottom&quot;</span><span class="p">,</span> <span class="n">ha</span><span class="o">=</span><span class="s2">&quot;right&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">savefig</span><span class="p">(</span><span class="s1">&#39;CasesLog.png&#39;</span><span class="p">,</span><span class="n">dpi</span><span class="o">=</span><span class="mi">400</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt"></div>



<div class="output_svg output_subarea ">
<?xml version="1.0" encoding="utf-8" standalone="no"?>
<!DOCTYPE svg PUBLIC "-//W3C//DTD SVG 1.1//EN"
  "http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd">
<!-- Created with matplotlib (https://matplotlib.org/) -->
<svg height="241.198125pt" version="1.1" viewBox="0 0 392.878125 241.198125" width="392.878125pt" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
 <defs>
  <style type="text/css">
*{stroke-linecap:butt;stroke-linejoin:round;}
  </style>
 </defs>
 <g id="figure_1">
  <g id="patch_1">
   <path d="M 0 241.198125 
L 392.878125 241.198125 
L 392.878125 -0 
L 0 -0 
z
" style="fill:#ffffff;"/>
  </g>
  <g id="axes_1">
   <g id="patch_2">
    <path d="M 45.478125 186.118125 
L 385.678125 186.118125 
L 385.678125 22.318125 
L 45.478125 22.318125 
z
" style="fill:#ffffff;"/>
   </g>
   <g id="PolyCollection_1">
    <defs>
     <path d="M 43.179476 -69.667017 
L 43.179476 -64.609395 
L 45.478125 -69.24059 
L 47.776774 -85.054699 
L 50.075422 -94.903843 
L 52.374071 -113.753259 
L 54.67272 -131.985054 
L 56.971368 -149.722454 
L 59.270017 -157.444046 
L 61.568666 -170.969231 
L 63.867314 -181.101582 
L 66.165963 -190.84372 
L 68.464611 -198.674706 
L 70.76326 -204.985043 
L 73.061909 -210.22389 
L 75.360557 -210.027879 
L 77.659206 -205.150688 
L 79.957855 -205.057894 
L 82.256503 -203.694254 
L 84.555152 -208.295371 
L 86.853801 -204.930314 
L 89.152449 -200.310894 
L 91.451098 -202.439788 
L 93.749747 -193.122604 
L 96.048395 -196.371849 
L 98.347044 -195.755658 
L 100.645693 -195.811082 
L 102.944341 -198.380954 
L 105.24299 -192.774753 
L 107.541639 -194.803553 
L 109.840287 -186.773945 
L 112.138936 -191.945799 
L 114.437584 -192.237518 
L 116.736233 -190.971974 
L 119.034882 -185.989611 
L 121.33353 -183.469622 
L 123.632179 -181.616943 
L 125.930828 -178.785751 
L 128.229476 -175.402334 
L 130.528125 -176.528625 
L 132.826774 -168.030291 
L 135.125422 -166.322507 
L 137.424071 -167.646991 
L 139.72272 -153.686024 
L 142.021368 -157.077628 
L 144.320017 -155.921788 
L 146.618666 -155.534607 
L 148.917314 -151.148836 
L 151.215963 -149.940172 
L 153.514611 -147.892479 
L 155.81326 -145.090148 
L 158.111909 -139.240197 
L 160.410557 -136.623748 
L 162.709206 -140.047203 
L 165.007855 -133.433719 
L 167.306503 -132.58199 
L 169.605152 -130.07534 
L 171.903801 -127.611111 
L 174.202449 -121.502788 
L 176.501098 -116.623422 
L 178.799747 -125.257511 
L 181.098395 -116.908337 
L 183.397044 -117.486439 
L 185.695693 -121.057779 
L 187.994341 -117.12334 
L 190.29299 -114.067756 
L 192.591639 -109.598188 
L 194.890287 -111.11228 
L 197.188936 -107.640584 
L 199.487584 -105.903779 
L 201.786233 -105.737741 
L 204.084882 -102.107944 
L 206.38353 -101.156957 
L 208.682179 -97.563024 
L 210.980828 -95.692411 
L 213.279476 -107.714605 
L 215.578125 -103.518594 
L 217.876774 -93.960945 
L 220.175422 -99.035333 
L 222.474071 -87.374327 
L 224.77272 -95.989013 
L 227.071368 -81.719585 
L 229.370017 -79.425055 
L 231.668666 -81.353875 
L 233.967314 -86.365717 
L 236.265963 -85.062729 
L 238.564611 -83.089526 
L 240.86326 -85.054699 
L 243.161909 -80.393451 
L 245.460557 -74.515362 
L 247.759206 -71.320182 
L 250.057855 -69.634516 
L 252.356503 -67.204785 
L 254.655152 -83.207325 
L 256.953801 -78.356867 
L 259.252449 -75.290987 
L 261.551098 -69.375614 
L 263.849747 -71.673147 
L 266.148395 -62.525455 
L 268.447044 -78.916446 
L 270.745693 -84.826857 
L 273.044341 -82.179408 
L 275.34299 -79.029637 
L 277.641639 -77.242724 
L 279.940287 -82.630249 
L 282.238936 -84.691023 
L 284.537584 -101.183299 
L 286.836233 -129.757695 
L 289.134882 -103.236077 
L 291.43353 -97.326305 
L 293.732179 -99.242867 
L 296.030828 -95.127537 
L 298.329476 -86.365717 
L 300.628125 -86.245394 
L 302.926774 -81.89536 
L 305.225422 -85.939572 
L 307.524071 -83.390541 
L 309.82272 -84.722093 
L 312.121368 -80.775519 
L 314.420017 -78.159228 
L 316.718666 -80.617996 
L 319.017314 -84.254705 
L 321.315963 -77.710788 
L 323.614611 -75.141212 
L 325.91326 -74.0702 
L 328.211909 -72.023536 
L 330.510557 -74.963452 
L 332.809206 -71.289393 
L 335.107855 -72.436899 
L 337.406503 -69.192396 
L 339.705152 -79.98836 
L 342.003801 -86.249858 
L 344.302449 -85.218272 
L 346.601098 -84.263059 
L 348.899747 -91.662749 
L 351.198395 -91.506167 
L 353.497044 -93.992381 
L 355.795693 -89.768859 
L 358.094341 -92.427868 
L 360.39299 -93.8153 
L 362.691639 -99.900232 
L 364.990287 -94.784503 
L 367.288936 -103.061458 
L 369.587584 -103.464845 
L 371.886233 -103.27333 
L 374.184882 -100.117263 
L 376.48353 -95.127537 
L 378.782179 -105.737741 
L 381.080828 -102.1842 
L 383.379476 -88.861265 
L 383.379476 -136.567446 
L 383.379476 -136.567446 
L 381.080828 -140.274355 
L 378.782179 -131.3279 
L 376.48353 -122.92172 
L 374.184882 -120.947535 
L 371.886233 -118.461304 
L 369.587584 -117.141135 
L 367.288936 -115.52989 
L 364.990287 -108.594108 
L 362.691639 -109.098439 
L 360.39299 -101.859976 
L 358.094341 -101.483989 
L 355.795693 -97.702801 
L 353.497044 -99.749178 
L 351.198395 -98.920001 
L 348.899747 -97.631877 
L 346.601098 -92.535008 
L 344.302449 -92.580067 
L 342.003801 -91.607283 
L 339.705152 -86.449092 
L 337.406503 -76.658625 
L 335.107855 -79.794507 
L 332.809206 -78.668368 
L 330.510557 -82.363149 
L 328.211909 -79.448162 
L 325.91326 -80.999065 
L 323.614611 -82.110385 
L 321.315963 -84.493254 
L 319.017314 -90.303524 
L 316.718666 -86.245394 
L 314.420017 -85.535673 
L 312.121368 -87.421226 
L 309.82272 -91.399927 
L 307.524071 -89.547136 
L 305.225422 -91.520393 
L 302.926774 -88.651645 
L 300.628125 -92.134758 
L 298.329476 -92.775625 
L 296.030828 -101.104007 
L 293.732179 -104.185639 
L 291.43353 -103.356741 
L 289.134882 -108.377707 
L 286.836233 -133.158702 
L 284.537584 -105.991311 
L 282.238936 -90.816047 
L 279.940287 -89.040158 
L 277.641639 -83.757176 
L 275.34299 -85.852774 
L 273.044341 -87.872841 
L 270.745693 -90.506069 
L 268.447044 -84.405143 
L 266.148395 -71.164622 
L 263.849747 -79.298387 
L 261.551098 -76.255843 
L 259.252449 -81.980472 
L 256.953801 -83.925164 
L 254.655152 -90.20193 
L 252.356503 -74.649576 
L 250.057855 -77.17283 
L 247.759206 -78.846236 
L 245.460557 -81.893954 
L 243.161909 -86.92087 
L 240.86326 -90.335073 
L 238.564611 -89.173989 
L 236.265963 -89.924019 
L 233.967314 -92.414246 
L 231.668666 -88.671375 
L 229.370017 -85.901588 
L 227.071368 -87.965717 
L 224.77272 -100.321135 
L 222.474071 -92.775904 
L 220.175422 -103.684416 
L 217.876774 -101.226649 
L 215.578125 -108.258163 
L 213.279476 -112.229226 
L 210.980828 -101.573931 
L 208.682179 -102.620645 
L 206.38353 -105.930416 
L 204.084882 -106.966732 
L 201.786233 -111.105826 
L 199.487584 -110.736804 
L 197.188936 -112.026824 
L 194.890287 -115.448361 
L 192.591639 -114.13074 
L 190.29299 -119.001499 
L 187.994341 -121.596921 
L 185.695693 -125.444957 
L 183.397044 -122.190696 
L 181.098395 -121.003646 
L 178.799747 -128.720523 
L 176.501098 -120.563488 
L 174.202449 -125.467193 
L 171.903801 -130.946897 
L 169.605152 -133.841173 
L 167.306503 -136.107605 
L 165.007855 -136.656045 
L 162.709206 -143.27362 
L 160.410557 -139.866934 
L 158.111909 -142.495886 
L 155.81326 -147.728173 
L 153.514611 -151.05947 
L 151.215963 -152.781416 
L 148.917314 -153.967371 
L 146.618666 -158.106323 
L 144.320017 -158.139814 
L 142.021368 -159.538598 
L 139.72272 -156.248484 
L 137.424071 -170.057485 
L 135.125422 -168.803095 
L 132.826774 -169.949429 
L 130.528125 -178.484574 
L 128.229476 -177.20391 
L 125.930828 -180.62952 
L 123.632179 -183.206924 
L 121.33353 -185.215379 
L 119.034882 -187.807278 
L 116.736233 -192.46295 
L 114.437584 -193.833048 
L 112.138936 -193.672627 
L 109.840287 -188.523588 
L 107.541639 -196.091862 
L 105.24299 -194.405616 
L 102.944341 -199.864173 
L 100.645693 -197.206955 
L 98.347044 -197.26373 
L 96.048395 -197.543506 
L 93.749747 -194.485483 
L 91.451098 -203.770834 
L 89.152449 -201.757825 
L 86.853801 -206.173564 
L 84.555152 -209.357348 
L 82.256503 -205.065717 
L 79.957855 -206.181035 
L 77.659206 -206.341663 
L 75.360557 -211.1036 
L 73.061909 -211.434545 
L 70.76326 -206.20557 
L 68.464611 -199.871686 
L 66.165963 -192.158954 
L 63.867314 -182.719397 
L 61.568666 -172.385022 
L 59.270017 -159.287815 
L 56.971368 -151.942228 
L 54.67272 -134.803854 
L 52.374071 -116.969371 
L 50.075422 -98.814889 
L 47.776774 -88.81104 
L 45.478125 -73.887252 
L 43.179476 -69.667017 
z
" id="m50935f5ad8"/>
    </defs>
    <g clip-path="url(#p362f9d746c)">
     <use style="fill:#008000;fill-opacity:0.3;" x="0" xlink:href="#m50935f5ad8" y="241.198125"/>
    </g>
   </g>
   <g id="matplotlib.axis_1">
    <g id="xtick_1">
     <g id="line2d_1">
      <defs>
       <path d="M 0 0 
L 0 3.5 
" id="m7d0f5b57da" style="stroke:#000000;stroke-width:0.8;"/>
      </defs>
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="45.478125" xlink:href="#m7d0f5b57da" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_2">
     <g id="line2d_2">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="112.138936" xlink:href="#m7d0f5b57da" y="186.118125"/>
      </g>
     </g>
     <g id="text_1">
      <!-- Apr -->
      <defs>
       <path d="M 34.1875 63.1875 
L 20.796875 26.90625 
L 47.609375 26.90625 
z
M 28.609375 72.90625 
L 39.796875 72.90625 
L 67.578125 0 
L 57.328125 0 
L 50.6875 18.703125 
L 17.828125 18.703125 
L 11.1875 0 
L 0.78125 0 
z
" id="DejaVuSans-65"/>
       <path d="M 18.109375 8.203125 
L 18.109375 -20.796875 
L 9.078125 -20.796875 
L 9.078125 54.6875 
L 18.109375 54.6875 
L 18.109375 46.390625 
Q 20.953125 51.265625 25.265625 53.625 
Q 29.59375 56 35.59375 56 
Q 45.5625 56 51.78125 48.09375 
Q 58.015625 40.1875 58.015625 27.296875 
Q 58.015625 14.40625 51.78125 6.484375 
Q 45.5625 -1.421875 35.59375 -1.421875 
Q 29.59375 -1.421875 25.265625 0.953125 
Q 20.953125 3.328125 18.109375 8.203125 
z
M 48.6875 27.296875 
Q 48.6875 37.203125 44.609375 42.84375 
Q 40.53125 48.484375 33.40625 48.484375 
Q 26.265625 48.484375 22.1875 42.84375 
Q 18.109375 37.203125 18.109375 27.296875 
Q 18.109375 17.390625 22.1875 11.75 
Q 26.265625 6.109375 33.40625 6.109375 
Q 40.53125 6.109375 44.609375 11.75 
Q 48.6875 17.390625 48.6875 27.296875 
z
" id="DejaVuSans-112"/>
       <path d="M 41.109375 46.296875 
Q 39.59375 47.171875 37.8125 47.578125 
Q 36.03125 48 33.890625 48 
Q 26.265625 48 22.1875 43.046875 
Q 18.109375 38.09375 18.109375 28.8125 
L 18.109375 0 
L 9.078125 0 
L 9.078125 54.6875 
L 18.109375 54.6875 
L 18.109375 46.1875 
Q 20.953125 51.171875 25.484375 53.578125 
Q 30.03125 56 36.53125 56 
Q 37.453125 56 38.578125 55.875 
Q 39.703125 55.765625 41.0625 55.515625 
z
" id="DejaVuSans-114"/>
      </defs>
      <g transform="translate(103.488936 202.216563)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-65"/>
       <use x="68.408203" xlink:href="#DejaVuSans-112"/>
       <use x="131.884766" xlink:href="#DejaVuSans-114"/>
      </g>
      <!-- 2020 -->
      <defs>
       <path d="M 19.1875 8.296875 
L 53.609375 8.296875 
L 53.609375 0 
L 7.328125 0 
L 7.328125 8.296875 
Q 12.9375 14.109375 22.625 23.890625 
Q 32.328125 33.6875 34.8125 36.53125 
Q 39.546875 41.84375 41.421875 45.53125 
Q 43.3125 49.21875 43.3125 52.78125 
Q 43.3125 58.59375 39.234375 62.25 
Q 35.15625 65.921875 28.609375 65.921875 
Q 23.96875 65.921875 18.8125 64.3125 
Q 13.671875 62.703125 7.8125 59.421875 
L 7.8125 69.390625 
Q 13.765625 71.78125 18.9375 73 
Q 24.125 74.21875 28.421875 74.21875 
Q 39.75 74.21875 46.484375 68.546875 
Q 53.21875 62.890625 53.21875 53.421875 
Q 53.21875 48.921875 51.53125 44.890625 
Q 49.859375 40.875 45.40625 35.40625 
Q 44.1875 33.984375 37.640625 27.21875 
Q 31.109375 20.453125 19.1875 8.296875 
z
" id="DejaVuSans-50"/>
       <path d="M 31.78125 66.40625 
Q 24.171875 66.40625 20.328125 58.90625 
Q 16.5 51.421875 16.5 36.375 
Q 16.5 21.390625 20.328125 13.890625 
Q 24.171875 6.390625 31.78125 6.390625 
Q 39.453125 6.390625 43.28125 13.890625 
Q 47.125 21.390625 47.125 36.375 
Q 47.125 51.421875 43.28125 58.90625 
Q 39.453125 66.40625 31.78125 66.40625 
z
M 31.78125 74.21875 
Q 44.046875 74.21875 50.515625 64.515625 
Q 56.984375 54.828125 56.984375 36.375 
Q 56.984375 17.96875 50.515625 8.265625 
Q 44.046875 -1.421875 31.78125 -1.421875 
Q 19.53125 -1.421875 13.0625 8.265625 
Q 6.59375 17.96875 6.59375 36.375 
Q 6.59375 54.828125 13.0625 64.515625 
Q 19.53125 74.21875 31.78125 74.21875 
z
" id="DejaVuSans-48"/>
      </defs>
      <g transform="translate(99.413936 213.414375)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
      </g>
     </g>
    </g>
    <g id="xtick_3">
     <g id="line2d_3">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="181.098395" xlink:href="#m7d0f5b57da" y="186.118125"/>
      </g>
     </g>
     <g id="text_2">
      <!-- Mai -->
      <defs>
       <path d="M 9.8125 72.90625 
L 24.515625 72.90625 
L 43.109375 23.296875 
L 61.8125 72.90625 
L 76.515625 72.90625 
L 76.515625 0 
L 66.890625 0 
L 66.890625 64.015625 
L 48.09375 14.015625 
L 38.1875 14.015625 
L 19.390625 64.015625 
L 19.390625 0 
L 9.8125 0 
z
" id="DejaVuSans-77"/>
       <path d="M 34.28125 27.484375 
Q 23.390625 27.484375 19.1875 25 
Q 14.984375 22.515625 14.984375 16.5 
Q 14.984375 11.71875 18.140625 8.90625 
Q 21.296875 6.109375 26.703125 6.109375 
Q 34.1875 6.109375 38.703125 11.40625 
Q 43.21875 16.703125 43.21875 25.484375 
L 43.21875 27.484375 
z
M 52.203125 31.203125 
L 52.203125 0 
L 43.21875 0 
L 43.21875 8.296875 
Q 40.140625 3.328125 35.546875 0.953125 
Q 30.953125 -1.421875 24.3125 -1.421875 
Q 15.921875 -1.421875 10.953125 3.296875 
Q 6 8.015625 6 15.921875 
Q 6 25.140625 12.171875 29.828125 
Q 18.359375 34.515625 30.609375 34.515625 
L 43.21875 34.515625 
L 43.21875 35.40625 
Q 43.21875 41.609375 39.140625 45 
Q 35.0625 48.390625 27.6875 48.390625 
Q 23 48.390625 18.546875 47.265625 
Q 14.109375 46.140625 10.015625 43.890625 
L 10.015625 52.203125 
Q 14.9375 54.109375 19.578125 55.046875 
Q 24.21875 56 28.609375 56 
Q 40.484375 56 46.34375 49.84375 
Q 52.203125 43.703125 52.203125 31.203125 
z
" id="DejaVuSans-97"/>
       <path d="M 9.421875 54.6875 
L 18.40625 54.6875 
L 18.40625 0 
L 9.421875 0 
z
M 9.421875 75.984375 
L 18.40625 75.984375 
L 18.40625 64.59375 
L 9.421875 64.59375 
z
" id="DejaVuSans-105"/>
      </defs>
      <g transform="translate(172.331208 202.216563)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-77"/>
       <use x="86.279297" xlink:href="#DejaVuSans-97"/>
       <use x="147.558594" xlink:href="#DejaVuSans-105"/>
      </g>
     </g>
    </g>
    <g id="xtick_4">
     <g id="line2d_4">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="252.356503" xlink:href="#m7d0f5b57da" y="186.118125"/>
      </g>
     </g>
     <g id="text_3">
      <!-- Jun -->
      <defs>
       <path d="M 9.8125 72.90625 
L 19.671875 72.90625 
L 19.671875 5.078125 
Q 19.671875 -8.109375 14.671875 -14.0625 
Q 9.671875 -20.015625 -1.421875 -20.015625 
L -5.171875 -20.015625 
L -5.171875 -11.71875 
L -2.09375 -11.71875 
Q 4.4375 -11.71875 7.125 -8.046875 
Q 9.8125 -4.390625 9.8125 5.078125 
z
" id="DejaVuSans-74"/>
       <path d="M 8.5 21.578125 
L 8.5 54.6875 
L 17.484375 54.6875 
L 17.484375 21.921875 
Q 17.484375 14.15625 20.5 10.265625 
Q 23.53125 6.390625 29.59375 6.390625 
Q 36.859375 6.390625 41.078125 11.03125 
Q 45.3125 15.671875 45.3125 23.6875 
L 45.3125 54.6875 
L 54.296875 54.6875 
L 54.296875 0 
L 45.3125 0 
L 45.3125 8.40625 
Q 42.046875 3.421875 37.71875 1 
Q 33.40625 -1.421875 27.6875 -1.421875 
Q 18.265625 -1.421875 13.375 4.4375 
Q 8.5 10.296875 8.5 21.578125 
z
M 31.109375 56 
z
" id="DejaVuSans-117"/>
       <path d="M 54.890625 33.015625 
L 54.890625 0 
L 45.90625 0 
L 45.90625 32.71875 
Q 45.90625 40.484375 42.875 44.328125 
Q 39.84375 48.1875 33.796875 48.1875 
Q 26.515625 48.1875 22.3125 43.546875 
Q 18.109375 38.921875 18.109375 30.90625 
L 18.109375 0 
L 9.078125 0 
L 9.078125 54.6875 
L 18.109375 54.6875 
L 18.109375 46.1875 
Q 21.34375 51.125 25.703125 53.5625 
Q 30.078125 56 35.796875 56 
Q 45.21875 56 50.046875 50.171875 
Q 54.890625 44.34375 54.890625 33.015625 
z
" id="DejaVuSans-110"/>
      </defs>
      <g transform="translate(244.544003 202.216563)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-74"/>
       <use x="29.492188" xlink:href="#DejaVuSans-117"/>
       <use x="92.871094" xlink:href="#DejaVuSans-110"/>
      </g>
     </g>
    </g>
    <g id="xtick_5">
     <g id="line2d_5">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="321.315963" xlink:href="#m7d0f5b57da" y="186.118125"/>
      </g>
     </g>
     <g id="text_4">
      <!-- Jul -->
      <defs>
       <path d="M 9.421875 75.984375 
L 18.40625 75.984375 
L 18.40625 0 
L 9.421875 0 
z
" id="DejaVuSans-108"/>
      </defs>
      <g transform="translate(315.28315 202.216563)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-74"/>
       <use x="29.492188" xlink:href="#DejaVuSans-117"/>
       <use x="92.871094" xlink:href="#DejaVuSans-108"/>
      </g>
     </g>
    </g>
    <g id="xtick_6">
     <g id="line2d_6">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="385.678125" xlink:href="#m7d0f5b57da" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_7">
     <g id="line2d_7">
      <defs>
       <path d="M 0 0 
L 0 2 
" id="md42fcfac78" style="stroke:#000000;stroke-width:0.6;"/>
      </defs>
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="59.270017" xlink:href="#md42fcfac78" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_8">
     <g id="line2d_8">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="75.360557" xlink:href="#md42fcfac78" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_9">
     <g id="line2d_9">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="91.451098" xlink:href="#md42fcfac78" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_10">
     <g id="line2d_10">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="107.541639" xlink:href="#md42fcfac78" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_11">
     <g id="line2d_11">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="123.632179" xlink:href="#md42fcfac78" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_12">
     <g id="line2d_12">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="139.72272" xlink:href="#md42fcfac78" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_13">
     <g id="line2d_13">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="155.81326" xlink:href="#md42fcfac78" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_14">
     <g id="line2d_14">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="171.903801" xlink:href="#md42fcfac78" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_15">
     <g id="line2d_15">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="187.994341" xlink:href="#md42fcfac78" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_16">
     <g id="line2d_16">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="204.084882" xlink:href="#md42fcfac78" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_17">
     <g id="line2d_17">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="220.175422" xlink:href="#md42fcfac78" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_18">
     <g id="line2d_18">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="236.265963" xlink:href="#md42fcfac78" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_19">
     <g id="line2d_19">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="268.447044" xlink:href="#md42fcfac78" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_20">
     <g id="line2d_20">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="284.537584" xlink:href="#md42fcfac78" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_21">
     <g id="line2d_21">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="300.628125" xlink:href="#md42fcfac78" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_22">
     <g id="line2d_22">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="316.718666" xlink:href="#md42fcfac78" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_23">
     <g id="line2d_23">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="332.809206" xlink:href="#md42fcfac78" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_24">
     <g id="line2d_24">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="348.899747" xlink:href="#md42fcfac78" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_25">
     <g id="line2d_25">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="364.990287" xlink:href="#md42fcfac78" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="xtick_26">
     <g id="line2d_26">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="381.080828" xlink:href="#md42fcfac78" y="186.118125"/>
      </g>
     </g>
    </g>
    <g id="text_5">
     <!-- Datum des Erkrankungsbeginns -->
     <defs>
      <path d="M 19.671875 64.796875 
L 19.671875 8.109375 
L 31.59375 8.109375 
Q 46.6875 8.109375 53.6875 14.9375 
Q 60.6875 21.78125 60.6875 36.53125 
Q 60.6875 51.171875 53.6875 57.984375 
Q 46.6875 64.796875 31.59375 64.796875 
z
M 9.8125 72.90625 
L 30.078125 72.90625 
Q 51.265625 72.90625 61.171875 64.09375 
Q 71.09375 55.28125 71.09375 36.53125 
Q 71.09375 17.671875 61.125 8.828125 
Q 51.171875 0 30.078125 0 
L 9.8125 0 
z
" id="DejaVuSans-68"/>
      <path d="M 18.3125 70.21875 
L 18.3125 54.6875 
L 36.8125 54.6875 
L 36.8125 47.703125 
L 18.3125 47.703125 
L 18.3125 18.015625 
Q 18.3125 11.328125 20.140625 9.421875 
Q 21.96875 7.515625 27.59375 7.515625 
L 36.8125 7.515625 
L 36.8125 0 
L 27.59375 0 
Q 17.1875 0 13.234375 3.875 
Q 9.28125 7.765625 9.28125 18.015625 
L 9.28125 47.703125 
L 2.6875 47.703125 
L 2.6875 54.6875 
L 9.28125 54.6875 
L 9.28125 70.21875 
z
" id="DejaVuSans-116"/>
      <path d="M 52 44.1875 
Q 55.375 50.25 60.0625 53.125 
Q 64.75 56 71.09375 56 
Q 79.640625 56 84.28125 50.015625 
Q 88.921875 44.046875 88.921875 33.015625 
L 88.921875 0 
L 79.890625 0 
L 79.890625 32.71875 
Q 79.890625 40.578125 77.09375 44.375 
Q 74.3125 48.1875 68.609375 48.1875 
Q 61.625 48.1875 57.5625 43.546875 
Q 53.515625 38.921875 53.515625 30.90625 
L 53.515625 0 
L 44.484375 0 
L 44.484375 32.71875 
Q 44.484375 40.625 41.703125 44.40625 
Q 38.921875 48.1875 33.109375 48.1875 
Q 26.21875 48.1875 22.15625 43.53125 
Q 18.109375 38.875 18.109375 30.90625 
L 18.109375 0 
L 9.078125 0 
L 9.078125 54.6875 
L 18.109375 54.6875 
L 18.109375 46.1875 
Q 21.1875 51.21875 25.484375 53.609375 
Q 29.78125 56 35.6875 56 
Q 41.65625 56 45.828125 52.96875 
Q 50 49.953125 52 44.1875 
z
" id="DejaVuSans-109"/>
      <path id="DejaVuSans-32"/>
      <path d="M 45.40625 46.390625 
L 45.40625 75.984375 
L 54.390625 75.984375 
L 54.390625 0 
L 45.40625 0 
L 45.40625 8.203125 
Q 42.578125 3.328125 38.25 0.953125 
Q 33.9375 -1.421875 27.875 -1.421875 
Q 17.96875 -1.421875 11.734375 6.484375 
Q 5.515625 14.40625 5.515625 27.296875 
Q 5.515625 40.1875 11.734375 48.09375 
Q 17.96875 56 27.875 56 
Q 33.9375 56 38.25 53.625 
Q 42.578125 51.265625 45.40625 46.390625 
z
M 14.796875 27.296875 
Q 14.796875 17.390625 18.875 11.75 
Q 22.953125 6.109375 30.078125 6.109375 
Q 37.203125 6.109375 41.296875 11.75 
Q 45.40625 17.390625 45.40625 27.296875 
Q 45.40625 37.203125 41.296875 42.84375 
Q 37.203125 48.484375 30.078125 48.484375 
Q 22.953125 48.484375 18.875 42.84375 
Q 14.796875 37.203125 14.796875 27.296875 
z
" id="DejaVuSans-100"/>
      <path d="M 56.203125 29.59375 
L 56.203125 25.203125 
L 14.890625 25.203125 
Q 15.484375 15.921875 20.484375 11.0625 
Q 25.484375 6.203125 34.421875 6.203125 
Q 39.59375 6.203125 44.453125 7.46875 
Q 49.3125 8.734375 54.109375 11.28125 
L 54.109375 2.78125 
Q 49.265625 0.734375 44.1875 -0.34375 
Q 39.109375 -1.421875 33.890625 -1.421875 
Q 20.796875 -1.421875 13.15625 6.1875 
Q 5.515625 13.8125 5.515625 26.8125 
Q 5.515625 40.234375 12.765625 48.109375 
Q 20.015625 56 32.328125 56 
Q 43.359375 56 49.78125 48.890625 
Q 56.203125 41.796875 56.203125 29.59375 
z
M 47.21875 32.234375 
Q 47.125 39.59375 43.09375 43.984375 
Q 39.0625 48.390625 32.421875 48.390625 
Q 24.90625 48.390625 20.390625 44.140625 
Q 15.875 39.890625 15.1875 32.171875 
z
" id="DejaVuSans-101"/>
      <path d="M 44.28125 53.078125 
L 44.28125 44.578125 
Q 40.484375 46.53125 36.375 47.5 
Q 32.28125 48.484375 27.875 48.484375 
Q 21.1875 48.484375 17.84375 46.4375 
Q 14.5 44.390625 14.5 40.28125 
Q 14.5 37.15625 16.890625 35.375 
Q 19.28125 33.59375 26.515625 31.984375 
L 29.59375 31.296875 
Q 39.15625 29.25 43.1875 25.515625 
Q 47.21875 21.78125 47.21875 15.09375 
Q 47.21875 7.46875 41.1875 3.015625 
Q 35.15625 -1.421875 24.609375 -1.421875 
Q 20.21875 -1.421875 15.453125 -0.5625 
Q 10.6875 0.296875 5.421875 2 
L 5.421875 11.28125 
Q 10.40625 8.6875 15.234375 7.390625 
Q 20.0625 6.109375 24.8125 6.109375 
Q 31.15625 6.109375 34.5625 8.28125 
Q 37.984375 10.453125 37.984375 14.40625 
Q 37.984375 18.0625 35.515625 20.015625 
Q 33.0625 21.96875 24.703125 23.78125 
L 21.578125 24.515625 
Q 13.234375 26.265625 9.515625 29.90625 
Q 5.8125 33.546875 5.8125 39.890625 
Q 5.8125 47.609375 11.28125 51.796875 
Q 16.75 56 26.8125 56 
Q 31.78125 56 36.171875 55.265625 
Q 40.578125 54.546875 44.28125 53.078125 
z
" id="DejaVuSans-115"/>
      <path d="M 9.8125 72.90625 
L 55.90625 72.90625 
L 55.90625 64.59375 
L 19.671875 64.59375 
L 19.671875 43.015625 
L 54.390625 43.015625 
L 54.390625 34.71875 
L 19.671875 34.71875 
L 19.671875 8.296875 
L 56.78125 8.296875 
L 56.78125 0 
L 9.8125 0 
z
" id="DejaVuSans-69"/>
      <path d="M 9.078125 75.984375 
L 18.109375 75.984375 
L 18.109375 31.109375 
L 44.921875 54.6875 
L 56.390625 54.6875 
L 27.390625 29.109375 
L 57.625 0 
L 45.90625 0 
L 18.109375 26.703125 
L 18.109375 0 
L 9.078125 0 
z
" id="DejaVuSans-107"/>
      <path d="M 45.40625 27.984375 
Q 45.40625 37.75 41.375 43.109375 
Q 37.359375 48.484375 30.078125 48.484375 
Q 22.859375 48.484375 18.828125 43.109375 
Q 14.796875 37.75 14.796875 27.984375 
Q 14.796875 18.265625 18.828125 12.890625 
Q 22.859375 7.515625 30.078125 7.515625 
Q 37.359375 7.515625 41.375 12.890625 
Q 45.40625 18.265625 45.40625 27.984375 
z
M 54.390625 6.78125 
Q 54.390625 -7.171875 48.1875 -13.984375 
Q 42 -20.796875 29.203125 -20.796875 
Q 24.46875 -20.796875 20.265625 -20.09375 
Q 16.0625 -19.390625 12.109375 -17.921875 
L 12.109375 -9.1875 
Q 16.0625 -11.328125 19.921875 -12.34375 
Q 23.78125 -13.375 27.78125 -13.375 
Q 36.625 -13.375 41.015625 -8.765625 
Q 45.40625 -4.15625 45.40625 5.171875 
L 45.40625 9.625 
Q 42.625 4.78125 38.28125 2.390625 
Q 33.9375 0 27.875 0 
Q 17.828125 0 11.671875 7.65625 
Q 5.515625 15.328125 5.515625 27.984375 
Q 5.515625 40.671875 11.671875 48.328125 
Q 17.828125 56 27.875 56 
Q 33.9375 56 38.28125 53.609375 
Q 42.625 51.21875 45.40625 46.390625 
L 45.40625 54.6875 
L 54.390625 54.6875 
z
" id="DejaVuSans-103"/>
      <path d="M 48.6875 27.296875 
Q 48.6875 37.203125 44.609375 42.84375 
Q 40.53125 48.484375 33.40625 48.484375 
Q 26.265625 48.484375 22.1875 42.84375 
Q 18.109375 37.203125 18.109375 27.296875 
Q 18.109375 17.390625 22.1875 11.75 
Q 26.265625 6.109375 33.40625 6.109375 
Q 40.53125 6.109375 44.609375 11.75 
Q 48.6875 17.390625 48.6875 27.296875 
z
M 18.109375 46.390625 
Q 20.953125 51.265625 25.265625 53.625 
Q 29.59375 56 35.59375 56 
Q 45.5625 56 51.78125 48.09375 
Q 58.015625 40.1875 58.015625 27.296875 
Q 58.015625 14.40625 51.78125 6.484375 
Q 45.5625 -1.421875 35.59375 -1.421875 
Q 29.59375 -1.421875 25.265625 0.953125 
Q 20.953125 3.328125 18.109375 8.203125 
L 18.109375 0 
L 9.078125 0 
L 9.078125 75.984375 
L 18.109375 75.984375 
z
" id="DejaVuSans-98"/>
     </defs>
     <g transform="translate(135.467187 227.0925)scale(0.1 -0.1)">
      <use xlink:href="#DejaVuSans-68"/>
      <use x="77.001953" xlink:href="#DejaVuSans-97"/>
      <use x="138.28125" xlink:href="#DejaVuSans-116"/>
      <use x="177.490234" xlink:href="#DejaVuSans-117"/>
      <use x="240.869141" xlink:href="#DejaVuSans-109"/>
      <use x="338.28125" xlink:href="#DejaVuSans-32"/>
      <use x="370.068359" xlink:href="#DejaVuSans-100"/>
      <use x="433.544922" xlink:href="#DejaVuSans-101"/>
      <use x="495.068359" xlink:href="#DejaVuSans-115"/>
      <use x="547.167969" xlink:href="#DejaVuSans-32"/>
      <use x="578.955078" xlink:href="#DejaVuSans-69"/>
      <use x="642.138672" xlink:href="#DejaVuSans-114"/>
      <use x="683.251953" xlink:href="#DejaVuSans-107"/>
      <use x="741.162109" xlink:href="#DejaVuSans-114"/>
      <use x="782.275391" xlink:href="#DejaVuSans-97"/>
      <use x="843.554688" xlink:href="#DejaVuSans-110"/>
      <use x="906.933594" xlink:href="#DejaVuSans-107"/>
      <use x="964.796875" xlink:href="#DejaVuSans-117"/>
      <use x="1028.175781" xlink:href="#DejaVuSans-110"/>
      <use x="1091.554688" xlink:href="#DejaVuSans-103"/>
      <use x="1155.03125" xlink:href="#DejaVuSans-115"/>
      <use x="1207.130859" xlink:href="#DejaVuSans-98"/>
      <use x="1270.607422" xlink:href="#DejaVuSans-101"/>
      <use x="1332.130859" xlink:href="#DejaVuSans-103"/>
      <use x="1395.607422" xlink:href="#DejaVuSans-105"/>
      <use x="1423.390625" xlink:href="#DejaVuSans-110"/>
      <use x="1486.769531" xlink:href="#DejaVuSans-110"/>
      <use x="1550.148438" xlink:href="#DejaVuSans-115"/>
     </g>
    </g>
   </g>
   <g id="matplotlib.axis_2">
    <g id="ytick_1">
     <g id="line2d_27">
      <path clip-path="url(#p362f9d746c)" d="M 45.478125 112.063862 
L 385.678125 112.063862 
" style="fill:none;stroke:#999999;stroke-linecap:square;stroke-opacity:0.15;stroke-width:0.8;"/>
     </g>
     <g id="line2d_28">
      <defs>
       <path d="M 0 0 
L -3.5 0 
" id="mafdb90430b" style="stroke:#000000;stroke-width:0.8;"/>
      </defs>
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="45.478125" xlink:href="#mafdb90430b" y="112.063862"/>
      </g>
     </g>
     <g id="text_6">
      <!-- $\mathdefault{10^{3}}$ -->
      <defs>
       <path d="M 12.40625 8.296875 
L 28.515625 8.296875 
L 28.515625 63.921875 
L 10.984375 60.40625 
L 10.984375 69.390625 
L 28.421875 72.90625 
L 38.28125 72.90625 
L 38.28125 8.296875 
L 54.390625 8.296875 
L 54.390625 0 
L 12.40625 0 
z
" id="DejaVuSans-49"/>
       <path d="M 40.578125 39.3125 
Q 47.65625 37.796875 51.625 33 
Q 55.609375 28.21875 55.609375 21.1875 
Q 55.609375 10.40625 48.1875 4.484375 
Q 40.765625 -1.421875 27.09375 -1.421875 
Q 22.515625 -1.421875 17.65625 -0.515625 
Q 12.796875 0.390625 7.625 2.203125 
L 7.625 11.71875 
Q 11.71875 9.328125 16.59375 8.109375 
Q 21.484375 6.890625 26.8125 6.890625 
Q 36.078125 6.890625 40.9375 10.546875 
Q 45.796875 14.203125 45.796875 21.1875 
Q 45.796875 27.640625 41.28125 31.265625 
Q 36.765625 34.90625 28.71875 34.90625 
L 20.21875 34.90625 
L 20.21875 43.015625 
L 29.109375 43.015625 
Q 36.375 43.015625 40.234375 45.921875 
Q 44.09375 48.828125 44.09375 54.296875 
Q 44.09375 59.90625 40.109375 62.90625 
Q 36.140625 65.921875 28.71875 65.921875 
Q 24.65625 65.921875 20.015625 65.03125 
Q 15.375 64.15625 9.8125 62.3125 
L 9.8125 71.09375 
Q 15.4375 72.65625 20.34375 73.4375 
Q 25.25 74.21875 29.59375 74.21875 
Q 40.828125 74.21875 47.359375 69.109375 
Q 53.90625 64.015625 53.90625 55.328125 
Q 53.90625 49.265625 50.4375 45.09375 
Q 46.96875 40.921875 40.578125 39.3125 
z
" id="DejaVuSans-51"/>
      </defs>
      <g transform="translate(20.878125 115.863081)scale(0.1 -0.1)">
       <use transform="translate(0 0.765625)" xlink:href="#DejaVuSans-49"/>
       <use transform="translate(63.623047 0.765625)" xlink:href="#DejaVuSans-48"/>
       <use transform="translate(128.203125 39.046875)scale(0.7)" xlink:href="#DejaVuSans-51"/>
      </g>
     </g>
    </g>
    <g id="ytick_2">
     <g id="line2d_29">
      <path clip-path="url(#p362f9d746c)" d="M 45.478125 169.85818 
L 385.678125 169.85818 
" style="fill:none;stroke:#999999;stroke-linecap:square;stroke-opacity:0.15;stroke-width:0.8;"/>
     </g>
     <g id="line2d_30">
      <defs>
       <path d="M 0 0 
L -2 0 
" id="m223f232fb1" style="stroke:#000000;stroke-width:0.6;"/>
      </defs>
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="45.478125" xlink:href="#m223f232fb1" y="169.85818"/>
      </g>
     </g>
    </g>
    <g id="ytick_3">
     <g id="line2d_31">
      <path clip-path="url(#p362f9d746c)" d="M 45.478125 156.048575 
L 385.678125 156.048575 
" style="fill:none;stroke:#999999;stroke-linecap:square;stroke-opacity:0.15;stroke-width:0.8;"/>
     </g>
     <g id="line2d_32">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="45.478125" xlink:href="#m223f232fb1" y="156.048575"/>
      </g>
     </g>
    </g>
    <g id="ytick_4">
     <g id="line2d_33">
      <path clip-path="url(#p362f9d746c)" d="M 45.478125 145.337013 
L 385.678125 145.337013 
" style="fill:none;stroke:#999999;stroke-linecap:square;stroke-opacity:0.15;stroke-width:0.8;"/>
     </g>
     <g id="line2d_34">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="45.478125" xlink:href="#m223f232fb1" y="145.337013"/>
      </g>
     </g>
    </g>
    <g id="ytick_5">
     <g id="line2d_35">
      <path clip-path="url(#p362f9d746c)" d="M 45.478125 136.585029 
L 385.678125 136.585029 
" style="fill:none;stroke:#999999;stroke-linecap:square;stroke-opacity:0.15;stroke-width:0.8;"/>
     </g>
     <g id="line2d_36">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="45.478125" xlink:href="#m223f232fb1" y="136.585029"/>
      </g>
     </g>
    </g>
    <g id="ytick_6">
     <g id="line2d_37">
      <path clip-path="url(#p362f9d746c)" d="M 45.478125 129.185333 
L 385.678125 129.185333 
" style="fill:none;stroke:#999999;stroke-linecap:square;stroke-opacity:0.15;stroke-width:0.8;"/>
     </g>
     <g id="line2d_38">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="45.478125" xlink:href="#m223f232fb1" y="129.185333"/>
      </g>
     </g>
    </g>
    <g id="ytick_7">
     <g id="line2d_39">
      <path clip-path="url(#p362f9d746c)" d="M 45.478125 122.775424 
L 385.678125 122.775424 
" style="fill:none;stroke:#999999;stroke-linecap:square;stroke-opacity:0.15;stroke-width:0.8;"/>
     </g>
     <g id="line2d_40">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="45.478125" xlink:href="#m223f232fb1" y="122.775424"/>
      </g>
     </g>
    </g>
    <g id="ytick_8">
     <g id="line2d_41">
      <path clip-path="url(#p362f9d746c)" d="M 45.478125 117.121484 
L 385.678125 117.121484 
" style="fill:none;stroke:#999999;stroke-linecap:square;stroke-opacity:0.15;stroke-width:0.8;"/>
     </g>
     <g id="line2d_42">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="45.478125" xlink:href="#m223f232fb1" y="117.121484"/>
      </g>
     </g>
    </g>
    <g id="ytick_9">
     <g id="line2d_43">
      <path clip-path="url(#p362f9d746c)" d="M 45.478125 78.790711 
L 385.678125 78.790711 
" style="fill:none;stroke:#999999;stroke-linecap:square;stroke-opacity:0.15;stroke-width:0.8;"/>
     </g>
     <g id="line2d_44">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="45.478125" xlink:href="#m223f232fb1" y="78.790711"/>
      </g>
     </g>
    </g>
    <g id="ytick_10">
     <g id="line2d_45">
      <path clip-path="url(#p362f9d746c)" d="M 45.478125 59.327166 
L 385.678125 59.327166 
" style="fill:none;stroke:#999999;stroke-linecap:square;stroke-opacity:0.15;stroke-width:0.8;"/>
     </g>
     <g id="line2d_46">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="45.478125" xlink:href="#m223f232fb1" y="59.327166"/>
      </g>
     </g>
    </g>
    <g id="ytick_11">
     <g id="line2d_47">
      <path clip-path="url(#p362f9d746c)" d="M 45.478125 45.51756 
L 385.678125 45.51756 
" style="fill:none;stroke:#999999;stroke-linecap:square;stroke-opacity:0.15;stroke-width:0.8;"/>
     </g>
     <g id="line2d_48">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="45.478125" xlink:href="#m223f232fb1" y="45.51756"/>
      </g>
     </g>
    </g>
    <g id="ytick_12">
     <g id="line2d_49">
      <path clip-path="url(#p362f9d746c)" d="M 45.478125 34.805998 
L 385.678125 34.805998 
" style="fill:none;stroke:#999999;stroke-linecap:square;stroke-opacity:0.15;stroke-width:0.8;"/>
     </g>
     <g id="line2d_50">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="45.478125" xlink:href="#m223f232fb1" y="34.805998"/>
      </g>
     </g>
    </g>
    <g id="ytick_13">
     <g id="line2d_51">
      <path clip-path="url(#p362f9d746c)" d="M 45.478125 26.054015 
L 385.678125 26.054015 
" style="fill:none;stroke:#999999;stroke-linecap:square;stroke-opacity:0.15;stroke-width:0.8;"/>
     </g>
     <g id="line2d_52">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="45.478125" xlink:href="#m223f232fb1" y="26.054015"/>
      </g>
     </g>
    </g>
    <g id="text_7">
     <!-- Saisonal bereinigte Fallzahlen -->
     <defs>
      <path d="M 53.515625 70.515625 
L 53.515625 60.890625 
Q 47.90625 63.578125 42.921875 64.890625 
Q 37.9375 66.21875 33.296875 66.21875 
Q 25.25 66.21875 20.875 63.09375 
Q 16.5 59.96875 16.5 54.203125 
Q 16.5 49.359375 19.40625 46.890625 
Q 22.3125 44.4375 30.421875 42.921875 
L 36.375 41.703125 
Q 47.40625 39.59375 52.65625 34.296875 
Q 57.90625 29 57.90625 20.125 
Q 57.90625 9.515625 50.796875 4.046875 
Q 43.703125 -1.421875 29.984375 -1.421875 
Q 24.8125 -1.421875 18.96875 -0.25 
Q 13.140625 0.921875 6.890625 3.21875 
L 6.890625 13.375 
Q 12.890625 10.015625 18.65625 8.296875 
Q 24.421875 6.59375 29.984375 6.59375 
Q 38.421875 6.59375 43.015625 9.90625 
Q 47.609375 13.234375 47.609375 19.390625 
Q 47.609375 24.75 44.3125 27.78125 
Q 41.015625 30.8125 33.5 32.328125 
L 27.484375 33.5 
Q 16.453125 35.6875 11.515625 40.375 
Q 6.59375 45.0625 6.59375 53.421875 
Q 6.59375 63.09375 13.40625 68.65625 
Q 20.21875 74.21875 32.171875 74.21875 
Q 37.3125 74.21875 42.625 73.28125 
Q 47.953125 72.359375 53.515625 70.515625 
z
" id="DejaVuSans-83"/>
      <path d="M 30.609375 48.390625 
Q 23.390625 48.390625 19.1875 42.75 
Q 14.984375 37.109375 14.984375 27.296875 
Q 14.984375 17.484375 19.15625 11.84375 
Q 23.34375 6.203125 30.609375 6.203125 
Q 37.796875 6.203125 41.984375 11.859375 
Q 46.1875 17.53125 46.1875 27.296875 
Q 46.1875 37.015625 41.984375 42.703125 
Q 37.796875 48.390625 30.609375 48.390625 
z
M 30.609375 56 
Q 42.328125 56 49.015625 48.375 
Q 55.71875 40.765625 55.71875 27.296875 
Q 55.71875 13.875 49.015625 6.21875 
Q 42.328125 -1.421875 30.609375 -1.421875 
Q 18.84375 -1.421875 12.171875 6.21875 
Q 5.515625 13.875 5.515625 27.296875 
Q 5.515625 40.765625 12.171875 48.375 
Q 18.84375 56 30.609375 56 
z
" id="DejaVuSans-111"/>
      <path d="M 9.8125 72.90625 
L 51.703125 72.90625 
L 51.703125 64.59375 
L 19.671875 64.59375 
L 19.671875 43.109375 
L 48.578125 43.109375 
L 48.578125 34.8125 
L 19.671875 34.8125 
L 19.671875 0 
L 9.8125 0 
z
" id="DejaVuSans-70"/>
      <path d="M 5.515625 54.6875 
L 48.1875 54.6875 
L 48.1875 46.484375 
L 14.40625 7.171875 
L 48.1875 7.171875 
L 48.1875 0 
L 4.296875 0 
L 4.296875 8.203125 
L 38.09375 47.515625 
L 5.515625 47.515625 
z
" id="DejaVuSans-122"/>
      <path d="M 54.890625 33.015625 
L 54.890625 0 
L 45.90625 0 
L 45.90625 32.71875 
Q 45.90625 40.484375 42.875 44.328125 
Q 39.84375 48.1875 33.796875 48.1875 
Q 26.515625 48.1875 22.3125 43.546875 
Q 18.109375 38.921875 18.109375 30.90625 
L 18.109375 0 
L 9.078125 0 
L 9.078125 75.984375 
L 18.109375 75.984375 
L 18.109375 46.1875 
Q 21.34375 51.125 25.703125 53.5625 
Q 30.078125 56 35.796875 56 
Q 45.21875 56 50.046875 50.171875 
Q 54.890625 44.34375 54.890625 33.015625 
z
" id="DejaVuSans-104"/>
     </defs>
     <g transform="translate(14.798438 179.050937)rotate(-90)scale(0.1 -0.1)">
      <use xlink:href="#DejaVuSans-83"/>
      <use x="63.476562" xlink:href="#DejaVuSans-97"/>
      <use x="124.755859" xlink:href="#DejaVuSans-105"/>
      <use x="152.539062" xlink:href="#DejaVuSans-115"/>
      <use x="204.638672" xlink:href="#DejaVuSans-111"/>
      <use x="265.820312" xlink:href="#DejaVuSans-110"/>
      <use x="329.199219" xlink:href="#DejaVuSans-97"/>
      <use x="390.478516" xlink:href="#DejaVuSans-108"/>
      <use x="418.261719" xlink:href="#DejaVuSans-32"/>
      <use x="450.048828" xlink:href="#DejaVuSans-98"/>
      <use x="513.525391" xlink:href="#DejaVuSans-101"/>
      <use x="575.048828" xlink:href="#DejaVuSans-114"/>
      <use x="616.130859" xlink:href="#DejaVuSans-101"/>
      <use x="677.654297" xlink:href="#DejaVuSans-105"/>
      <use x="705.4375" xlink:href="#DejaVuSans-110"/>
      <use x="768.816406" xlink:href="#DejaVuSans-105"/>
      <use x="796.599609" xlink:href="#DejaVuSans-103"/>
      <use x="860.076172" xlink:href="#DejaVuSans-116"/>
      <use x="899.285156" xlink:href="#DejaVuSans-101"/>
      <use x="960.808594" xlink:href="#DejaVuSans-32"/>
      <use x="992.595703" xlink:href="#DejaVuSans-70"/>
      <use x="1049.974609" xlink:href="#DejaVuSans-97"/>
      <use x="1111.253906" xlink:href="#DejaVuSans-108"/>
      <use x="1139.037109" xlink:href="#DejaVuSans-108"/>
      <use x="1166.820312" xlink:href="#DejaVuSans-122"/>
      <use x="1219.310547" xlink:href="#DejaVuSans-97"/>
      <use x="1280.589844" xlink:href="#DejaVuSans-104"/>
      <use x="1343.96875" xlink:href="#DejaVuSans-108"/>
      <use x="1371.751953" xlink:href="#DejaVuSans-101"/>
      <use x="1433.275391" xlink:href="#DejaVuSans-110"/>
     </g>
    </g>
   </g>
   <g id="line2d_53">
    <path clip-path="url(#p362f9d746c)" d="M 43.179476 174.151505 
L 45.478125 169.652948 
L 47.776774 154.174917 
L 50.075422 144.156143 
L 56.971368 90.424601 
L 59.270017 82.894301 
L 61.568666 69.53441 
L 63.867314 59.243732 
L 66.165963 49.77871 
L 68.464611 41.915708 
L 70.76326 35.582742 
L 73.061909 30.406145 
L 75.360557 30.625389 
L 77.659206 35.448256 
L 79.957855 35.593493 
L 82.256503 36.737115 
L 84.555152 32.35983 
L 86.853801 35.60434 
L 89.152449 40.152024 
L 91.451098 38.083548 
L 93.749747 47.400994 
L 96.048395 44.226026 
L 98.347044 44.718426 
L 100.645693 44.695666 
L 102.944341 42.082194 
L 105.24299 47.623057 
L 107.541639 45.778859 
L 109.840287 53.628271 
L 112.138936 48.428476 
L 114.437584 48.117631 
L 116.736233 49.436333 
L 119.034882 54.22735 
L 121.33353 56.812078 
L 123.632179 58.815429 
L 125.930828 61.458008 
L 128.229476 64.986732 
L 130.528125 63.663788 
L 132.826774 72.188359 
L 135.125422 73.619303 
L 137.424071 72.158924 
L 139.72272 86.175743 
L 142.021368 82.972761 
L 144.320017 84.117153 
L 146.618666 84.36044 
L 148.917314 88.633864 
L 151.215963 89.799607 
L 153.514611 91.585728 
L 155.81326 94.907455 
L 158.111909 100.408729 
L 160.410557 102.9254 
L 162.709206 99.736155 
L 165.007855 106.063502 
L 167.306503 106.820967 
L 169.605152 109.282534 
L 171.903801 112.128918 
L 174.202449 117.570734 
L 176.501098 122.536533 
L 178.799747 114.279804 
L 181.098395 122.198473 
L 183.397044 121.398637 
L 185.695693 117.611581 
L 187.994341 122.159882 
L 190.29299 124.424411 
L 192.591639 129.439928 
L 194.890287 128.072408 
L 197.188936 131.173155 
L 199.487584 132.776129 
L 201.786233 132.701343 
L 204.084882 136.708148 
L 206.38353 137.749231 
L 208.682179 141.121281 
L 210.980828 142.383236 
L 213.279476 131.31434 
L 215.578125 135.380605 
L 217.876774 143.629623 
L 220.175422 139.937089 
L 222.474071 151.098004 
L 224.77272 143.036659 
L 227.071368 156.560682 
L 229.370017 158.675027 
L 231.668666 156.112641 
L 233.967314 151.906111 
L 236.265963 153.488474 
L 238.564611 154.914822 
L 240.86326 153.325284 
L 243.161909 157.555599 
L 245.460557 162.988401 
L 247.759206 166.295239 
L 252.356503 170.053976 
L 254.655152 154.475432 
L 256.953801 159.976415 
L 259.252449 162.585304 
L 261.551098 168.182979 
L 263.849747 165.480228 
L 266.148395 173.954294 
L 268.447044 159.168174 
L 270.745693 153.716047 
L 275.34299 158.958177 
L 277.641639 160.718017 
L 279.940287 155.452342 
L 282.238936 153.747548 
L 284.537584 137.884391 
L 286.836233 109.388147 
L 289.134882 134.926151 
L 291.43353 141.028404 
L 293.732179 139.378449 
L 296.030828 143.242985 
L 298.329476 151.648722 
L 300.628125 152.368523 
L 302.926774 155.693567 
L 305.225422 152.181063 
L 307.524071 154.867705 
L 309.82272 153.021087 
L 312.121368 157.188384 
L 314.420017 159.737881 
L 316.718666 157.796566 
L 319.017314 154.040028 
L 321.315963 159.735193 
L 323.614611 162.585304 
L 325.91326 163.400447 
L 328.211909 165.642127 
L 330.510557 162.232105 
L 332.809206 165.877168 
L 335.107855 164.941594 
L 337.406503 168.127602 
L 339.705152 158.060898 
L 342.003801 152.140273 
L 344.302449 151.913676 
L 346.601098 152.425068 
L 348.899747 146.413622 
L 351.198395 145.614227 
L 353.497044 144.154058 
L 355.795693 147.501969 
L 358.094341 143.84503 
L 360.39299 143.344794 
L 362.691639 136.572473 
L 364.990287 138.4835 
L 367.288936 132.009617 
L 369.587584 130.344453 
L 371.886233 130.156802 
L 374.184882 129.103739 
L 376.48353 129.382556 
L 378.782179 121.627882 
L 381.080828 116.786854 
L 383.379476 122.308391 
L 383.379476 122.308391 
" style="fill:none;stroke:#1f77b4;stroke-linecap:square;stroke-width:1.5;"/>
   </g>
   <g id="patch_3">
    <path d="M 45.478125 186.118125 
L 45.478125 22.318125 
" style="fill:none;stroke:#000000;stroke-linecap:square;stroke-linejoin:miter;stroke-width:0.8;"/>
   </g>
   <g id="patch_4">
    <path d="M 385.678125 186.118125 
L 385.678125 22.318125 
" style="fill:none;stroke:#000000;stroke-linecap:square;stroke-linejoin:miter;stroke-width:0.8;"/>
   </g>
   <g id="patch_5">
    <path d="M 45.478125 186.118125 
L 385.678125 186.118125 
" style="fill:none;stroke:#000000;stroke-linecap:square;stroke-linejoin:miter;stroke-width:0.8;"/>
   </g>
   <g id="patch_6">
    <path d="M 45.478125 22.318125 
L 385.678125 22.318125 
" style="fill:none;stroke:#000000;stroke-linecap:square;stroke-linejoin:miter;stroke-width:0.8;"/>
   </g>
   <g id="text_8">
    <!-- Logarithmische Darstellung der deutschen Fallzahlen -->
    <defs>
     <path d="M 9.8125 72.90625 
L 19.671875 72.90625 
L 19.671875 8.296875 
L 55.171875 8.296875 
L 55.171875 0 
L 9.8125 0 
z
" id="DejaVuSans-76"/>
     <path d="M 48.78125 52.59375 
L 48.78125 44.1875 
Q 44.96875 46.296875 41.140625 47.34375 
Q 37.3125 48.390625 33.40625 48.390625 
Q 24.65625 48.390625 19.8125 42.84375 
Q 14.984375 37.3125 14.984375 27.296875 
Q 14.984375 17.28125 19.8125 11.734375 
Q 24.65625 6.203125 33.40625 6.203125 
Q 37.3125 6.203125 41.140625 7.25 
Q 44.96875 8.296875 48.78125 10.40625 
L 48.78125 2.09375 
Q 45.015625 0.34375 40.984375 -0.53125 
Q 36.96875 -1.421875 32.421875 -1.421875 
Q 20.0625 -1.421875 12.78125 6.34375 
Q 5.515625 14.109375 5.515625 27.296875 
Q 5.515625 40.671875 12.859375 48.328125 
Q 20.21875 56 33.015625 56 
Q 37.15625 56 41.109375 55.140625 
Q 45.0625 54.296875 48.78125 52.59375 
z
" id="DejaVuSans-99"/>
    </defs>
    <g transform="translate(55.464375 16.318125)scale(0.12 -0.12)">
     <use xlink:href="#DejaVuSans-76"/>
     <use x="55.697266" xlink:href="#DejaVuSans-111"/>
     <use x="116.878906" xlink:href="#DejaVuSans-103"/>
     <use x="180.355469" xlink:href="#DejaVuSans-97"/>
     <use x="241.634766" xlink:href="#DejaVuSans-114"/>
     <use x="282.748047" xlink:href="#DejaVuSans-105"/>
     <use x="310.53125" xlink:href="#DejaVuSans-116"/>
     <use x="349.740234" xlink:href="#DejaVuSans-104"/>
     <use x="413.119141" xlink:href="#DejaVuSans-109"/>
     <use x="510.53125" xlink:href="#DejaVuSans-105"/>
     <use x="538.314453" xlink:href="#DejaVuSans-115"/>
     <use x="590.414062" xlink:href="#DejaVuSans-99"/>
     <use x="645.394531" xlink:href="#DejaVuSans-104"/>
     <use x="708.773438" xlink:href="#DejaVuSans-101"/>
     <use x="770.296875" xlink:href="#DejaVuSans-32"/>
     <use x="802.083984" xlink:href="#DejaVuSans-68"/>
     <use x="879.085938" xlink:href="#DejaVuSans-97"/>
     <use x="940.365234" xlink:href="#DejaVuSans-114"/>
     <use x="981.478516" xlink:href="#DejaVuSans-115"/>
     <use x="1033.578125" xlink:href="#DejaVuSans-116"/>
     <use x="1072.787109" xlink:href="#DejaVuSans-101"/>
     <use x="1134.310547" xlink:href="#DejaVuSans-108"/>
     <use x="1162.09375" xlink:href="#DejaVuSans-108"/>
     <use x="1189.876953" xlink:href="#DejaVuSans-117"/>
     <use x="1253.255859" xlink:href="#DejaVuSans-110"/>
     <use x="1316.634766" xlink:href="#DejaVuSans-103"/>
     <use x="1380.111328" xlink:href="#DejaVuSans-32"/>
     <use x="1411.898438" xlink:href="#DejaVuSans-100"/>
     <use x="1475.375" xlink:href="#DejaVuSans-101"/>
     <use x="1536.898438" xlink:href="#DejaVuSans-114"/>
     <use x="1578.011719" xlink:href="#DejaVuSans-32"/>
     <use x="1609.798828" xlink:href="#DejaVuSans-100"/>
     <use x="1673.275391" xlink:href="#DejaVuSans-101"/>
     <use x="1734.798828" xlink:href="#DejaVuSans-117"/>
     <use x="1798.177734" xlink:href="#DejaVuSans-116"/>
     <use x="1837.386719" xlink:href="#DejaVuSans-115"/>
     <use x="1889.486328" xlink:href="#DejaVuSans-99"/>
     <use x="1944.466797" xlink:href="#DejaVuSans-104"/>
     <use x="2007.845703" xlink:href="#DejaVuSans-101"/>
     <use x="2069.369141" xlink:href="#DejaVuSans-110"/>
     <use x="2132.748047" xlink:href="#DejaVuSans-32"/>
     <use x="2164.535156" xlink:href="#DejaVuSans-70"/>
     <use x="2221.914062" xlink:href="#DejaVuSans-97"/>
     <use x="2283.193359" xlink:href="#DejaVuSans-108"/>
     <use x="2310.976562" xlink:href="#DejaVuSans-108"/>
     <use x="2338.759766" xlink:href="#DejaVuSans-122"/>
     <use x="2391.25" xlink:href="#DejaVuSans-97"/>
     <use x="2452.529297" xlink:href="#DejaVuSans-104"/>
     <use x="2515.908203" xlink:href="#DejaVuSans-108"/>
     <use x="2543.691406" xlink:href="#DejaVuSans-101"/>
     <use x="2605.214844" xlink:href="#DejaVuSans-110"/>
    </g>
   </g>
   <g id="legend_1">
    <g id="patch_7">
     <path d="M 226.392188 38.916562 
L 246.392188 38.916562 
L 246.392188 31.916562 
L 226.392188 31.916562 
z
" style="fill:#008000;opacity:0.3;"/>
    </g>
    <g id="text_9">
     <!-- 95%-Prädiktionsintervall -->
     <defs>
      <path d="M 10.984375 1.515625 
L 10.984375 10.5 
Q 14.703125 8.734375 18.5 7.8125 
Q 22.3125 6.890625 25.984375 6.890625 
Q 35.75 6.890625 40.890625 13.453125 
Q 46.046875 20.015625 46.78125 33.40625 
Q 43.953125 29.203125 39.59375 26.953125 
Q 35.25 24.703125 29.984375 24.703125 
Q 19.046875 24.703125 12.671875 31.3125 
Q 6.296875 37.9375 6.296875 49.421875 
Q 6.296875 60.640625 12.9375 67.421875 
Q 19.578125 74.21875 30.609375 74.21875 
Q 43.265625 74.21875 49.921875 64.515625 
Q 56.59375 54.828125 56.59375 36.375 
Q 56.59375 19.140625 48.40625 8.859375 
Q 40.234375 -1.421875 26.421875 -1.421875 
Q 22.703125 -1.421875 18.890625 -0.6875 
Q 15.09375 0.046875 10.984375 1.515625 
z
M 30.609375 32.421875 
Q 37.25 32.421875 41.125 36.953125 
Q 45.015625 41.5 45.015625 49.421875 
Q 45.015625 57.28125 41.125 61.84375 
Q 37.25 66.40625 30.609375 66.40625 
Q 23.96875 66.40625 20.09375 61.84375 
Q 16.21875 57.28125 16.21875 49.421875 
Q 16.21875 41.5 20.09375 36.953125 
Q 23.96875 32.421875 30.609375 32.421875 
z
" id="DejaVuSans-57"/>
      <path d="M 10.796875 72.90625 
L 49.515625 72.90625 
L 49.515625 64.59375 
L 19.828125 64.59375 
L 19.828125 46.734375 
Q 21.96875 47.46875 24.109375 47.828125 
Q 26.265625 48.1875 28.421875 48.1875 
Q 40.625 48.1875 47.75 41.5 
Q 54.890625 34.8125 54.890625 23.390625 
Q 54.890625 11.625 47.5625 5.09375 
Q 40.234375 -1.421875 26.90625 -1.421875 
Q 22.3125 -1.421875 17.546875 -0.640625 
Q 12.796875 0.140625 7.71875 1.703125 
L 7.71875 11.625 
Q 12.109375 9.234375 16.796875 8.0625 
Q 21.484375 6.890625 26.703125 6.890625 
Q 35.15625 6.890625 40.078125 11.328125 
Q 45.015625 15.765625 45.015625 23.390625 
Q 45.015625 31 40.078125 35.4375 
Q 35.15625 39.890625 26.703125 39.890625 
Q 22.75 39.890625 18.8125 39.015625 
Q 14.890625 38.140625 10.796875 36.28125 
z
" id="DejaVuSans-53"/>
      <path d="M 72.703125 32.078125 
Q 68.453125 32.078125 66.03125 28.46875 
Q 63.625 24.859375 63.625 18.40625 
Q 63.625 12.0625 66.03125 8.421875 
Q 68.453125 4.78125 72.703125 4.78125 
Q 76.859375 4.78125 79.265625 8.421875 
Q 81.6875 12.0625 81.6875 18.40625 
Q 81.6875 24.8125 79.265625 28.4375 
Q 76.859375 32.078125 72.703125 32.078125 
z
M 72.703125 38.28125 
Q 80.421875 38.28125 84.953125 32.90625 
Q 89.5 27.546875 89.5 18.40625 
Q 89.5 9.28125 84.9375 3.921875 
Q 80.375 -1.421875 72.703125 -1.421875 
Q 64.890625 -1.421875 60.34375 3.921875 
Q 55.8125 9.28125 55.8125 18.40625 
Q 55.8125 27.59375 60.375 32.9375 
Q 64.9375 38.28125 72.703125 38.28125 
z
M 22.3125 68.015625 
Q 18.109375 68.015625 15.6875 64.375 
Q 13.28125 60.75 13.28125 54.390625 
Q 13.28125 47.953125 15.671875 44.328125 
Q 18.0625 40.71875 22.3125 40.71875 
Q 26.5625 40.71875 28.96875 44.328125 
Q 31.390625 47.953125 31.390625 54.390625 
Q 31.390625 60.6875 28.953125 64.34375 
Q 26.515625 68.015625 22.3125 68.015625 
z
M 66.40625 74.21875 
L 74.21875 74.21875 
L 28.609375 -1.421875 
L 20.796875 -1.421875 
z
M 22.3125 74.21875 
Q 30.03125 74.21875 34.609375 68.875 
Q 39.203125 63.53125 39.203125 54.390625 
Q 39.203125 45.171875 34.640625 39.84375 
Q 30.078125 34.515625 22.3125 34.515625 
Q 14.546875 34.515625 10.03125 39.859375 
Q 5.515625 45.21875 5.515625 54.390625 
Q 5.515625 63.484375 10.046875 68.84375 
Q 14.59375 74.21875 22.3125 74.21875 
z
" id="DejaVuSans-37"/>
      <path d="M 4.890625 31.390625 
L 31.203125 31.390625 
L 31.203125 23.390625 
L 4.890625 23.390625 
z
" id="DejaVuSans-45"/>
      <path d="M 19.671875 64.796875 
L 19.671875 37.40625 
L 32.078125 37.40625 
Q 38.96875 37.40625 42.71875 40.96875 
Q 46.484375 44.53125 46.484375 51.125 
Q 46.484375 57.671875 42.71875 61.234375 
Q 38.96875 64.796875 32.078125 64.796875 
z
M 9.8125 72.90625 
L 32.078125 72.90625 
Q 44.34375 72.90625 50.609375 67.359375 
Q 56.890625 61.8125 56.890625 51.125 
Q 56.890625 40.328125 50.609375 34.8125 
Q 44.34375 29.296875 32.078125 29.296875 
L 19.671875 29.296875 
L 19.671875 0 
L 9.8125 0 
z
" id="DejaVuSans-80"/>
      <path d="M 34.28125 27.484375 
Q 23.390625 27.484375 19.1875 25 
Q 14.984375 22.515625 14.984375 16.5 
Q 14.984375 11.71875 18.140625 8.90625 
Q 21.296875 6.109375 26.703125 6.109375 
Q 34.1875 6.109375 38.703125 11.40625 
Q 43.21875 16.703125 43.21875 25.484375 
L 43.21875 27.484375 
z
M 52.203125 31.203125 
L 52.203125 0 
L 43.21875 0 
L 43.21875 8.296875 
Q 40.140625 3.328125 35.546875 0.953125 
Q 30.953125 -1.421875 24.3125 -1.421875 
Q 15.921875 -1.421875 10.953125 3.296875 
Q 6 8.015625 6 15.921875 
Q 6 25.140625 12.171875 29.828125 
Q 18.359375 34.515625 30.609375 34.515625 
L 43.21875 34.515625 
L 43.21875 35.40625 
Q 43.21875 41.609375 39.140625 45 
Q 35.0625 48.390625 27.6875 48.390625 
Q 23 48.390625 18.546875 47.265625 
Q 14.109375 46.140625 10.015625 43.890625 
L 10.015625 52.203125 
Q 14.9375 54.109375 19.578125 55.046875 
Q 24.21875 56 28.609375 56 
Q 40.484375 56 46.34375 49.84375 
Q 52.203125 43.703125 52.203125 31.203125 
z
M 33.59375 75.78125 
L 43.5 75.78125 
L 43.5 65.921875 
L 33.59375 65.921875 
z
M 14.5 75.78125 
L 24.421875 75.78125 
L 24.421875 65.921875 
L 14.5 65.921875 
z
" id="DejaVuSans-228"/>
      <path d="M 2.984375 54.6875 
L 12.5 54.6875 
L 29.59375 8.796875 
L 46.6875 54.6875 
L 56.203125 54.6875 
L 35.6875 0 
L 23.484375 0 
z
" id="DejaVuSans-118"/>
     </defs>
     <g transform="translate(254.392188 38.916562)scale(0.1 -0.1)">
      <use xlink:href="#DejaVuSans-57"/>
      <use x="63.623047" xlink:href="#DejaVuSans-53"/>
      <use x="127.246094" xlink:href="#DejaVuSans-37"/>
      <use x="222.265625" xlink:href="#DejaVuSans-45"/>
      <use x="258.349609" xlink:href="#DejaVuSans-80"/>
      <use x="318.636719" xlink:href="#DejaVuSans-114"/>
      <use x="359.75" xlink:href="#DejaVuSans-228"/>
      <use x="421.029297" xlink:href="#DejaVuSans-100"/>
      <use x="484.505859" xlink:href="#DejaVuSans-105"/>
      <use x="512.289062" xlink:href="#DejaVuSans-107"/>
      <use x="570.199219" xlink:href="#DejaVuSans-116"/>
      <use x="609.408203" xlink:href="#DejaVuSans-105"/>
      <use x="637.191406" xlink:href="#DejaVuSans-111"/>
      <use x="698.373047" xlink:href="#DejaVuSans-110"/>
      <use x="761.751953" xlink:href="#DejaVuSans-115"/>
      <use x="813.851562" xlink:href="#DejaVuSans-105"/>
      <use x="841.634766" xlink:href="#DejaVuSans-110"/>
      <use x="905.013672" xlink:href="#DejaVuSans-116"/>
      <use x="944.222656" xlink:href="#DejaVuSans-101"/>
      <use x="1005.746094" xlink:href="#DejaVuSans-114"/>
      <use x="1046.859375" xlink:href="#DejaVuSans-118"/>
      <use x="1106.039062" xlink:href="#DejaVuSans-97"/>
      <use x="1167.318359" xlink:href="#DejaVuSans-108"/>
      <use x="1195.101562" xlink:href="#DejaVuSans-108"/>
     </g>
    </g>
   </g>
  </g>
  <g id="text_10">
   <!-- Datenstand: 1. August 2020 -->
   <defs>
    <path d="M 11.71875 12.40625 
L 22.015625 12.40625 
L 22.015625 0 
L 11.71875 0 
z
M 11.71875 51.703125 
L 22.015625 51.703125 
L 22.015625 39.3125 
L 11.71875 39.3125 
z
" id="DejaVuSans-58"/>
    <path d="M 10.6875 12.40625 
L 21 12.40625 
L 21 0 
L 10.6875 0 
z
" id="DejaVuSans-46"/>
   </defs>
   <g transform="translate(315.142969 221.760469)scale(0.05 -0.05)">
    <use xlink:href="#DejaVuSans-68"/>
    <use x="77.001953" xlink:href="#DejaVuSans-97"/>
    <use x="138.28125" xlink:href="#DejaVuSans-116"/>
    <use x="177.490234" xlink:href="#DejaVuSans-101"/>
    <use x="239.013672" xlink:href="#DejaVuSans-110"/>
    <use x="302.392578" xlink:href="#DejaVuSans-115"/>
    <use x="354.492188" xlink:href="#DejaVuSans-116"/>
    <use x="393.701172" xlink:href="#DejaVuSans-97"/>
    <use x="454.980469" xlink:href="#DejaVuSans-110"/>
    <use x="518.359375" xlink:href="#DejaVuSans-100"/>
    <use x="581.835938" xlink:href="#DejaVuSans-58"/>
    <use x="615.527344" xlink:href="#DejaVuSans-32"/>
    <use x="647.314453" xlink:href="#DejaVuSans-49"/>
    <use x="710.9375" xlink:href="#DejaVuSans-46"/>
    <use x="742.724609" xlink:href="#DejaVuSans-32"/>
    <use x="774.511719" xlink:href="#DejaVuSans-65"/>
    <use x="842.919922" xlink:href="#DejaVuSans-117"/>
    <use x="906.298828" xlink:href="#DejaVuSans-103"/>
    <use x="969.775391" xlink:href="#DejaVuSans-117"/>
    <use x="1033.154297" xlink:href="#DejaVuSans-115"/>
    <use x="1085.253906" xlink:href="#DejaVuSans-116"/>
    <use x="1124.462891" xlink:href="#DejaVuSans-32"/>
    <use x="1156.25" xlink:href="#DejaVuSans-50"/>
    <use x="1219.873047" xlink:href="#DejaVuSans-48"/>
    <use x="1283.496094" xlink:href="#DejaVuSans-50"/>
    <use x="1347.119141" xlink:href="#DejaVuSans-48"/>
   </g>
   <!-- Datenquelle: RKI Nowcast -->
   <defs>
    <path d="M 14.796875 27.296875 
Q 14.796875 17.390625 18.875 11.75 
Q 22.953125 6.109375 30.078125 6.109375 
Q 37.203125 6.109375 41.296875 11.75 
Q 45.40625 17.390625 45.40625 27.296875 
Q 45.40625 37.203125 41.296875 42.84375 
Q 37.203125 48.484375 30.078125 48.484375 
Q 22.953125 48.484375 18.875 42.84375 
Q 14.796875 37.203125 14.796875 27.296875 
z
M 45.40625 8.203125 
Q 42.578125 3.328125 38.25 0.953125 
Q 33.9375 -1.421875 27.875 -1.421875 
Q 17.96875 -1.421875 11.734375 6.484375 
Q 5.515625 14.40625 5.515625 27.296875 
Q 5.515625 40.1875 11.734375 48.09375 
Q 17.96875 56 27.875 56 
Q 33.9375 56 38.25 53.625 
Q 42.578125 51.265625 45.40625 46.390625 
L 45.40625 54.6875 
L 54.390625 54.6875 
L 54.390625 -20.796875 
L 45.40625 -20.796875 
z
" id="DejaVuSans-113"/>
    <path d="M 44.390625 34.1875 
Q 47.5625 33.109375 50.5625 29.59375 
Q 53.5625 26.078125 56.59375 19.921875 
L 66.609375 0 
L 56 0 
L 46.6875 18.703125 
Q 43.0625 26.03125 39.671875 28.421875 
Q 36.28125 30.8125 30.421875 30.8125 
L 19.671875 30.8125 
L 19.671875 0 
L 9.8125 0 
L 9.8125 72.90625 
L 32.078125 72.90625 
Q 44.578125 72.90625 50.734375 67.671875 
Q 56.890625 62.453125 56.890625 51.90625 
Q 56.890625 45.015625 53.6875 40.46875 
Q 50.484375 35.9375 44.390625 34.1875 
z
M 19.671875 64.796875 
L 19.671875 38.921875 
L 32.078125 38.921875 
Q 39.203125 38.921875 42.84375 42.21875 
Q 46.484375 45.515625 46.484375 51.90625 
Q 46.484375 58.296875 42.84375 61.546875 
Q 39.203125 64.796875 32.078125 64.796875 
z
" id="DejaVuSans-82"/>
    <path d="M 9.8125 72.90625 
L 19.671875 72.90625 
L 19.671875 42.09375 
L 52.390625 72.90625 
L 65.09375 72.90625 
L 28.90625 38.921875 
L 67.671875 0 
L 54.6875 0 
L 19.671875 35.109375 
L 19.671875 0 
L 9.8125 0 
z
" id="DejaVuSans-75"/>
    <path d="M 9.8125 72.90625 
L 19.671875 72.90625 
L 19.671875 0 
L 9.8125 0 
z
" id="DejaVuSans-73"/>
    <path d="M 9.8125 72.90625 
L 23.09375 72.90625 
L 55.421875 11.921875 
L 55.421875 72.90625 
L 64.984375 72.90625 
L 64.984375 0 
L 51.703125 0 
L 19.390625 60.984375 
L 19.390625 0 
L 9.8125 0 
z
" id="DejaVuSans-78"/>
    <path d="M 4.203125 54.6875 
L 13.1875 54.6875 
L 24.421875 12.015625 
L 35.59375 54.6875 
L 46.1875 54.6875 
L 57.421875 12.015625 
L 68.609375 54.6875 
L 77.59375 54.6875 
L 63.28125 0 
L 52.6875 0 
L 40.921875 44.828125 
L 29.109375 0 
L 18.5 0 
z
" id="DejaVuSans-119"/>
   </defs>
   <g transform="translate(320.926563 227.359375)scale(0.05 -0.05)">
    <use xlink:href="#DejaVuSans-68"/>
    <use x="77.001953" xlink:href="#DejaVuSans-97"/>
    <use x="138.28125" xlink:href="#DejaVuSans-116"/>
    <use x="177.490234" xlink:href="#DejaVuSans-101"/>
    <use x="239.013672" xlink:href="#DejaVuSans-110"/>
    <use x="302.392578" xlink:href="#DejaVuSans-113"/>
    <use x="365.869141" xlink:href="#DejaVuSans-117"/>
    <use x="429.248047" xlink:href="#DejaVuSans-101"/>
    <use x="490.771484" xlink:href="#DejaVuSans-108"/>
    <use x="518.554688" xlink:href="#DejaVuSans-108"/>
    <use x="546.337891" xlink:href="#DejaVuSans-101"/>
    <use x="607.861328" xlink:href="#DejaVuSans-58"/>
    <use x="641.552734" xlink:href="#DejaVuSans-32"/>
    <use x="673.339844" xlink:href="#DejaVuSans-82"/>
    <use x="742.822266" xlink:href="#DejaVuSans-75"/>
    <use x="808.398438" xlink:href="#DejaVuSans-73"/>
    <use x="837.890625" xlink:href="#DejaVuSans-32"/>
    <use x="869.677734" xlink:href="#DejaVuSans-78"/>
    <use x="944.482422" xlink:href="#DejaVuSans-111"/>
    <use x="1005.664062" xlink:href="#DejaVuSans-119"/>
    <use x="1087.451172" xlink:href="#DejaVuSans-99"/>
    <use x="1142.431641" xlink:href="#DejaVuSans-97"/>
    <use x="1203.710938" xlink:href="#DejaVuSans-115"/>
    <use x="1255.810547" xlink:href="#DejaVuSans-116"/>
   </g>
   <!-- Viz: @CorneliusRoemer -->
   <defs>
    <path d="M 28.609375 0 
L 0.78125 72.90625 
L 11.078125 72.90625 
L 34.1875 11.53125 
L 57.328125 72.90625 
L 67.578125 72.90625 
L 39.796875 0 
z
" id="DejaVuSans-86"/>
    <path d="M 37.203125 26.21875 
Q 37.203125 19.234375 40.671875 15.25 
Q 44.140625 11.28125 50.203125 11.28125 
Q 56.203125 11.28125 59.640625 15.28125 
Q 63.09375 19.28125 63.09375 26.21875 
Q 63.09375 33.0625 59.578125 37.078125 
Q 56.0625 41.109375 50.09375 41.109375 
Q 44.1875 41.109375 40.6875 37.109375 
Q 37.203125 33.109375 37.203125 26.21875 
z
M 63.8125 11.625 
Q 60.890625 7.859375 57.109375 6.078125 
Q 53.328125 4.296875 48.296875 4.296875 
Q 39.890625 4.296875 34.640625 10.375 
Q 29.390625 16.453125 29.390625 26.21875 
Q 29.390625 35.984375 34.65625 42.078125 
Q 39.9375 48.1875 48.296875 48.1875 
Q 53.328125 48.1875 57.125 46.359375 
Q 60.9375 44.53125 63.8125 40.828125 
L 63.8125 47.21875 
L 70.796875 47.21875 
L 70.796875 11.28125 
Q 77.9375 12.359375 81.953125 17.796875 
Q 85.984375 23.25 85.984375 31.890625 
Q 85.984375 37.109375 84.4375 41.703125 
Q 82.90625 46.296875 79.78125 50.203125 
Q 74.703125 56.59375 67.40625 59.984375 
Q 60.109375 63.375 51.515625 63.375 
Q 45.515625 63.375 39.984375 61.78125 
Q 34.46875 60.203125 29.78125 57.078125 
Q 22.125 52.09375 17.796875 44.015625 
Q 13.484375 35.9375 13.484375 26.515625 
Q 13.484375 18.75 16.28125 11.953125 
Q 19.09375 5.171875 24.421875 0 
Q 29.546875 -5.078125 36.28125 -7.734375 
Q 43.015625 -10.40625 50.6875 -10.40625 
Q 56.984375 -10.40625 63.0625 -8.28125 
Q 69.140625 -6.15625 74.21875 -2.203125 
L 78.609375 -7.625 
Q 72.515625 -12.359375 65.3125 -14.875 
Q 58.109375 -17.390625 50.6875 -17.390625 
Q 41.65625 -17.390625 33.640625 -14.1875 
Q 25.640625 -10.984375 19.390625 -4.890625 
Q 13.140625 1.21875 9.859375 9.25 
Q 6.59375 17.28125 6.59375 26.515625 
Q 6.59375 35.40625 9.90625 43.453125 
Q 13.234375 51.515625 19.390625 57.625 
Q 25.6875 63.8125 33.9375 67.109375 
Q 42.1875 70.40625 51.421875 70.40625 
Q 61.765625 70.40625 70.625 66.15625 
Q 79.5 61.921875 85.5 54.109375 
Q 89.15625 49.3125 91.078125 43.703125 
Q 93.015625 38.09375 93.015625 32.078125 
Q 93.015625 19.234375 85.25 11.8125 
Q 77.484375 4.390625 63.8125 4.109375 
z
" id="DejaVuSans-64"/>
    <path d="M 64.40625 67.28125 
L 64.40625 56.890625 
Q 59.421875 61.53125 53.78125 63.8125 
Q 48.140625 66.109375 41.796875 66.109375 
Q 29.296875 66.109375 22.65625 58.46875 
Q 16.015625 50.828125 16.015625 36.375 
Q 16.015625 21.96875 22.65625 14.328125 
Q 29.296875 6.6875 41.796875 6.6875 
Q 48.140625 6.6875 53.78125 8.984375 
Q 59.421875 11.28125 64.40625 15.921875 
L 64.40625 5.609375 
Q 59.234375 2.09375 53.4375 0.328125 
Q 47.65625 -1.421875 41.21875 -1.421875 
Q 24.65625 -1.421875 15.125 8.703125 
Q 5.609375 18.84375 5.609375 36.375 
Q 5.609375 53.953125 15.125 64.078125 
Q 24.65625 74.21875 41.21875 74.21875 
Q 47.75 74.21875 53.53125 72.484375 
Q 59.328125 70.75 64.40625 67.28125 
z
" id="DejaVuSans-67"/>
   </defs>
   <g transform="translate(326.960938 232.958281)scale(0.05 -0.05)">
    <use xlink:href="#DejaVuSans-86"/>
    <use x="68.376953" xlink:href="#DejaVuSans-105"/>
    <use x="96.160156" xlink:href="#DejaVuSans-122"/>
    <use x="148.650391" xlink:href="#DejaVuSans-58"/>
    <use x="182.341797" xlink:href="#DejaVuSans-32"/>
    <use x="214.128906" xlink:href="#DejaVuSans-64"/>
    <use x="314.128906" xlink:href="#DejaVuSans-67"/>
    <use x="383.953125" xlink:href="#DejaVuSans-111"/>
    <use x="445.134766" xlink:href="#DejaVuSans-114"/>
    <use x="486.232422" xlink:href="#DejaVuSans-110"/>
    <use x="549.611328" xlink:href="#DejaVuSans-101"/>
    <use x="611.134766" xlink:href="#DejaVuSans-108"/>
    <use x="638.917969" xlink:href="#DejaVuSans-105"/>
    <use x="666.701172" xlink:href="#DejaVuSans-117"/>
    <use x="730.080078" xlink:href="#DejaVuSans-115"/>
    <use x="782.179688" xlink:href="#DejaVuSans-82"/>
    <use x="851.599609" xlink:href="#DejaVuSans-111"/>
    <use x="912.78125" xlink:href="#DejaVuSans-101"/>
    <use x="974.304688" xlink:href="#DejaVuSans-109"/>
    <use x="1071.716797" xlink:href="#DejaVuSans-101"/>
    <use x="1133.240234" xlink:href="#DejaVuSans-114"/>
   </g>
  </g>
 </g>
 <defs>
  <clipPath id="p362f9d746c">
   <rect height="163.8" width="340.2" x="45.478125" y="22.318125"/>
  </clipPath>
 </defs>
</svg>

</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[84]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">start</span><span class="o">=</span><span class="mi">4</span>
<span class="n">locale</span><span class="o">.</span><span class="n">setlocale</span><span class="p">(</span><span class="n">locale</span><span class="o">.</span><span class="n">LC_ALL</span><span class="p">,</span> <span class="s1">&#39;de_DE&#39;</span><span class="p">)</span>
<span class="n">locale</span><span class="o">.</span><span class="n">setlocale</span><span class="p">(</span><span class="n">locale</span><span class="o">.</span><span class="n">LC_NUMERIC</span><span class="p">,</span> <span class="s1">&#39;de_DE&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">rcParams</span><span class="p">[</span><span class="s1">&#39;axes.formatter.use_locale&#39;</span><span class="p">]</span> <span class="o">=</span> <span class="kc">True</span>
<span class="n">fig</span> <span class="o">=</span> <span class="n">plt</span><span class="o">.</span><span class="n">figure</span><span class="p">(</span><span class="n">num</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span> <span class="n">figsize</span><span class="o">=</span><span class="p">(</span><span class="mi">7</span><span class="p">,</span> <span class="mf">3.5</span><span class="p">),</span> <span class="n">facecolor</span><span class="o">=</span><span class="s1">&#39;w&#39;</span><span class="p">,</span> <span class="n">edgecolor</span><span class="o">=</span><span class="s1">&#39;k&#39;</span><span class="p">)</span>
<span class="n">ax</span> <span class="o">=</span> <span class="n">nowcast</span><span class="o">.</span><span class="n">k</span><span class="p">[</span><span class="n">start</span><span class="p">:</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span><span class="o">.</span><span class="n">plot</span><span class="p">(</span><span class="n">zorder</span><span class="o">=</span><span class="mi">1</span><span class="p">)</span>
<span class="n">ax</span><span class="o">.</span><span class="n">fill_between</span><span class="p">(</span><span class="n">nowcast</span><span class="o">.</span><span class="n">index</span><span class="p">[</span><span class="n">start</span><span class="p">:</span><span class="o">-</span><span class="mi">1</span><span class="p">],</span><span class="n">nowcast</span><span class="o">.</span><span class="n">l</span><span class="p">[</span><span class="n">start</span><span class="p">:</span><span class="o">-</span><span class="mi">1</span><span class="p">],</span><span class="n">nowcast</span><span class="o">.</span><span class="n">m</span><span class="p">[</span><span class="n">start</span><span class="p">:</span><span class="o">-</span><span class="mi">1</span><span class="p">],</span><span class="n">color</span><span class="o">=</span><span class="s1">&#39;g&#39;</span><span class="p">,</span><span class="n">alpha</span><span class="o">=</span><span class="mf">0.3</span><span class="p">,</span><span class="n">lw</span><span class="o">=</span><span class="mi">0</span><span class="p">,</span><span class="n">zorder</span><span class="o">=</span><span class="mi">0</span><span class="p">)</span>
<span class="n">ax</span><span class="o">.</span><span class="n">set_xlim</span><span class="p">(</span><span class="n">right</span><span class="o">=</span><span class="n">nowcast</span><span class="o">.</span><span class="n">index</span><span class="p">[</span><span class="o">-</span><span class="mi">2</span><span class="p">]</span><span class="o">+</span><span class="n">pd</span><span class="o">.</span><span class="n">Timedelta</span><span class="p">(</span><span class="n">days</span><span class="o">=</span><span class="mi">1</span><span class="p">))</span>
<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s2">&quot;7-Tage Reproduktionszahl im Zeitverlauf (Deutschland)&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s2">&quot;7-Tage R&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s2">&quot;Datum des Erkrankungsbeginns&quot;</span><span class="p">,</span><span class="n">labelpad</span><span class="o">=</span><span class="mi">0</span><span class="p">)</span>
<span class="n">red_patch</span> <span class="o">=</span> <span class="n">mpatches</span><span class="o">.</span><span class="n">Patch</span><span class="p">(</span><span class="n">color</span><span class="o">=</span><span class="s1">&#39;green&#39;</span><span class="p">,</span> <span class="n">alpha</span><span class="o">=</span><span class="mf">0.3</span><span class="p">,</span> <span class="n">label</span><span class="o">=</span><span class="s1">&#39;95%-Prädiktionsintervall&#39;</span><span class="p">,</span><span class="n">ec</span><span class="o">=</span><span class="kc">None</span><span class="p">)</span>
<span class="n">ax</span><span class="o">.</span><span class="n">legend</span><span class="p">(</span><span class="n">handles</span><span class="o">=</span><span class="p">[</span><span class="n">red_patch</span><span class="p">],</span><span class="n">frameon</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
<span class="n">ax</span><span class="o">.</span><span class="n">axhline</span><span class="p">(</span><span class="mi">1</span><span class="p">,</span><span class="n">c</span><span class="o">=</span><span class="s1">&#39;black&#39;</span><span class="p">,</span><span class="n">ls</span><span class="o">=</span><span class="s1">&#39;:&#39;</span><span class="p">,</span><span class="n">alpha</span><span class="o">=</span><span class="mf">0.3</span><span class="p">)</span>
<span class="c1">#ax.tick_params(axis=&#39;x&#39;, which=&#39;major&#39;, pad=-10)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">grid</span><span class="p">(</span><span class="n">axis</span> <span class="o">=</span> <span class="s1">&#39;y&#39;</span><span class="p">,</span> <span class="n">b</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">which</span><span class="o">=</span><span class="s1">&#39;major&#39;</span><span class="p">,</span> <span class="n">color</span><span class="o">=</span><span class="s1">&#39;#999999&#39;</span><span class="p">,</span> <span class="n">linestyle</span><span class="o">=</span><span class="s1">&#39;-&#39;</span><span class="p">,</span> <span class="n">alpha</span><span class="o">=</span><span class="mf">0.15</span><span class="p">,</span><span class="n">zorder</span><span class="o">=-</span><span class="mi">1</span><span class="p">)</span>
<span class="n">fig</span><span class="o">.</span><span class="n">text</span><span class="p">(</span><span class="mf">0.91</span><span class="p">,</span> <span class="mf">0.04</span><span class="p">,</span> <span class="s2">&quot;Datenstand: &quot;</span> <span class="o">+</span> <span class="n">today</span> <span class="o">+</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">Datenquelle: RKI Nowcast</span><span class="se">\n</span><span class="s2">Viz: @CorneliusRoemer&quot;</span><span class="p">,</span> <span class="n">size</span><span class="o">=</span><span class="mi">6</span><span class="p">,</span> <span class="n">va</span><span class="o">=</span><span class="s2">&quot;bottom&quot;</span><span class="p">,</span> <span class="n">ha</span><span class="o">=</span><span class="s2">&quot;right&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">subplots_adjust</span><span class="p">(</span><span class="n">left</span><span class="o">=</span><span class="mf">0.15</span><span class="p">,</span> <span class="n">right</span><span class="o">=</span><span class="mf">0.9</span><span class="p">,</span> <span class="n">top</span><span class="o">=</span><span class="mf">0.9</span><span class="p">,</span> <span class="n">bottom</span><span class="o">=</span><span class="mf">0.23</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">savefig</span><span class="p">(</span><span class="s1">&#39;7rAll.png&#39;</span><span class="p">,</span><span class="n">dpi</span><span class="o">=</span><span class="mi">400</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt"></div>



<div class="output_svg output_subarea ">
<?xml version="1.0" encoding="utf-8" standalone="no"?>
<!DOCTYPE svg PUBLIC "-//W3C//DTD SVG 1.1//EN"
  "http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd">
<!-- Created with matplotlib (https://matplotlib.org/) -->
<svg height="246.238125pt" version="1.1" viewBox="0 0 434.02125 246.238125" width="434.02125pt" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
 <defs>
  <style type="text/css">
*{stroke-linecap:butt;stroke-linejoin:round;}
  </style>
 </defs>
 <g id="figure_1">
  <g id="patch_1">
   <path d="M 0 246.238125 
L 434.02125 246.238125 
L 434.02125 0 
L 0 0 
z
" style="fill:#ffffff;"/>
  </g>
  <g id="axes_1">
   <g id="patch_2">
    <path d="M 43.78125 191.158125 
L 421.78125 191.158125 
L 421.78125 22.318125 
L 43.78125 22.318125 
z
" style="fill:#ffffff;"/>
   </g>
   <g id="PolyCollection_1">
    <defs>
     <path d="M 43.78125 -164.479893 
L 43.78125 -158.460642 
L 46.40625 -171.702995 
L 49.03125 -193.974225 
L 51.65625 -206.012727 
L 54.28125 -211.430053 
L 56.90625 -206.012727 
L 59.53125 -189.760749 
L 62.15625 -169.295294 
L 64.78125 -150.635615 
L 67.40625 -139.199037 
L 70.03125 -124.150909 
L 72.65625 -113.316257 
L 75.28125 -103.685455 
L 77.90625 -94.054652 
L 80.53125 -88.035401 
L 83.15625 -82.01615 
L 85.78125 -78.404599 
L 88.40625 -75.394973 
L 91.03125 -73.589198 
L 93.65625 -73.589198 
L 96.28125 -72.987273 
L 98.90625 -73.589198 
L 101.53125 -74.191123 
L 104.15625 -74.191123 
L 106.78125 -75.394973 
L 109.40625 -75.394973 
L 112.03125 -75.996898 
L 114.65625 -76.598824 
L 117.28125 -75.996898 
L 119.90625 -75.394973 
L 122.53125 -73.589198 
L 125.15625 -72.987273 
L 127.78125 -71.783422 
L 130.40625 -70.579572 
L 133.03125 -69.375722 
L 135.65625 -68.171872 
L 138.28125 -68.773797 
L 140.90625 -66.968021 
L 143.53125 -66.968021 
L 146.15625 -66.366096 
L 148.78125 -65.162246 
L 151.40625 -66.366096 
L 154.03125 -67.569947 
L 156.65625 -68.171872 
L 159.28125 -69.977647 
L 161.90625 -69.977647 
L 164.53125 -69.375722 
L 167.15625 -69.375722 
L 169.78125 -68.171872 
L 172.40625 -68.171872 
L 175.03125 -68.773797 
L 177.65625 -68.773797 
L 180.28125 -68.773797 
L 182.90625 -68.171872 
L 185.53125 -68.171872 
L 188.15625 -68.171872 
L 190.78125 -68.773797 
L 193.40625 -70.579572 
L 196.03125 -71.181497 
L 198.65625 -72.987273 
L 201.28125 -73.589198 
L 203.90625 -72.385348 
L 206.53125 -72.987273 
L 209.15625 -72.987273 
L 211.78125 -71.783422 
L 214.40625 -71.181497 
L 217.03125 -70.579572 
L 219.65625 -69.977647 
L 222.28125 -69.977647 
L 224.90625 -72.385348 
L 227.53125 -74.191123 
L 230.15625 -74.793048 
L 232.78125 -76.598824 
L 235.40625 -74.191123 
L 238.03125 -74.191123 
L 240.65625 -74.191123 
L 243.28125 -69.977647 
L 245.90625 -69.375722 
L 248.53125 -68.171872 
L 251.15625 -67.569947 
L 253.78125 -71.181497 
L 256.40625 -72.385348 
L 259.03125 -72.987273 
L 261.65625 -75.394973 
L 264.28125 -74.191123 
L 266.90625 -74.191123 
L 269.53125 -71.783422 
L 272.15625 -72.385348 
L 274.78125 -72.385348 
L 277.40625 -73.589198 
L 280.03125 -75.394973 
L 282.65625 -75.394973 
L 285.28125 -76.598824 
L 287.90625 -79.006524 
L 290.53125 -80.210374 
L 293.15625 -80.812299 
L 295.78125 -82.618075 
L 298.40625 -81.414225 
L 301.03125 -82.618075 
L 303.65625 -85.025775 
L 306.28125 -89.841176 
L 308.90625 -104.28738 
L 311.53125 -107.297005 
L 314.15625 -106.69508 
L 316.78125 -104.28738 
L 319.40625 -90.443102 
L 322.03125 -86.831551 
L 324.65625 -81.414225 
L 327.28125 -68.773797 
L 329.90625 -65.162246 
L 332.53125 -62.754545 
L 335.15625 -62.754545 
L 337.78125 -68.773797 
L 340.40625 -70.579572 
L 343.03125 -71.783422 
L 345.65625 -74.793048 
L 348.28125 -75.394973 
L 350.90625 -75.394973 
L 353.53125 -74.191123 
L 356.15625 -72.987273 
L 358.78125 -74.191123 
L 361.40625 -73.589198 
L 364.03125 -73.589198 
L 366.65625 -72.987273 
L 369.28125 -74.191123 
L 371.90625 -77.802674 
L 374.53125 -82.618075 
L 377.15625 -85.627701 
L 379.78125 -89.239251 
L 382.40625 -91.045027 
L 385.03125 -93.452727 
L 387.65625 -93.452727 
L 390.28125 -90.443102 
L 392.90625 -88.035401 
L 395.53125 -85.627701 
L 398.15625 -85.627701 
L 400.78125 -86.229626 
L 403.40625 -87.433476 
L 406.03125 -87.433476 
L 408.65625 -88.637326 
L 411.28125 -87.433476 
L 413.90625 -85.627701 
L 416.53125 -85.627701 
L 419.15625 -84.42385 
L 419.15625 -100.675829 
L 419.15625 -100.675829 
L 416.53125 -99.471979 
L 413.90625 -96.462353 
L 411.28125 -96.462353 
L 408.65625 -96.462353 
L 406.03125 -94.656578 
L 403.40625 -93.452727 
L 400.78125 -91.646952 
L 398.15625 -89.841176 
L 395.53125 -89.841176 
L 392.90625 -91.646952 
L 390.28125 -94.656578 
L 387.65625 -97.666203 
L 385.03125 -97.064278 
L 382.40625 -95.258503 
L 379.78125 -93.452727 
L 377.15625 -89.841176 
L 374.53125 -85.627701 
L 371.90625 -81.414225 
L 369.28125 -77.802674 
L 366.65625 -76.598824 
L 364.03125 -76.598824 
L 361.40625 -76.598824 
L 358.78125 -76.598824 
L 356.15625 -75.996898 
L 353.53125 -77.200749 
L 350.90625 -78.404599 
L 348.28125 -78.404599 
L 345.65625 -77.200749 
L 343.03125 -74.191123 
L 340.40625 -73.589198 
L 337.78125 -71.181497 
L 335.15625 -64.560321 
L 332.53125 -64.560321 
L 329.90625 -66.968021 
L 327.28125 -71.181497 
L 324.65625 -83.821925 
L 322.03125 -89.239251 
L 319.40625 -93.452727 
L 316.78125 -107.89893 
L 314.15625 -110.908556 
L 311.53125 -111.510481 
L 308.90625 -107.89893 
L 306.28125 -93.452727 
L 303.65625 -88.637326 
L 301.03125 -86.229626 
L 298.40625 -85.025775 
L 295.78125 -85.627701 
L 293.15625 -83.821925 
L 290.53125 -83.22 
L 287.90625 -82.01615 
L 285.28125 -79.006524 
L 282.65625 -78.404599 
L 280.03125 -78.404599 
L 277.40625 -76.598824 
L 274.78125 -74.793048 
L 272.15625 -74.793048 
L 269.53125 -74.191123 
L 266.90625 -77.200749 
L 264.28125 -77.200749 
L 261.65625 -77.802674 
L 259.03125 -75.394973 
L 256.40625 -74.793048 
L 253.78125 -72.987273 
L 251.15625 -69.977647 
L 248.53125 -70.579572 
L 245.90625 -71.181497 
L 243.28125 -72.385348 
L 240.65625 -75.996898 
L 238.03125 -76.598824 
L 235.40625 -76.598824 
L 232.78125 -79.006524 
L 230.15625 -77.200749 
L 227.53125 -75.996898 
L 224.90625 -74.191123 
L 222.28125 -71.783422 
L 219.65625 -71.783422 
L 217.03125 -71.783422 
L 214.40625 -72.987273 
L 211.78125 -72.987273 
L 209.15625 -74.191123 
L 206.53125 -74.793048 
L 203.90625 -74.793048 
L 201.28125 -75.394973 
L 198.65625 -74.191123 
L 196.03125 -72.987273 
L 193.40625 -71.783422 
L 190.78125 -69.977647 
L 188.15625 -69.375722 
L 185.53125 -69.375722 
L 182.90625 -69.375722 
L 180.28125 -69.977647 
L 177.65625 -69.977647 
L 175.03125 -69.977647 
L 172.40625 -69.375722 
L 169.78125 -69.375722 
L 167.15625 -70.579572 
L 164.53125 -69.977647 
L 161.90625 -71.181497 
L 159.28125 -71.181497 
L 156.65625 -69.375722 
L 154.03125 -68.773797 
L 151.40625 -67.569947 
L 148.78125 -65.764171 
L 146.15625 -66.968021 
L 143.53125 -67.569947 
L 140.90625 -67.569947 
L 138.28125 -69.375722 
L 135.65625 -68.773797 
L 133.03125 -69.977647 
L 130.40625 -71.181497 
L 127.78125 -72.987273 
L 125.15625 -73.589198 
L 122.53125 -74.191123 
L 119.90625 -75.996898 
L 117.28125 -76.598824 
L 114.65625 -77.200749 
L 112.03125 -76.598824 
L 109.40625 -75.996898 
L 106.78125 -75.996898 
L 104.15625 -74.793048 
L 101.53125 -74.793048 
L 98.90625 -74.191123 
L 96.28125 -73.589198 
L 93.65625 -74.191123 
L 91.03125 -74.191123 
L 88.40625 -75.394973 
L 85.78125 -79.006524 
L 83.15625 -82.618075 
L 80.53125 -88.637326 
L 77.90625 -94.656578 
L 75.28125 -104.28738 
L 72.65625 -114.520107 
L 70.03125 -125.354759 
L 67.40625 -140.402888 
L 64.78125 -152.44139 
L 62.15625 -171.702995 
L 59.53125 -192.770374 
L 56.90625 -210.226203 
L 54.28125 -216.245455 
L 51.65625 -212.031979 
L 49.03125 -199.993476 
L 46.40625 -177.120321 
L 43.78125 -164.479893 
z
" id="m9423680d1a"/>
    </defs>
    <g clip-path="url(#p1a1571f52a)">
     <use style="fill:#008000;fill-opacity:0.3;" x="0" xlink:href="#m9423680d1a" y="246.238125"/>
    </g>
   </g>
   <g id="line2d_1">
    <path clip-path="url(#p1a1571f52a)" d="M 43.78125 85.369783 
L 46.40625 71.525505 
L 49.03125 49.254275 
L 51.65625 37.215772 
L 54.28125 32.400371 
L 56.90625 38.419622 
L 59.53125 55.273526 
L 62.15625 75.738981 
L 64.78125 95.000585 
L 67.40625 106.437162 
L 70.03125 121.485291 
L 72.65625 132.319943 
L 75.28125 142.55267 
L 77.90625 151.581547 
L 80.53125 158.202724 
L 83.15625 163.62005 
L 88.40625 170.843152 
L 91.03125 172.047002 
L 93.65625 172.047002 
L 96.28125 173.250852 
L 98.90625 172.047002 
L 104.15625 172.047002 
L 106.78125 170.843152 
L 109.40625 170.241227 
L 112.03125 170.241227 
L 114.65625 169.037376 
L 117.28125 170.241227 
L 119.90625 170.843152 
L 122.53125 172.648927 
L 125.15625 172.648927 
L 133.03125 176.260478 
L 135.65625 178.066253 
L 138.28125 177.464328 
L 140.90625 178.668178 
L 143.53125 178.668178 
L 146.15625 179.270104 
L 148.78125 180.473954 
L 154.03125 178.066253 
L 156.65625 177.464328 
L 159.28125 175.658553 
L 161.90625 175.658553 
L 164.53125 176.260478 
L 167.15625 176.260478 
L 169.78125 177.464328 
L 172.40625 177.464328 
L 175.03125 176.260478 
L 177.65625 176.862403 
L 180.28125 176.862403 
L 182.90625 177.464328 
L 188.15625 177.464328 
L 190.78125 176.862403 
L 193.40625 175.056628 
L 196.03125 174.454703 
L 198.65625 172.648927 
L 201.28125 171.445077 
L 203.90625 172.648927 
L 206.53125 172.047002 
L 209.15625 172.648927 
L 211.78125 173.852777 
L 214.40625 173.852777 
L 217.03125 175.056628 
L 219.65625 175.056628 
L 222.28125 175.658553 
L 224.90625 172.648927 
L 227.53125 170.843152 
L 230.15625 170.241227 
L 232.78125 168.435451 
L 235.40625 170.843152 
L 238.03125 170.843152 
L 240.65625 171.445077 
L 243.28125 175.056628 
L 245.90625 176.260478 
L 251.15625 177.464328 
L 253.78125 173.852777 
L 256.40625 172.648927 
L 259.03125 172.047002 
L 261.65625 169.639301 
L 266.90625 170.843152 
L 269.53125 173.250852 
L 272.15625 172.648927 
L 274.78125 172.648927 
L 277.40625 171.445077 
L 280.03125 169.037376 
L 282.65625 169.037376 
L 285.28125 168.435451 
L 287.90625 165.425826 
L 290.53125 164.221975 
L 293.15625 163.62005 
L 295.78125 162.4162 
L 298.40625 163.018125 
L 301.03125 161.814275 
L 303.65625 159.406574 
L 306.28125 154.591173 
L 308.90625 140.14497 
L 311.53125 137.135344 
L 314.15625 137.135344 
L 316.78125 140.14497 
L 319.40625 153.989248 
L 322.03125 158.202724 
L 324.65625 163.62005 
L 327.28125 176.260478 
L 329.90625 180.473954 
L 332.53125 182.279729 
L 335.15625 182.881654 
L 337.78125 176.260478 
L 340.40625 174.454703 
L 343.03125 173.250852 
L 345.65625 170.241227 
L 348.28125 169.639301 
L 350.90625 169.639301 
L 353.53125 170.241227 
L 356.15625 172.047002 
L 358.78125 170.843152 
L 361.40625 170.843152 
L 364.03125 171.445077 
L 366.65625 171.445077 
L 369.28125 170.241227 
L 371.90625 166.629676 
L 374.53125 161.814275 
L 379.78125 154.591173 
L 382.40625 153.387323 
L 385.03125 150.979622 
L 387.65625 150.979622 
L 390.28125 153.989248 
L 395.53125 158.804649 
L 398.15625 158.804649 
L 400.78125 156.998874 
L 403.40625 155.795023 
L 406.03125 155.193098 
L 408.65625 153.989248 
L 413.90625 155.193098 
L 416.53125 153.387323 
L 419.15625 153.989248 
L 419.15625 153.989248 
" style="fill:none;stroke:#1f77b4;stroke-linecap:square;stroke-width:1.5;"/>
   </g>
   <g id="matplotlib.axis_1">
    <g id="xtick_1">
     <g id="line2d_2">
      <defs>
       <path d="M 0 0 
L 0 3.5 
" id="m326fd4019b" style="stroke:#000000;stroke-width:0.8;"/>
      </defs>
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="43.78125" xlink:href="#m326fd4019b" y="191.158125"/>
      </g>
     </g>
    </g>
    <g id="xtick_2">
     <g id="line2d_3">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="112.03125" xlink:href="#m326fd4019b" y="191.158125"/>
      </g>
     </g>
     <g id="text_1">
      <!-- Apr -->
      <defs>
       <path d="M 34.1875 63.1875 
L 20.796875 26.90625 
L 47.609375 26.90625 
z
M 28.609375 72.90625 
L 39.796875 72.90625 
L 67.578125 0 
L 57.328125 0 
L 50.6875 18.703125 
L 17.828125 18.703125 
L 11.1875 0 
L 0.78125 0 
z
" id="DejaVuSans-65"/>
       <path d="M 18.109375 8.203125 
L 18.109375 -20.796875 
L 9.078125 -20.796875 
L 9.078125 54.6875 
L 18.109375 54.6875 
L 18.109375 46.390625 
Q 20.953125 51.265625 25.265625 53.625 
Q 29.59375 56 35.59375 56 
Q 45.5625 56 51.78125 48.09375 
Q 58.015625 40.1875 58.015625 27.296875 
Q 58.015625 14.40625 51.78125 6.484375 
Q 45.5625 -1.421875 35.59375 -1.421875 
Q 29.59375 -1.421875 25.265625 0.953125 
Q 20.953125 3.328125 18.109375 8.203125 
z
M 48.6875 27.296875 
Q 48.6875 37.203125 44.609375 42.84375 
Q 40.53125 48.484375 33.40625 48.484375 
Q 26.265625 48.484375 22.1875 42.84375 
Q 18.109375 37.203125 18.109375 27.296875 
Q 18.109375 17.390625 22.1875 11.75 
Q 26.265625 6.109375 33.40625 6.109375 
Q 40.53125 6.109375 44.609375 11.75 
Q 48.6875 17.390625 48.6875 27.296875 
z
" id="DejaVuSans-112"/>
       <path d="M 41.109375 46.296875 
Q 39.59375 47.171875 37.8125 47.578125 
Q 36.03125 48 33.890625 48 
Q 26.265625 48 22.1875 43.046875 
Q 18.109375 38.09375 18.109375 28.8125 
L 18.109375 0 
L 9.078125 0 
L 9.078125 54.6875 
L 18.109375 54.6875 
L 18.109375 46.1875 
Q 20.953125 51.171875 25.484375 53.578125 
Q 30.03125 56 36.53125 56 
Q 37.453125 56 38.578125 55.875 
Q 39.703125 55.765625 41.0625 55.515625 
z
" id="DejaVuSans-114"/>
      </defs>
      <g transform="translate(103.38125 205.756563)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-65"/>
       <use x="68.408203" xlink:href="#DejaVuSans-112"/>
       <use x="131.884766" xlink:href="#DejaVuSans-114"/>
      </g>
      <!-- 2020 -->
      <defs>
       <path d="M 19.1875 8.296875 
L 53.609375 8.296875 
L 53.609375 0 
L 7.328125 0 
L 7.328125 8.296875 
Q 12.9375 14.109375 22.625 23.890625 
Q 32.328125 33.6875 34.8125 36.53125 
Q 39.546875 41.84375 41.421875 45.53125 
Q 43.3125 49.21875 43.3125 52.78125 
Q 43.3125 58.59375 39.234375 62.25 
Q 35.15625 65.921875 28.609375 65.921875 
Q 23.96875 65.921875 18.8125 64.3125 
Q 13.671875 62.703125 7.8125 59.421875 
L 7.8125 69.390625 
Q 13.765625 71.78125 18.9375 73 
Q 24.125 74.21875 28.421875 74.21875 
Q 39.75 74.21875 46.484375 68.546875 
Q 53.21875 62.890625 53.21875 53.421875 
Q 53.21875 48.921875 51.53125 44.890625 
Q 49.859375 40.875 45.40625 35.40625 
Q 44.1875 33.984375 37.640625 27.21875 
Q 31.109375 20.453125 19.1875 8.296875 
z
" id="DejaVuSans-50"/>
       <path d="M 31.78125 66.40625 
Q 24.171875 66.40625 20.328125 58.90625 
Q 16.5 51.421875 16.5 36.375 
Q 16.5 21.390625 20.328125 13.890625 
Q 24.171875 6.390625 31.78125 6.390625 
Q 39.453125 6.390625 43.28125 13.890625 
Q 47.125 21.390625 47.125 36.375 
Q 47.125 51.421875 43.28125 58.90625 
Q 39.453125 66.40625 31.78125 66.40625 
z
M 31.78125 74.21875 
Q 44.046875 74.21875 50.515625 64.515625 
Q 56.984375 54.828125 56.984375 36.375 
Q 56.984375 17.96875 50.515625 8.265625 
Q 44.046875 -1.421875 31.78125 -1.421875 
Q 19.53125 -1.421875 13.0625 8.265625 
Q 6.59375 17.96875 6.59375 36.375 
Q 6.59375 54.828125 13.0625 64.515625 
Q 19.53125 74.21875 31.78125 74.21875 
z
" id="DejaVuSans-48"/>
      </defs>
      <g transform="translate(99.30625 216.954375)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
      </g>
     </g>
    </g>
    <g id="xtick_3">
     <g id="line2d_4">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="190.78125" xlink:href="#m326fd4019b" y="191.158125"/>
      </g>
     </g>
     <g id="text_2">
      <!-- Mai -->
      <defs>
       <path d="M 9.8125 72.90625 
L 24.515625 72.90625 
L 43.109375 23.296875 
L 61.8125 72.90625 
L 76.515625 72.90625 
L 76.515625 0 
L 66.890625 0 
L 66.890625 64.015625 
L 48.09375 14.015625 
L 38.1875 14.015625 
L 19.390625 64.015625 
L 19.390625 0 
L 9.8125 0 
z
" id="DejaVuSans-77"/>
       <path d="M 34.28125 27.484375 
Q 23.390625 27.484375 19.1875 25 
Q 14.984375 22.515625 14.984375 16.5 
Q 14.984375 11.71875 18.140625 8.90625 
Q 21.296875 6.109375 26.703125 6.109375 
Q 34.1875 6.109375 38.703125 11.40625 
Q 43.21875 16.703125 43.21875 25.484375 
L 43.21875 27.484375 
z
M 52.203125 31.203125 
L 52.203125 0 
L 43.21875 0 
L 43.21875 8.296875 
Q 40.140625 3.328125 35.546875 0.953125 
Q 30.953125 -1.421875 24.3125 -1.421875 
Q 15.921875 -1.421875 10.953125 3.296875 
Q 6 8.015625 6 15.921875 
Q 6 25.140625 12.171875 29.828125 
Q 18.359375 34.515625 30.609375 34.515625 
L 43.21875 34.515625 
L 43.21875 35.40625 
Q 43.21875 41.609375 39.140625 45 
Q 35.0625 48.390625 27.6875 48.390625 
Q 23 48.390625 18.546875 47.265625 
Q 14.109375 46.140625 10.015625 43.890625 
L 10.015625 52.203125 
Q 14.9375 54.109375 19.578125 55.046875 
Q 24.21875 56 28.609375 56 
Q 40.484375 56 46.34375 49.84375 
Q 52.203125 43.703125 52.203125 31.203125 
z
" id="DejaVuSans-97"/>
       <path d="M 9.421875 54.6875 
L 18.40625 54.6875 
L 18.40625 0 
L 9.421875 0 
z
M 9.421875 75.984375 
L 18.40625 75.984375 
L 18.40625 64.59375 
L 9.421875 64.59375 
z
" id="DejaVuSans-105"/>
      </defs>
      <g transform="translate(182.014062 205.756563)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-77"/>
       <use x="86.279297" xlink:href="#DejaVuSans-97"/>
       <use x="147.558594" xlink:href="#DejaVuSans-105"/>
      </g>
     </g>
    </g>
    <g id="xtick_4">
     <g id="line2d_5">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="272.15625" xlink:href="#m326fd4019b" y="191.158125"/>
      </g>
     </g>
     <g id="text_3">
      <!-- Jun -->
      <defs>
       <path d="M 9.8125 72.90625 
L 19.671875 72.90625 
L 19.671875 5.078125 
Q 19.671875 -8.109375 14.671875 -14.0625 
Q 9.671875 -20.015625 -1.421875 -20.015625 
L -5.171875 -20.015625 
L -5.171875 -11.71875 
L -2.09375 -11.71875 
Q 4.4375 -11.71875 7.125 -8.046875 
Q 9.8125 -4.390625 9.8125 5.078125 
z
" id="DejaVuSans-74"/>
       <path d="M 8.5 21.578125 
L 8.5 54.6875 
L 17.484375 54.6875 
L 17.484375 21.921875 
Q 17.484375 14.15625 20.5 10.265625 
Q 23.53125 6.390625 29.59375 6.390625 
Q 36.859375 6.390625 41.078125 11.03125 
Q 45.3125 15.671875 45.3125 23.6875 
L 45.3125 54.6875 
L 54.296875 54.6875 
L 54.296875 0 
L 45.3125 0 
L 45.3125 8.40625 
Q 42.046875 3.421875 37.71875 1 
Q 33.40625 -1.421875 27.6875 -1.421875 
Q 18.265625 -1.421875 13.375 4.4375 
Q 8.5 10.296875 8.5 21.578125 
z
M 31.109375 56 
z
" id="DejaVuSans-117"/>
       <path d="M 54.890625 33.015625 
L 54.890625 0 
L 45.90625 0 
L 45.90625 32.71875 
Q 45.90625 40.484375 42.875 44.328125 
Q 39.84375 48.1875 33.796875 48.1875 
Q 26.515625 48.1875 22.3125 43.546875 
Q 18.109375 38.921875 18.109375 30.90625 
L 18.109375 0 
L 9.078125 0 
L 9.078125 54.6875 
L 18.109375 54.6875 
L 18.109375 46.1875 
Q 21.34375 51.125 25.703125 53.5625 
Q 30.078125 56 35.796875 56 
Q 45.21875 56 50.046875 50.171875 
Q 54.890625 44.34375 54.890625 33.015625 
z
" id="DejaVuSans-110"/>
      </defs>
      <g transform="translate(264.34375 205.756563)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-74"/>
       <use x="29.492188" xlink:href="#DejaVuSans-117"/>
       <use x="92.871094" xlink:href="#DejaVuSans-110"/>
      </g>
     </g>
    </g>
    <g id="xtick_5">
     <g id="line2d_6">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="350.90625" xlink:href="#m326fd4019b" y="191.158125"/>
      </g>
     </g>
     <g id="text_4">
      <!-- Jul -->
      <defs>
       <path d="M 9.421875 75.984375 
L 18.40625 75.984375 
L 18.40625 0 
L 9.421875 0 
z
" id="DejaVuSans-108"/>
      </defs>
      <g transform="translate(344.873438 205.756563)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-74"/>
       <use x="29.492188" xlink:href="#DejaVuSans-117"/>
       <use x="92.871094" xlink:href="#DejaVuSans-108"/>
      </g>
     </g>
    </g>
    <g id="xtick_6">
     <g id="line2d_7">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="421.78125" xlink:href="#m326fd4019b" y="191.158125"/>
      </g>
     </g>
    </g>
    <g id="xtick_7">
     <g id="line2d_8">
      <defs>
       <path d="M 0 0 
L 0 2 
" id="m7ec723a5ee" style="stroke:#000000;stroke-width:0.6;"/>
      </defs>
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="51.65625" xlink:href="#m7ec723a5ee" y="191.158125"/>
      </g>
     </g>
    </g>
    <g id="xtick_8">
     <g id="line2d_9">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="70.03125" xlink:href="#m7ec723a5ee" y="191.158125"/>
      </g>
     </g>
    </g>
    <g id="xtick_9">
     <g id="line2d_10">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="88.40625" xlink:href="#m7ec723a5ee" y="191.158125"/>
      </g>
     </g>
    </g>
    <g id="xtick_10">
     <g id="line2d_11">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="106.78125" xlink:href="#m7ec723a5ee" y="191.158125"/>
      </g>
     </g>
    </g>
    <g id="xtick_11">
     <g id="line2d_12">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="125.15625" xlink:href="#m7ec723a5ee" y="191.158125"/>
      </g>
     </g>
    </g>
    <g id="xtick_12">
     <g id="line2d_13">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="143.53125" xlink:href="#m7ec723a5ee" y="191.158125"/>
      </g>
     </g>
    </g>
    <g id="xtick_13">
     <g id="line2d_14">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="161.90625" xlink:href="#m7ec723a5ee" y="191.158125"/>
      </g>
     </g>
    </g>
    <g id="xtick_14">
     <g id="line2d_15">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="180.28125" xlink:href="#m7ec723a5ee" y="191.158125"/>
      </g>
     </g>
    </g>
    <g id="xtick_15">
     <g id="line2d_16">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="198.65625" xlink:href="#m7ec723a5ee" y="191.158125"/>
      </g>
     </g>
    </g>
    <g id="xtick_16">
     <g id="line2d_17">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="217.03125" xlink:href="#m7ec723a5ee" y="191.158125"/>
      </g>
     </g>
    </g>
    <g id="xtick_17">
     <g id="line2d_18">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="235.40625" xlink:href="#m7ec723a5ee" y="191.158125"/>
      </g>
     </g>
    </g>
    <g id="xtick_18">
     <g id="line2d_19">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="253.78125" xlink:href="#m7ec723a5ee" y="191.158125"/>
      </g>
     </g>
    </g>
    <g id="xtick_19">
     <g id="line2d_20">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="290.53125" xlink:href="#m7ec723a5ee" y="191.158125"/>
      </g>
     </g>
    </g>
    <g id="xtick_20">
     <g id="line2d_21">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="308.90625" xlink:href="#m7ec723a5ee" y="191.158125"/>
      </g>
     </g>
    </g>
    <g id="xtick_21">
     <g id="line2d_22">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="327.28125" xlink:href="#m7ec723a5ee" y="191.158125"/>
      </g>
     </g>
    </g>
    <g id="xtick_22">
     <g id="line2d_23">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="345.65625" xlink:href="#m7ec723a5ee" y="191.158125"/>
      </g>
     </g>
    </g>
    <g id="xtick_23">
     <g id="line2d_24">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="364.03125" xlink:href="#m7ec723a5ee" y="191.158125"/>
      </g>
     </g>
    </g>
    <g id="xtick_24">
     <g id="line2d_25">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="382.40625" xlink:href="#m7ec723a5ee" y="191.158125"/>
      </g>
     </g>
    </g>
    <g id="xtick_25">
     <g id="line2d_26">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="400.78125" xlink:href="#m7ec723a5ee" y="191.158125"/>
      </g>
     </g>
    </g>
    <g id="xtick_26">
     <g id="line2d_27">
      <g>
       <use style="stroke:#000000;stroke-width:0.6;" x="419.15625" xlink:href="#m7ec723a5ee" y="191.158125"/>
      </g>
     </g>
    </g>
    <g id="text_5">
     <!-- Datum des Erkrankungsbeginns -->
     <defs>
      <path d="M 19.671875 64.796875 
L 19.671875 8.109375 
L 31.59375 8.109375 
Q 46.6875 8.109375 53.6875 14.9375 
Q 60.6875 21.78125 60.6875 36.53125 
Q 60.6875 51.171875 53.6875 57.984375 
Q 46.6875 64.796875 31.59375 64.796875 
z
M 9.8125 72.90625 
L 30.078125 72.90625 
Q 51.265625 72.90625 61.171875 64.09375 
Q 71.09375 55.28125 71.09375 36.53125 
Q 71.09375 17.671875 61.125 8.828125 
Q 51.171875 0 30.078125 0 
L 9.8125 0 
z
" id="DejaVuSans-68"/>
      <path d="M 18.3125 70.21875 
L 18.3125 54.6875 
L 36.8125 54.6875 
L 36.8125 47.703125 
L 18.3125 47.703125 
L 18.3125 18.015625 
Q 18.3125 11.328125 20.140625 9.421875 
Q 21.96875 7.515625 27.59375 7.515625 
L 36.8125 7.515625 
L 36.8125 0 
L 27.59375 0 
Q 17.1875 0 13.234375 3.875 
Q 9.28125 7.765625 9.28125 18.015625 
L 9.28125 47.703125 
L 2.6875 47.703125 
L 2.6875 54.6875 
L 9.28125 54.6875 
L 9.28125 70.21875 
z
" id="DejaVuSans-116"/>
      <path d="M 52 44.1875 
Q 55.375 50.25 60.0625 53.125 
Q 64.75 56 71.09375 56 
Q 79.640625 56 84.28125 50.015625 
Q 88.921875 44.046875 88.921875 33.015625 
L 88.921875 0 
L 79.890625 0 
L 79.890625 32.71875 
Q 79.890625 40.578125 77.09375 44.375 
Q 74.3125 48.1875 68.609375 48.1875 
Q 61.625 48.1875 57.5625 43.546875 
Q 53.515625 38.921875 53.515625 30.90625 
L 53.515625 0 
L 44.484375 0 
L 44.484375 32.71875 
Q 44.484375 40.625 41.703125 44.40625 
Q 38.921875 48.1875 33.109375 48.1875 
Q 26.21875 48.1875 22.15625 43.53125 
Q 18.109375 38.875 18.109375 30.90625 
L 18.109375 0 
L 9.078125 0 
L 9.078125 54.6875 
L 18.109375 54.6875 
L 18.109375 46.1875 
Q 21.1875 51.21875 25.484375 53.609375 
Q 29.78125 56 35.6875 56 
Q 41.65625 56 45.828125 52.96875 
Q 50 49.953125 52 44.1875 
z
" id="DejaVuSans-109"/>
      <path id="DejaVuSans-32"/>
      <path d="M 45.40625 46.390625 
L 45.40625 75.984375 
L 54.390625 75.984375 
L 54.390625 0 
L 45.40625 0 
L 45.40625 8.203125 
Q 42.578125 3.328125 38.25 0.953125 
Q 33.9375 -1.421875 27.875 -1.421875 
Q 17.96875 -1.421875 11.734375 6.484375 
Q 5.515625 14.40625 5.515625 27.296875 
Q 5.515625 40.1875 11.734375 48.09375 
Q 17.96875 56 27.875 56 
Q 33.9375 56 38.25 53.625 
Q 42.578125 51.265625 45.40625 46.390625 
z
M 14.796875 27.296875 
Q 14.796875 17.390625 18.875 11.75 
Q 22.953125 6.109375 30.078125 6.109375 
Q 37.203125 6.109375 41.296875 11.75 
Q 45.40625 17.390625 45.40625 27.296875 
Q 45.40625 37.203125 41.296875 42.84375 
Q 37.203125 48.484375 30.078125 48.484375 
Q 22.953125 48.484375 18.875 42.84375 
Q 14.796875 37.203125 14.796875 27.296875 
z
" id="DejaVuSans-100"/>
      <path d="M 56.203125 29.59375 
L 56.203125 25.203125 
L 14.890625 25.203125 
Q 15.484375 15.921875 20.484375 11.0625 
Q 25.484375 6.203125 34.421875 6.203125 
Q 39.59375 6.203125 44.453125 7.46875 
Q 49.3125 8.734375 54.109375 11.28125 
L 54.109375 2.78125 
Q 49.265625 0.734375 44.1875 -0.34375 
Q 39.109375 -1.421875 33.890625 -1.421875 
Q 20.796875 -1.421875 13.15625 6.1875 
Q 5.515625 13.8125 5.515625 26.8125 
Q 5.515625 40.234375 12.765625 48.109375 
Q 20.015625 56 32.328125 56 
Q 43.359375 56 49.78125 48.890625 
Q 56.203125 41.796875 56.203125 29.59375 
z
M 47.21875 32.234375 
Q 47.125 39.59375 43.09375 43.984375 
Q 39.0625 48.390625 32.421875 48.390625 
Q 24.90625 48.390625 20.390625 44.140625 
Q 15.875 39.890625 15.1875 32.171875 
z
" id="DejaVuSans-101"/>
      <path d="M 44.28125 53.078125 
L 44.28125 44.578125 
Q 40.484375 46.53125 36.375 47.5 
Q 32.28125 48.484375 27.875 48.484375 
Q 21.1875 48.484375 17.84375 46.4375 
Q 14.5 44.390625 14.5 40.28125 
Q 14.5 37.15625 16.890625 35.375 
Q 19.28125 33.59375 26.515625 31.984375 
L 29.59375 31.296875 
Q 39.15625 29.25 43.1875 25.515625 
Q 47.21875 21.78125 47.21875 15.09375 
Q 47.21875 7.46875 41.1875 3.015625 
Q 35.15625 -1.421875 24.609375 -1.421875 
Q 20.21875 -1.421875 15.453125 -0.5625 
Q 10.6875 0.296875 5.421875 2 
L 5.421875 11.28125 
Q 10.40625 8.6875 15.234375 7.390625 
Q 20.0625 6.109375 24.8125 6.109375 
Q 31.15625 6.109375 34.5625 8.28125 
Q 37.984375 10.453125 37.984375 14.40625 
Q 37.984375 18.0625 35.515625 20.015625 
Q 33.0625 21.96875 24.703125 23.78125 
L 21.578125 24.515625 
Q 13.234375 26.265625 9.515625 29.90625 
Q 5.8125 33.546875 5.8125 39.890625 
Q 5.8125 47.609375 11.28125 51.796875 
Q 16.75 56 26.8125 56 
Q 31.78125 56 36.171875 55.265625 
Q 40.578125 54.546875 44.28125 53.078125 
z
" id="DejaVuSans-115"/>
      <path d="M 9.8125 72.90625 
L 55.90625 72.90625 
L 55.90625 64.59375 
L 19.671875 64.59375 
L 19.671875 43.015625 
L 54.390625 43.015625 
L 54.390625 34.71875 
L 19.671875 34.71875 
L 19.671875 8.296875 
L 56.78125 8.296875 
L 56.78125 0 
L 9.8125 0 
z
" id="DejaVuSans-69"/>
      <path d="M 9.078125 75.984375 
L 18.109375 75.984375 
L 18.109375 31.109375 
L 44.921875 54.6875 
L 56.390625 54.6875 
L 27.390625 29.109375 
L 57.625 0 
L 45.90625 0 
L 18.109375 26.703125 
L 18.109375 0 
L 9.078125 0 
z
" id="DejaVuSans-107"/>
      <path d="M 45.40625 27.984375 
Q 45.40625 37.75 41.375 43.109375 
Q 37.359375 48.484375 30.078125 48.484375 
Q 22.859375 48.484375 18.828125 43.109375 
Q 14.796875 37.75 14.796875 27.984375 
Q 14.796875 18.265625 18.828125 12.890625 
Q 22.859375 7.515625 30.078125 7.515625 
Q 37.359375 7.515625 41.375 12.890625 
Q 45.40625 18.265625 45.40625 27.984375 
z
M 54.390625 6.78125 
Q 54.390625 -7.171875 48.1875 -13.984375 
Q 42 -20.796875 29.203125 -20.796875 
Q 24.46875 -20.796875 20.265625 -20.09375 
Q 16.0625 -19.390625 12.109375 -17.921875 
L 12.109375 -9.1875 
Q 16.0625 -11.328125 19.921875 -12.34375 
Q 23.78125 -13.375 27.78125 -13.375 
Q 36.625 -13.375 41.015625 -8.765625 
Q 45.40625 -4.15625 45.40625 5.171875 
L 45.40625 9.625 
Q 42.625 4.78125 38.28125 2.390625 
Q 33.9375 0 27.875 0 
Q 17.828125 0 11.671875 7.65625 
Q 5.515625 15.328125 5.515625 27.984375 
Q 5.515625 40.671875 11.671875 48.328125 
Q 17.828125 56 27.875 56 
Q 33.9375 56 38.28125 53.609375 
Q 42.625 51.21875 45.40625 46.390625 
L 45.40625 54.6875 
L 54.390625 54.6875 
z
" id="DejaVuSans-103"/>
      <path d="M 48.6875 27.296875 
Q 48.6875 37.203125 44.609375 42.84375 
Q 40.53125 48.484375 33.40625 48.484375 
Q 26.265625 48.484375 22.1875 42.84375 
Q 18.109375 37.203125 18.109375 27.296875 
Q 18.109375 17.390625 22.1875 11.75 
Q 26.265625 6.109375 33.40625 6.109375 
Q 40.53125 6.109375 44.609375 11.75 
Q 48.6875 17.390625 48.6875 27.296875 
z
M 18.109375 46.390625 
Q 20.953125 51.265625 25.265625 53.625 
Q 29.59375 56 35.59375 56 
Q 45.5625 56 51.78125 48.09375 
Q 58.015625 40.1875 58.015625 27.296875 
Q 58.015625 14.40625 51.78125 6.484375 
Q 45.5625 -1.421875 35.59375 -1.421875 
Q 29.59375 -1.421875 25.265625 0.953125 
Q 20.953125 3.328125 18.109375 8.203125 
L 18.109375 0 
L 9.078125 0 
L 9.078125 75.984375 
L 18.109375 75.984375 
z
" id="DejaVuSans-98"/>
     </defs>
     <g transform="translate(152.670313 226.6325)scale(0.1 -0.1)">
      <use xlink:href="#DejaVuSans-68"/>
      <use x="77.001953" xlink:href="#DejaVuSans-97"/>
      <use x="138.28125" xlink:href="#DejaVuSans-116"/>
      <use x="177.490234" xlink:href="#DejaVuSans-117"/>
      <use x="240.869141" xlink:href="#DejaVuSans-109"/>
      <use x="338.28125" xlink:href="#DejaVuSans-32"/>
      <use x="370.068359" xlink:href="#DejaVuSans-100"/>
      <use x="433.544922" xlink:href="#DejaVuSans-101"/>
      <use x="495.068359" xlink:href="#DejaVuSans-115"/>
      <use x="547.167969" xlink:href="#DejaVuSans-32"/>
      <use x="578.955078" xlink:href="#DejaVuSans-69"/>
      <use x="642.138672" xlink:href="#DejaVuSans-114"/>
      <use x="683.251953" xlink:href="#DejaVuSans-107"/>
      <use x="741.162109" xlink:href="#DejaVuSans-114"/>
      <use x="782.275391" xlink:href="#DejaVuSans-97"/>
      <use x="843.554688" xlink:href="#DejaVuSans-110"/>
      <use x="906.933594" xlink:href="#DejaVuSans-107"/>
      <use x="964.796875" xlink:href="#DejaVuSans-117"/>
      <use x="1028.175781" xlink:href="#DejaVuSans-110"/>
      <use x="1091.554688" xlink:href="#DejaVuSans-103"/>
      <use x="1155.03125" xlink:href="#DejaVuSans-115"/>
      <use x="1207.130859" xlink:href="#DejaVuSans-98"/>
      <use x="1270.607422" xlink:href="#DejaVuSans-101"/>
      <use x="1332.130859" xlink:href="#DejaVuSans-103"/>
      <use x="1395.607422" xlink:href="#DejaVuSans-105"/>
      <use x="1423.390625" xlink:href="#DejaVuSans-110"/>
      <use x="1486.769531" xlink:href="#DejaVuSans-110"/>
      <use x="1550.148438" xlink:href="#DejaVuSans-115"/>
     </g>
    </g>
   </g>
   <g id="matplotlib.axis_2">
    <g id="ytick_1">
     <g id="line2d_28">
      <path clip-path="url(#p1a1571f52a)" d="M 43.78125 166.027751 
L 421.78125 166.027751 
" style="fill:none;stroke:#999999;stroke-linecap:square;stroke-opacity:0.15;stroke-width:0.8;"/>
     </g>
     <g id="line2d_29">
      <defs>
       <path d="M 0 0 
L -3.5 0 
" id="m4d9ca8d2b7" style="stroke:#000000;stroke-width:0.8;"/>
      </defs>
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="43.78125" xlink:href="#m4d9ca8d2b7" y="166.027751"/>
      </g>
     </g>
     <g id="text_6">
      <!-- 1,0 -->
      <defs>
       <path d="M 12.40625 8.296875 
L 28.515625 8.296875 
L 28.515625 63.921875 
L 10.984375 60.40625 
L 10.984375 69.390625 
L 28.421875 72.90625 
L 38.28125 72.90625 
L 38.28125 8.296875 
L 54.390625 8.296875 
L 54.390625 0 
L 12.40625 0 
z
" id="DejaVuSans-49"/>
       <path d="M 11.71875 12.40625 
L 22.015625 12.40625 
L 22.015625 4 
L 14.015625 -11.625 
L 7.71875 -11.625 
L 11.71875 4 
z
" id="DejaVuSans-44"/>
      </defs>
      <g transform="translate(20.878125 169.826969)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-49"/>
       <use x="63.623047" xlink:href="#DejaVuSans-44"/>
       <use x="95.410156" xlink:href="#DejaVuSans-48"/>
      </g>
     </g>
    </g>
    <g id="ytick_2">
     <g id="line2d_30">
      <path clip-path="url(#p1a1571f52a)" d="M 43.78125 135.931494 
L 421.78125 135.931494 
" style="fill:none;stroke:#999999;stroke-linecap:square;stroke-opacity:0.15;stroke-width:0.8;"/>
     </g>
     <g id="line2d_31">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="43.78125" xlink:href="#m4d9ca8d2b7" y="135.931494"/>
      </g>
     </g>
     <g id="text_7">
      <!-- 1,5 -->
      <defs>
       <path d="M 10.796875 72.90625 
L 49.515625 72.90625 
L 49.515625 64.59375 
L 19.828125 64.59375 
L 19.828125 46.734375 
Q 21.96875 47.46875 24.109375 47.828125 
Q 26.265625 48.1875 28.421875 48.1875 
Q 40.625 48.1875 47.75 41.5 
Q 54.890625 34.8125 54.890625 23.390625 
Q 54.890625 11.625 47.5625 5.09375 
Q 40.234375 -1.421875 26.90625 -1.421875 
Q 22.3125 -1.421875 17.546875 -0.640625 
Q 12.796875 0.140625 7.71875 1.703125 
L 7.71875 11.625 
Q 12.109375 9.234375 16.796875 8.0625 
Q 21.484375 6.890625 26.703125 6.890625 
Q 35.15625 6.890625 40.078125 11.328125 
Q 45.015625 15.765625 45.015625 23.390625 
Q 45.015625 31 40.078125 35.4375 
Q 35.15625 39.890625 26.703125 39.890625 
Q 22.75 39.890625 18.8125 39.015625 
Q 14.890625 38.140625 10.796875 36.28125 
z
" id="DejaVuSans-53"/>
      </defs>
      <g transform="translate(20.878125 139.730713)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-49"/>
       <use x="63.623047" xlink:href="#DejaVuSans-44"/>
       <use x="95.410156" xlink:href="#DejaVuSans-53"/>
      </g>
     </g>
    </g>
    <g id="ytick_3">
     <g id="line2d_32">
      <path clip-path="url(#p1a1571f52a)" d="M 43.78125 105.835237 
L 421.78125 105.835237 
" style="fill:none;stroke:#999999;stroke-linecap:square;stroke-opacity:0.15;stroke-width:0.8;"/>
     </g>
     <g id="line2d_33">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="43.78125" xlink:href="#m4d9ca8d2b7" y="105.835237"/>
      </g>
     </g>
     <g id="text_8">
      <!-- 2,0 -->
      <g transform="translate(20.878125 109.634456)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-44"/>
       <use x="95.410156" xlink:href="#DejaVuSans-48"/>
      </g>
     </g>
    </g>
    <g id="ytick_4">
     <g id="line2d_34">
      <path clip-path="url(#p1a1571f52a)" d="M 43.78125 75.738981 
L 421.78125 75.738981 
" style="fill:none;stroke:#999999;stroke-linecap:square;stroke-opacity:0.15;stroke-width:0.8;"/>
     </g>
     <g id="line2d_35">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="43.78125" xlink:href="#m4d9ca8d2b7" y="75.738981"/>
      </g>
     </g>
     <g id="text_9">
      <!-- 2,5 -->
      <g transform="translate(20.878125 79.538199)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-44"/>
       <use x="95.410156" xlink:href="#DejaVuSans-53"/>
      </g>
     </g>
    </g>
    <g id="ytick_5">
     <g id="line2d_36">
      <path clip-path="url(#p1a1571f52a)" d="M 43.78125 45.642724 
L 421.78125 45.642724 
" style="fill:none;stroke:#999999;stroke-linecap:square;stroke-opacity:0.15;stroke-width:0.8;"/>
     </g>
     <g id="line2d_37">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="43.78125" xlink:href="#m4d9ca8d2b7" y="45.642724"/>
      </g>
     </g>
     <g id="text_10">
      <!-- 3,0 -->
      <defs>
       <path d="M 40.578125 39.3125 
Q 47.65625 37.796875 51.625 33 
Q 55.609375 28.21875 55.609375 21.1875 
Q 55.609375 10.40625 48.1875 4.484375 
Q 40.765625 -1.421875 27.09375 -1.421875 
Q 22.515625 -1.421875 17.65625 -0.515625 
Q 12.796875 0.390625 7.625 2.203125 
L 7.625 11.71875 
Q 11.71875 9.328125 16.59375 8.109375 
Q 21.484375 6.890625 26.8125 6.890625 
Q 36.078125 6.890625 40.9375 10.546875 
Q 45.796875 14.203125 45.796875 21.1875 
Q 45.796875 27.640625 41.28125 31.265625 
Q 36.765625 34.90625 28.71875 34.90625 
L 20.21875 34.90625 
L 20.21875 43.015625 
L 29.109375 43.015625 
Q 36.375 43.015625 40.234375 45.921875 
Q 44.09375 48.828125 44.09375 54.296875 
Q 44.09375 59.90625 40.109375 62.90625 
Q 36.140625 65.921875 28.71875 65.921875 
Q 24.65625 65.921875 20.015625 65.03125 
Q 15.375 64.15625 9.8125 62.3125 
L 9.8125 71.09375 
Q 15.4375 72.65625 20.34375 73.4375 
Q 25.25 74.21875 29.59375 74.21875 
Q 40.828125 74.21875 47.359375 69.109375 
Q 53.90625 64.015625 53.90625 55.328125 
Q 53.90625 49.265625 50.4375 45.09375 
Q 46.96875 40.921875 40.578125 39.3125 
z
" id="DejaVuSans-51"/>
      </defs>
      <g transform="translate(20.878125 49.441943)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-51"/>
       <use x="63.623047" xlink:href="#DejaVuSans-44"/>
       <use x="95.410156" xlink:href="#DejaVuSans-48"/>
      </g>
     </g>
    </g>
    <g id="text_11">
     <!-- 7-Tage R -->
     <defs>
      <path d="M 8.203125 72.90625 
L 55.078125 72.90625 
L 55.078125 68.703125 
L 28.609375 0 
L 18.3125 0 
L 43.21875 64.59375 
L 8.203125 64.59375 
z
" id="DejaVuSans-55"/>
      <path d="M 4.890625 31.390625 
L 31.203125 31.390625 
L 31.203125 23.390625 
L 4.890625 23.390625 
z
" id="DejaVuSans-45"/>
      <path d="M -0.296875 72.90625 
L 61.375 72.90625 
L 61.375 64.59375 
L 35.5 64.59375 
L 35.5 0 
L 25.59375 0 
L 25.59375 64.59375 
L -0.296875 64.59375 
z
" id="DejaVuSans-84"/>
      <path d="M 44.390625 34.1875 
Q 47.5625 33.109375 50.5625 29.59375 
Q 53.5625 26.078125 56.59375 19.921875 
L 66.609375 0 
L 56 0 
L 46.6875 18.703125 
Q 43.0625 26.03125 39.671875 28.421875 
Q 36.28125 30.8125 30.421875 30.8125 
L 19.671875 30.8125 
L 19.671875 0 
L 9.8125 0 
L 9.8125 72.90625 
L 32.078125 72.90625 
Q 44.578125 72.90625 50.734375 67.671875 
Q 56.890625 62.453125 56.890625 51.90625 
Q 56.890625 45.015625 53.6875 40.46875 
Q 50.484375 35.9375 44.390625 34.1875 
z
M 19.671875 64.796875 
L 19.671875 38.921875 
L 32.078125 38.921875 
Q 39.203125 38.921875 42.84375 42.21875 
Q 46.484375 45.515625 46.484375 51.90625 
Q 46.484375 58.296875 42.84375 61.546875 
Q 39.203125 64.796875 32.078125 64.796875 
z
" id="DejaVuSans-82"/>
     </defs>
     <g transform="translate(14.798437 129.135781)rotate(-90)scale(0.1 -0.1)">
      <use xlink:href="#DejaVuSans-55"/>
      <use x="63.623047" xlink:href="#DejaVuSans-45"/>
      <use x="99.566406" xlink:href="#DejaVuSans-84"/>
      <use x="160.400391" xlink:href="#DejaVuSans-97"/>
      <use x="221.679688" xlink:href="#DejaVuSans-103"/>
      <use x="285.15625" xlink:href="#DejaVuSans-101"/>
      <use x="346.679688" xlink:href="#DejaVuSans-32"/>
      <use x="378.466797" xlink:href="#DejaVuSans-82"/>
     </g>
    </g>
   </g>
   <g id="line2d_38">
    <path clip-path="url(#p1a1571f52a)" d="M 43.78125 166.027751 
L 421.78125 166.027751 
" style="fill:none;stroke:#000000;stroke-dasharray:1.5,2.475;stroke-dashoffset:0;stroke-opacity:0.3;stroke-width:1.5;"/>
   </g>
   <g id="patch_3">
    <path d="M 43.78125 191.158125 
L 43.78125 22.318125 
" style="fill:none;stroke:#000000;stroke-linecap:square;stroke-linejoin:miter;stroke-width:0.8;"/>
   </g>
   <g id="patch_4">
    <path d="M 421.78125 191.158125 
L 421.78125 22.318125 
" style="fill:none;stroke:#000000;stroke-linecap:square;stroke-linejoin:miter;stroke-width:0.8;"/>
   </g>
   <g id="patch_5">
    <path d="M 43.78125 191.158125 
L 421.78125 191.158125 
" style="fill:none;stroke:#000000;stroke-linecap:square;stroke-linejoin:miter;stroke-width:0.8;"/>
   </g>
   <g id="patch_6">
    <path d="M 43.78125 22.318125 
L 421.78125 22.318125 
" style="fill:none;stroke:#000000;stroke-linecap:square;stroke-linejoin:miter;stroke-width:0.8;"/>
   </g>
   <g id="text_12">
    <!-- 7-Tage Reproduktionszahl im Zeitverlauf (Deutschland) -->
    <defs>
     <path d="M 30.609375 48.390625 
Q 23.390625 48.390625 19.1875 42.75 
Q 14.984375 37.109375 14.984375 27.296875 
Q 14.984375 17.484375 19.15625 11.84375 
Q 23.34375 6.203125 30.609375 6.203125 
Q 37.796875 6.203125 41.984375 11.859375 
Q 46.1875 17.53125 46.1875 27.296875 
Q 46.1875 37.015625 41.984375 42.703125 
Q 37.796875 48.390625 30.609375 48.390625 
z
M 30.609375 56 
Q 42.328125 56 49.015625 48.375 
Q 55.71875 40.765625 55.71875 27.296875 
Q 55.71875 13.875 49.015625 6.21875 
Q 42.328125 -1.421875 30.609375 -1.421875 
Q 18.84375 -1.421875 12.171875 6.21875 
Q 5.515625 13.875 5.515625 27.296875 
Q 5.515625 40.765625 12.171875 48.375 
Q 18.84375 56 30.609375 56 
z
" id="DejaVuSans-111"/>
     <path d="M 5.515625 54.6875 
L 48.1875 54.6875 
L 48.1875 46.484375 
L 14.40625 7.171875 
L 48.1875 7.171875 
L 48.1875 0 
L 4.296875 0 
L 4.296875 8.203125 
L 38.09375 47.515625 
L 5.515625 47.515625 
z
" id="DejaVuSans-122"/>
     <path d="M 54.890625 33.015625 
L 54.890625 0 
L 45.90625 0 
L 45.90625 32.71875 
Q 45.90625 40.484375 42.875 44.328125 
Q 39.84375 48.1875 33.796875 48.1875 
Q 26.515625 48.1875 22.3125 43.546875 
Q 18.109375 38.921875 18.109375 30.90625 
L 18.109375 0 
L 9.078125 0 
L 9.078125 75.984375 
L 18.109375 75.984375 
L 18.109375 46.1875 
Q 21.34375 51.125 25.703125 53.5625 
Q 30.078125 56 35.796875 56 
Q 45.21875 56 50.046875 50.171875 
Q 54.890625 44.34375 54.890625 33.015625 
z
" id="DejaVuSans-104"/>
     <path d="M 5.609375 72.90625 
L 62.890625 72.90625 
L 62.890625 65.375 
L 16.796875 8.296875 
L 64.015625 8.296875 
L 64.015625 0 
L 4.5 0 
L 4.5 7.515625 
L 50.59375 64.59375 
L 5.609375 64.59375 
z
" id="DejaVuSans-90"/>
     <path d="M 2.984375 54.6875 
L 12.5 54.6875 
L 29.59375 8.796875 
L 46.6875 54.6875 
L 56.203125 54.6875 
L 35.6875 0 
L 23.484375 0 
z
" id="DejaVuSans-118"/>
     <path d="M 37.109375 75.984375 
L 37.109375 68.5 
L 28.515625 68.5 
Q 23.6875 68.5 21.796875 66.546875 
Q 19.921875 64.59375 19.921875 59.515625 
L 19.921875 54.6875 
L 34.71875 54.6875 
L 34.71875 47.703125 
L 19.921875 47.703125 
L 19.921875 0 
L 10.890625 0 
L 10.890625 47.703125 
L 2.296875 47.703125 
L 2.296875 54.6875 
L 10.890625 54.6875 
L 10.890625 58.5 
Q 10.890625 67.625 15.140625 71.796875 
Q 19.390625 75.984375 28.609375 75.984375 
z
" id="DejaVuSans-102"/>
     <path d="M 31 75.875 
Q 24.46875 64.65625 21.28125 53.65625 
Q 18.109375 42.671875 18.109375 31.390625 
Q 18.109375 20.125 21.3125 9.0625 
Q 24.515625 -2 31 -13.1875 
L 23.1875 -13.1875 
Q 15.875 -1.703125 12.234375 9.375 
Q 8.59375 20.453125 8.59375 31.390625 
Q 8.59375 42.28125 12.203125 53.3125 
Q 15.828125 64.359375 23.1875 75.875 
z
" id="DejaVuSans-40"/>
     <path d="M 48.78125 52.59375 
L 48.78125 44.1875 
Q 44.96875 46.296875 41.140625 47.34375 
Q 37.3125 48.390625 33.40625 48.390625 
Q 24.65625 48.390625 19.8125 42.84375 
Q 14.984375 37.3125 14.984375 27.296875 
Q 14.984375 17.28125 19.8125 11.734375 
Q 24.65625 6.203125 33.40625 6.203125 
Q 37.3125 6.203125 41.140625 7.25 
Q 44.96875 8.296875 48.78125 10.40625 
L 48.78125 2.09375 
Q 45.015625 0.34375 40.984375 -0.53125 
Q 36.96875 -1.421875 32.421875 -1.421875 
Q 20.0625 -1.421875 12.78125 6.34375 
Q 5.515625 14.109375 5.515625 27.296875 
Q 5.515625 40.671875 12.859375 48.328125 
Q 20.21875 56 33.015625 56 
Q 37.15625 56 41.109375 55.140625 
Q 45.0625 54.296875 48.78125 52.59375 
z
" id="DejaVuSans-99"/>
     <path d="M 8.015625 75.875 
L 15.828125 75.875 
Q 23.140625 64.359375 26.78125 53.3125 
Q 30.421875 42.28125 30.421875 31.390625 
Q 30.421875 20.453125 26.78125 9.375 
Q 23.140625 -1.703125 15.828125 -13.1875 
L 8.015625 -13.1875 
Q 14.5 -2 17.703125 9.0625 
Q 20.90625 20.125 20.90625 31.390625 
Q 20.90625 42.671875 17.703125 53.65625 
Q 14.5 64.65625 8.015625 75.875 
z
" id="DejaVuSans-41"/>
    </defs>
    <g transform="translate(65.919375 16.318125)scale(0.12 -0.12)">
     <use xlink:href="#DejaVuSans-55"/>
     <use x="63.623047" xlink:href="#DejaVuSans-45"/>
     <use x="99.566406" xlink:href="#DejaVuSans-84"/>
     <use x="160.400391" xlink:href="#DejaVuSans-97"/>
     <use x="221.679688" xlink:href="#DejaVuSans-103"/>
     <use x="285.15625" xlink:href="#DejaVuSans-101"/>
     <use x="346.679688" xlink:href="#DejaVuSans-32"/>
     <use x="378.466797" xlink:href="#DejaVuSans-82"/>
     <use x="447.886719" xlink:href="#DejaVuSans-101"/>
     <use x="509.410156" xlink:href="#DejaVuSans-112"/>
     <use x="572.886719" xlink:href="#DejaVuSans-114"/>
     <use x="613.96875" xlink:href="#DejaVuSans-111"/>
     <use x="675.150391" xlink:href="#DejaVuSans-100"/>
     <use x="738.626953" xlink:href="#DejaVuSans-117"/>
     <use x="802.005859" xlink:href="#DejaVuSans-107"/>
     <use x="859.916016" xlink:href="#DejaVuSans-116"/>
     <use x="899.125" xlink:href="#DejaVuSans-105"/>
     <use x="926.908203" xlink:href="#DejaVuSans-111"/>
     <use x="988.089844" xlink:href="#DejaVuSans-110"/>
     <use x="1051.46875" xlink:href="#DejaVuSans-115"/>
     <use x="1103.568359" xlink:href="#DejaVuSans-122"/>
     <use x="1156.058594" xlink:href="#DejaVuSans-97"/>
     <use x="1217.337891" xlink:href="#DejaVuSans-104"/>
     <use x="1280.716797" xlink:href="#DejaVuSans-108"/>
     <use x="1308.5" xlink:href="#DejaVuSans-32"/>
     <use x="1340.287109" xlink:href="#DejaVuSans-105"/>
     <use x="1368.070312" xlink:href="#DejaVuSans-109"/>
     <use x="1465.482422" xlink:href="#DejaVuSans-32"/>
     <use x="1497.269531" xlink:href="#DejaVuSans-90"/>
     <use x="1565.775391" xlink:href="#DejaVuSans-101"/>
     <use x="1627.298828" xlink:href="#DejaVuSans-105"/>
     <use x="1655.082031" xlink:href="#DejaVuSans-116"/>
     <use x="1694.291016" xlink:href="#DejaVuSans-118"/>
     <use x="1753.470703" xlink:href="#DejaVuSans-101"/>
     <use x="1814.994141" xlink:href="#DejaVuSans-114"/>
     <use x="1856.107422" xlink:href="#DejaVuSans-108"/>
     <use x="1883.890625" xlink:href="#DejaVuSans-97"/>
     <use x="1945.169922" xlink:href="#DejaVuSans-117"/>
     <use x="2008.548828" xlink:href="#DejaVuSans-102"/>
     <use x="2043.753906" xlink:href="#DejaVuSans-32"/>
     <use x="2075.541016" xlink:href="#DejaVuSans-40"/>
     <use x="2114.554688" xlink:href="#DejaVuSans-68"/>
     <use x="2191.556641" xlink:href="#DejaVuSans-101"/>
     <use x="2253.080078" xlink:href="#DejaVuSans-117"/>
     <use x="2316.458984" xlink:href="#DejaVuSans-116"/>
     <use x="2355.667969" xlink:href="#DejaVuSans-115"/>
     <use x="2407.767578" xlink:href="#DejaVuSans-99"/>
     <use x="2462.748047" xlink:href="#DejaVuSans-104"/>
     <use x="2526.126953" xlink:href="#DejaVuSans-108"/>
     <use x="2553.910156" xlink:href="#DejaVuSans-97"/>
     <use x="2615.189453" xlink:href="#DejaVuSans-110"/>
     <use x="2678.568359" xlink:href="#DejaVuSans-100"/>
     <use x="2742.044922" xlink:href="#DejaVuSans-41"/>
    </g>
   </g>
   <g id="legend_1">
    <g id="patch_7">
     <path d="M 262.495313 38.916562 
L 282.495313 38.916562 
L 282.495313 31.916562 
L 262.495313 31.916562 
z
" style="fill:#008000;opacity:0.3;"/>
    </g>
    <g id="text_13">
     <!-- 95%-Prädiktionsintervall -->
     <defs>
      <path d="M 10.984375 1.515625 
L 10.984375 10.5 
Q 14.703125 8.734375 18.5 7.8125 
Q 22.3125 6.890625 25.984375 6.890625 
Q 35.75 6.890625 40.890625 13.453125 
Q 46.046875 20.015625 46.78125 33.40625 
Q 43.953125 29.203125 39.59375 26.953125 
Q 35.25 24.703125 29.984375 24.703125 
Q 19.046875 24.703125 12.671875 31.3125 
Q 6.296875 37.9375 6.296875 49.421875 
Q 6.296875 60.640625 12.9375 67.421875 
Q 19.578125 74.21875 30.609375 74.21875 
Q 43.265625 74.21875 49.921875 64.515625 
Q 56.59375 54.828125 56.59375 36.375 
Q 56.59375 19.140625 48.40625 8.859375 
Q 40.234375 -1.421875 26.421875 -1.421875 
Q 22.703125 -1.421875 18.890625 -0.6875 
Q 15.09375 0.046875 10.984375 1.515625 
z
M 30.609375 32.421875 
Q 37.25 32.421875 41.125 36.953125 
Q 45.015625 41.5 45.015625 49.421875 
Q 45.015625 57.28125 41.125 61.84375 
Q 37.25 66.40625 30.609375 66.40625 
Q 23.96875 66.40625 20.09375 61.84375 
Q 16.21875 57.28125 16.21875 49.421875 
Q 16.21875 41.5 20.09375 36.953125 
Q 23.96875 32.421875 30.609375 32.421875 
z
" id="DejaVuSans-57"/>
      <path d="M 72.703125 32.078125 
Q 68.453125 32.078125 66.03125 28.46875 
Q 63.625 24.859375 63.625 18.40625 
Q 63.625 12.0625 66.03125 8.421875 
Q 68.453125 4.78125 72.703125 4.78125 
Q 76.859375 4.78125 79.265625 8.421875 
Q 81.6875 12.0625 81.6875 18.40625 
Q 81.6875 24.8125 79.265625 28.4375 
Q 76.859375 32.078125 72.703125 32.078125 
z
M 72.703125 38.28125 
Q 80.421875 38.28125 84.953125 32.90625 
Q 89.5 27.546875 89.5 18.40625 
Q 89.5 9.28125 84.9375 3.921875 
Q 80.375 -1.421875 72.703125 -1.421875 
Q 64.890625 -1.421875 60.34375 3.921875 
Q 55.8125 9.28125 55.8125 18.40625 
Q 55.8125 27.59375 60.375 32.9375 
Q 64.9375 38.28125 72.703125 38.28125 
z
M 22.3125 68.015625 
Q 18.109375 68.015625 15.6875 64.375 
Q 13.28125 60.75 13.28125 54.390625 
Q 13.28125 47.953125 15.671875 44.328125 
Q 18.0625 40.71875 22.3125 40.71875 
Q 26.5625 40.71875 28.96875 44.328125 
Q 31.390625 47.953125 31.390625 54.390625 
Q 31.390625 60.6875 28.953125 64.34375 
Q 26.515625 68.015625 22.3125 68.015625 
z
M 66.40625 74.21875 
L 74.21875 74.21875 
L 28.609375 -1.421875 
L 20.796875 -1.421875 
z
M 22.3125 74.21875 
Q 30.03125 74.21875 34.609375 68.875 
Q 39.203125 63.53125 39.203125 54.390625 
Q 39.203125 45.171875 34.640625 39.84375 
Q 30.078125 34.515625 22.3125 34.515625 
Q 14.546875 34.515625 10.03125 39.859375 
Q 5.515625 45.21875 5.515625 54.390625 
Q 5.515625 63.484375 10.046875 68.84375 
Q 14.59375 74.21875 22.3125 74.21875 
z
" id="DejaVuSans-37"/>
      <path d="M 19.671875 64.796875 
L 19.671875 37.40625 
L 32.078125 37.40625 
Q 38.96875 37.40625 42.71875 40.96875 
Q 46.484375 44.53125 46.484375 51.125 
Q 46.484375 57.671875 42.71875 61.234375 
Q 38.96875 64.796875 32.078125 64.796875 
z
M 9.8125 72.90625 
L 32.078125 72.90625 
Q 44.34375 72.90625 50.609375 67.359375 
Q 56.890625 61.8125 56.890625 51.125 
Q 56.890625 40.328125 50.609375 34.8125 
Q 44.34375 29.296875 32.078125 29.296875 
L 19.671875 29.296875 
L 19.671875 0 
L 9.8125 0 
z
" id="DejaVuSans-80"/>
      <path d="M 34.28125 27.484375 
Q 23.390625 27.484375 19.1875 25 
Q 14.984375 22.515625 14.984375 16.5 
Q 14.984375 11.71875 18.140625 8.90625 
Q 21.296875 6.109375 26.703125 6.109375 
Q 34.1875 6.109375 38.703125 11.40625 
Q 43.21875 16.703125 43.21875 25.484375 
L 43.21875 27.484375 
z
M 52.203125 31.203125 
L 52.203125 0 
L 43.21875 0 
L 43.21875 8.296875 
Q 40.140625 3.328125 35.546875 0.953125 
Q 30.953125 -1.421875 24.3125 -1.421875 
Q 15.921875 -1.421875 10.953125 3.296875 
Q 6 8.015625 6 15.921875 
Q 6 25.140625 12.171875 29.828125 
Q 18.359375 34.515625 30.609375 34.515625 
L 43.21875 34.515625 
L 43.21875 35.40625 
Q 43.21875 41.609375 39.140625 45 
Q 35.0625 48.390625 27.6875 48.390625 
Q 23 48.390625 18.546875 47.265625 
Q 14.109375 46.140625 10.015625 43.890625 
L 10.015625 52.203125 
Q 14.9375 54.109375 19.578125 55.046875 
Q 24.21875 56 28.609375 56 
Q 40.484375 56 46.34375 49.84375 
Q 52.203125 43.703125 52.203125 31.203125 
z
M 33.59375 75.78125 
L 43.5 75.78125 
L 43.5 65.921875 
L 33.59375 65.921875 
z
M 14.5 75.78125 
L 24.421875 75.78125 
L 24.421875 65.921875 
L 14.5 65.921875 
z
" id="DejaVuSans-228"/>
     </defs>
     <g transform="translate(290.495313 38.916562)scale(0.1 -0.1)">
      <use xlink:href="#DejaVuSans-57"/>
      <use x="63.623047" xlink:href="#DejaVuSans-53"/>
      <use x="127.246094" xlink:href="#DejaVuSans-37"/>
      <use x="222.265625" xlink:href="#DejaVuSans-45"/>
      <use x="258.349609" xlink:href="#DejaVuSans-80"/>
      <use x="318.636719" xlink:href="#DejaVuSans-114"/>
      <use x="359.75" xlink:href="#DejaVuSans-228"/>
      <use x="421.029297" xlink:href="#DejaVuSans-100"/>
      <use x="484.505859" xlink:href="#DejaVuSans-105"/>
      <use x="512.289062" xlink:href="#DejaVuSans-107"/>
      <use x="570.199219" xlink:href="#DejaVuSans-116"/>
      <use x="609.408203" xlink:href="#DejaVuSans-105"/>
      <use x="637.191406" xlink:href="#DejaVuSans-111"/>
      <use x="698.373047" xlink:href="#DejaVuSans-110"/>
      <use x="761.751953" xlink:href="#DejaVuSans-115"/>
      <use x="813.851562" xlink:href="#DejaVuSans-105"/>
      <use x="841.634766" xlink:href="#DejaVuSans-110"/>
      <use x="905.013672" xlink:href="#DejaVuSans-116"/>
      <use x="944.222656" xlink:href="#DejaVuSans-101"/>
      <use x="1005.746094" xlink:href="#DejaVuSans-114"/>
      <use x="1046.859375" xlink:href="#DejaVuSans-118"/>
      <use x="1106.039062" xlink:href="#DejaVuSans-97"/>
      <use x="1167.318359" xlink:href="#DejaVuSans-108"/>
      <use x="1195.101562" xlink:href="#DejaVuSans-108"/>
     </g>
    </g>
   </g>
  </g>
  <g id="text_14">
   <!-- Datenstand: 1. August 2020 -->
   <defs>
    <path d="M 11.71875 12.40625 
L 22.015625 12.40625 
L 22.015625 0 
L 11.71875 0 
z
M 11.71875 51.703125 
L 22.015625 51.703125 
L 22.015625 39.3125 
L 11.71875 39.3125 
z
" id="DejaVuSans-58"/>
    <path d="M 10.6875 12.40625 
L 21 12.40625 
L 21 0 
L 10.6875 0 
z
" id="DejaVuSans-46"/>
   </defs>
   <g transform="translate(342.179063 224.352937)scale(0.06 -0.06)">
    <use xlink:href="#DejaVuSans-68"/>
    <use x="77.001953" xlink:href="#DejaVuSans-97"/>
    <use x="138.28125" xlink:href="#DejaVuSans-116"/>
    <use x="177.490234" xlink:href="#DejaVuSans-101"/>
    <use x="239.013672" xlink:href="#DejaVuSans-110"/>
    <use x="302.392578" xlink:href="#DejaVuSans-115"/>
    <use x="354.492188" xlink:href="#DejaVuSans-116"/>
    <use x="393.701172" xlink:href="#DejaVuSans-97"/>
    <use x="454.980469" xlink:href="#DejaVuSans-110"/>
    <use x="518.359375" xlink:href="#DejaVuSans-100"/>
    <use x="581.835938" xlink:href="#DejaVuSans-58"/>
    <use x="615.527344" xlink:href="#DejaVuSans-32"/>
    <use x="647.314453" xlink:href="#DejaVuSans-49"/>
    <use x="710.9375" xlink:href="#DejaVuSans-46"/>
    <use x="742.724609" xlink:href="#DejaVuSans-32"/>
    <use x="774.511719" xlink:href="#DejaVuSans-65"/>
    <use x="842.919922" xlink:href="#DejaVuSans-117"/>
    <use x="906.298828" xlink:href="#DejaVuSans-103"/>
    <use x="969.775391" xlink:href="#DejaVuSans-117"/>
    <use x="1033.154297" xlink:href="#DejaVuSans-115"/>
    <use x="1085.253906" xlink:href="#DejaVuSans-116"/>
    <use x="1124.462891" xlink:href="#DejaVuSans-32"/>
    <use x="1156.25" xlink:href="#DejaVuSans-50"/>
    <use x="1219.873047" xlink:href="#DejaVuSans-48"/>
    <use x="1283.496094" xlink:href="#DejaVuSans-50"/>
    <use x="1347.119141" xlink:href="#DejaVuSans-48"/>
   </g>
   <!-- Datenquelle: RKI Nowcast -->
   <defs>
    <path d="M 14.796875 27.296875 
Q 14.796875 17.390625 18.875 11.75 
Q 22.953125 6.109375 30.078125 6.109375 
Q 37.203125 6.109375 41.296875 11.75 
Q 45.40625 17.390625 45.40625 27.296875 
Q 45.40625 37.203125 41.296875 42.84375 
Q 37.203125 48.484375 30.078125 48.484375 
Q 22.953125 48.484375 18.875 42.84375 
Q 14.796875 37.203125 14.796875 27.296875 
z
M 45.40625 8.203125 
Q 42.578125 3.328125 38.25 0.953125 
Q 33.9375 -1.421875 27.875 -1.421875 
Q 17.96875 -1.421875 11.734375 6.484375 
Q 5.515625 14.40625 5.515625 27.296875 
Q 5.515625 40.1875 11.734375 48.09375 
Q 17.96875 56 27.875 56 
Q 33.9375 56 38.25 53.625 
Q 42.578125 51.265625 45.40625 46.390625 
L 45.40625 54.6875 
L 54.390625 54.6875 
L 54.390625 -20.796875 
L 45.40625 -20.796875 
z
" id="DejaVuSans-113"/>
    <path d="M 9.8125 72.90625 
L 19.671875 72.90625 
L 19.671875 42.09375 
L 52.390625 72.90625 
L 65.09375 72.90625 
L 28.90625 38.921875 
L 67.671875 0 
L 54.6875 0 
L 19.671875 35.109375 
L 19.671875 0 
L 9.8125 0 
z
" id="DejaVuSans-75"/>
    <path d="M 9.8125 72.90625 
L 19.671875 72.90625 
L 19.671875 0 
L 9.8125 0 
z
" id="DejaVuSans-73"/>
    <path d="M 9.8125 72.90625 
L 23.09375 72.90625 
L 55.421875 11.921875 
L 55.421875 72.90625 
L 64.984375 72.90625 
L 64.984375 0 
L 51.703125 0 
L 19.390625 60.984375 
L 19.390625 0 
L 9.8125 0 
z
" id="DejaVuSans-78"/>
    <path d="M 4.203125 54.6875 
L 13.1875 54.6875 
L 24.421875 12.015625 
L 35.59375 54.6875 
L 46.1875 54.6875 
L 57.421875 12.015625 
L 68.609375 54.6875 
L 77.59375 54.6875 
L 63.28125 0 
L 52.6875 0 
L 40.921875 44.828125 
L 29.109375 0 
L 18.5 0 
z
" id="DejaVuSans-119"/>
   </defs>
   <g transform="translate(349.119375 231.071625)scale(0.06 -0.06)">
    <use xlink:href="#DejaVuSans-68"/>
    <use x="77.001953" xlink:href="#DejaVuSans-97"/>
    <use x="138.28125" xlink:href="#DejaVuSans-116"/>
    <use x="177.490234" xlink:href="#DejaVuSans-101"/>
    <use x="239.013672" xlink:href="#DejaVuSans-110"/>
    <use x="302.392578" xlink:href="#DejaVuSans-113"/>
    <use x="365.869141" xlink:href="#DejaVuSans-117"/>
    <use x="429.248047" xlink:href="#DejaVuSans-101"/>
    <use x="490.771484" xlink:href="#DejaVuSans-108"/>
    <use x="518.554688" xlink:href="#DejaVuSans-108"/>
    <use x="546.337891" xlink:href="#DejaVuSans-101"/>
    <use x="607.861328" xlink:href="#DejaVuSans-58"/>
    <use x="641.552734" xlink:href="#DejaVuSans-32"/>
    <use x="673.339844" xlink:href="#DejaVuSans-82"/>
    <use x="742.822266" xlink:href="#DejaVuSans-75"/>
    <use x="808.398438" xlink:href="#DejaVuSans-73"/>
    <use x="837.890625" xlink:href="#DejaVuSans-32"/>
    <use x="869.677734" xlink:href="#DejaVuSans-78"/>
    <use x="944.482422" xlink:href="#DejaVuSans-111"/>
    <use x="1005.664062" xlink:href="#DejaVuSans-119"/>
    <use x="1087.451172" xlink:href="#DejaVuSans-99"/>
    <use x="1142.431641" xlink:href="#DejaVuSans-97"/>
    <use x="1203.710938" xlink:href="#DejaVuSans-115"/>
    <use x="1255.810547" xlink:href="#DejaVuSans-116"/>
   </g>
   <!-- Viz: @CorneliusRoemer -->
   <defs>
    <path d="M 28.609375 0 
L 0.78125 72.90625 
L 11.078125 72.90625 
L 34.1875 11.53125 
L 57.328125 72.90625 
L 67.578125 72.90625 
L 39.796875 0 
z
" id="DejaVuSans-86"/>
    <path d="M 37.203125 26.21875 
Q 37.203125 19.234375 40.671875 15.25 
Q 44.140625 11.28125 50.203125 11.28125 
Q 56.203125 11.28125 59.640625 15.28125 
Q 63.09375 19.28125 63.09375 26.21875 
Q 63.09375 33.0625 59.578125 37.078125 
Q 56.0625 41.109375 50.09375 41.109375 
Q 44.1875 41.109375 40.6875 37.109375 
Q 37.203125 33.109375 37.203125 26.21875 
z
M 63.8125 11.625 
Q 60.890625 7.859375 57.109375 6.078125 
Q 53.328125 4.296875 48.296875 4.296875 
Q 39.890625 4.296875 34.640625 10.375 
Q 29.390625 16.453125 29.390625 26.21875 
Q 29.390625 35.984375 34.65625 42.078125 
Q 39.9375 48.1875 48.296875 48.1875 
Q 53.328125 48.1875 57.125 46.359375 
Q 60.9375 44.53125 63.8125 40.828125 
L 63.8125 47.21875 
L 70.796875 47.21875 
L 70.796875 11.28125 
Q 77.9375 12.359375 81.953125 17.796875 
Q 85.984375 23.25 85.984375 31.890625 
Q 85.984375 37.109375 84.4375 41.703125 
Q 82.90625 46.296875 79.78125 50.203125 
Q 74.703125 56.59375 67.40625 59.984375 
Q 60.109375 63.375 51.515625 63.375 
Q 45.515625 63.375 39.984375 61.78125 
Q 34.46875 60.203125 29.78125 57.078125 
Q 22.125 52.09375 17.796875 44.015625 
Q 13.484375 35.9375 13.484375 26.515625 
Q 13.484375 18.75 16.28125 11.953125 
Q 19.09375 5.171875 24.421875 0 
Q 29.546875 -5.078125 36.28125 -7.734375 
Q 43.015625 -10.40625 50.6875 -10.40625 
Q 56.984375 -10.40625 63.0625 -8.28125 
Q 69.140625 -6.15625 74.21875 -2.203125 
L 78.609375 -7.625 
Q 72.515625 -12.359375 65.3125 -14.875 
Q 58.109375 -17.390625 50.6875 -17.390625 
Q 41.65625 -17.390625 33.640625 -14.1875 
Q 25.640625 -10.984375 19.390625 -4.890625 
Q 13.140625 1.21875 9.859375 9.25 
Q 6.59375 17.28125 6.59375 26.515625 
Q 6.59375 35.40625 9.90625 43.453125 
Q 13.234375 51.515625 19.390625 57.625 
Q 25.6875 63.8125 33.9375 67.109375 
Q 42.1875 70.40625 51.421875 70.40625 
Q 61.765625 70.40625 70.625 66.15625 
Q 79.5 61.921875 85.5 54.109375 
Q 89.15625 49.3125 91.078125 43.703125 
Q 93.015625 38.09375 93.015625 32.078125 
Q 93.015625 19.234375 85.25 11.8125 
Q 77.484375 4.390625 63.8125 4.109375 
z
" id="DejaVuSans-64"/>
    <path d="M 64.40625 67.28125 
L 64.40625 56.890625 
Q 59.421875 61.53125 53.78125 63.8125 
Q 48.140625 66.109375 41.796875 66.109375 
Q 29.296875 66.109375 22.65625 58.46875 
Q 16.015625 50.828125 16.015625 36.375 
Q 16.015625 21.96875 22.65625 14.328125 
Q 29.296875 6.6875 41.796875 6.6875 
Q 48.140625 6.6875 53.78125 8.984375 
Q 59.421875 11.28125 64.40625 15.921875 
L 64.40625 5.609375 
Q 59.234375 2.09375 53.4375 0.328125 
Q 47.65625 -1.421875 41.21875 -1.421875 
Q 24.65625 -1.421875 15.125 8.703125 
Q 5.609375 18.84375 5.609375 36.375 
Q 5.609375 53.953125 15.125 64.078125 
Q 24.65625 74.21875 41.21875 74.21875 
Q 47.75 74.21875 53.53125 72.484375 
Q 59.328125 70.75 64.40625 67.28125 
z
" id="DejaVuSans-67"/>
   </defs>
   <g transform="translate(356.360625 237.790312)scale(0.06 -0.06)">
    <use xlink:href="#DejaVuSans-86"/>
    <use x="68.376953" xlink:href="#DejaVuSans-105"/>
    <use x="96.160156" xlink:href="#DejaVuSans-122"/>
    <use x="148.650391" xlink:href="#DejaVuSans-58"/>
    <use x="182.341797" xlink:href="#DejaVuSans-32"/>
    <use x="214.128906" xlink:href="#DejaVuSans-64"/>
    <use x="314.128906" xlink:href="#DejaVuSans-67"/>
    <use x="383.953125" xlink:href="#DejaVuSans-111"/>
    <use x="445.134766" xlink:href="#DejaVuSans-114"/>
    <use x="486.232422" xlink:href="#DejaVuSans-110"/>
    <use x="549.611328" xlink:href="#DejaVuSans-101"/>
    <use x="611.134766" xlink:href="#DejaVuSans-108"/>
    <use x="638.917969" xlink:href="#DejaVuSans-105"/>
    <use x="666.701172" xlink:href="#DejaVuSans-117"/>
    <use x="730.080078" xlink:href="#DejaVuSans-115"/>
    <use x="782.179688" xlink:href="#DejaVuSans-82"/>
    <use x="851.599609" xlink:href="#DejaVuSans-111"/>
    <use x="912.78125" xlink:href="#DejaVuSans-101"/>
    <use x="974.304688" xlink:href="#DejaVuSans-109"/>
    <use x="1071.716797" xlink:href="#DejaVuSans-101"/>
    <use x="1133.240234" xlink:href="#DejaVuSans-114"/>
   </g>
  </g>
 </g>
 <defs>
  <clipPath id="p1a1571f52a">
   <rect height="168.84" width="378" x="43.78125" y="22.318125"/>
  </clipPath>
 </defs>
</svg>

</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[85]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="kn">import</span> <span class="nn">statsmodels.api</span> <span class="k">as</span> <span class="nn">sm</span>
<span class="kn">import</span> <span class="nn">numpy</span> <span class="k">as</span> <span class="nn">np</span>
<span class="n">nowcast</span><span class="o">.</span><span class="n">index</span><span class="o">.</span><span class="n">freq</span> <span class="o">=</span> <span class="s1">&#39;D&#39;</span>
<span class="n">nowcast</span><span class="p">[</span><span class="s1">&#39;log_b&#39;</span><span class="p">]</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">log10</span><span class="p">(</span><span class="n">nowcast</span><span class="p">[</span><span class="s1">&#39;b&#39;</span><span class="p">])</span>
<span class="n">train</span><span class="p">,</span><span class="n">test</span> <span class="o">=</span> <span class="n">nowcast</span><span class="p">[</span><span class="s1">&#39;log_b&#39;</span><span class="p">][</span><span class="mi">10</span><span class="p">:],</span> <span class="n">nowcast</span><span class="p">[</span><span class="s1">&#39;log_b&#39;</span><span class="p">][</span><span class="o">-</span><span class="mi">1</span><span class="p">:]</span>
<span class="n">model</span> <span class="o">=</span> <span class="n">sm</span><span class="o">.</span><span class="n">tsa</span><span class="o">.</span><span class="n">statespace</span><span class="o">.</span><span class="n">ExponentialSmoothing</span><span class="p">(</span><span class="n">train</span><span class="p">,</span> <span class="n">trend</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span><span class="n">seasonal</span><span class="o">=</span><span class="mi">7</span><span class="p">)</span><span class="o">.</span><span class="n">fit</span><span class="p">()</span>
<span class="n">pred</span> <span class="o">=</span> <span class="n">model</span><span class="o">.</span><span class="n">predict</span><span class="p">(</span><span class="n">start</span><span class="o">=</span><span class="n">test</span><span class="o">.</span><span class="n">index</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">+</span><span class="mi">1</span><span class="p">,</span> <span class="n">end</span><span class="o">=</span><span class="n">test</span><span class="o">.</span><span class="n">index</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span><span class="o">+</span><span class="mi">30</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">plot</span><span class="p">(</span><span class="n">train</span><span class="o">.</span><span class="n">index</span><span class="p">,</span> <span class="n">train</span><span class="p">,</span> <span class="n">label</span><span class="o">=</span><span class="s1">&#39;Train&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">plot</span><span class="p">(</span><span class="n">test</span><span class="o">.</span><span class="n">index</span><span class="p">,</span> <span class="n">test</span><span class="p">,</span> <span class="n">label</span><span class="o">=</span><span class="s1">&#39;Test&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">plot</span><span class="p">(</span><span class="n">pred</span><span class="o">.</span><span class="n">index</span><span class="p">,</span> <span class="n">pred</span><span class="p">,</span> <span class="n">label</span><span class="o">=</span><span class="s1">&#39;Holt-Winters&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">legend</span><span class="p">(</span><span class="n">loc</span><span class="o">=</span><span class="s1">&#39;best&#39;</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt"></div>


<div class="output_subarea output_stream output_stderr output_text">
<pre>/Users/cornelius/opt/anaconda3/lib/python3.7/site-packages/statsmodels/base/model.py:568: ConvergenceWarning: Maximum Likelihood optimization failed to converge. Check mle_retvals
  &#34;Check mle_retvals&#34;, ConvergenceWarning)
</pre>
</div>
</div>

<div class="output_area">

    <div class="prompt output_prompt">Out[85]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>&lt;matplotlib.legend.Legend at 0x7ff1afd8be50&gt;</pre>
</div>

</div>

<div class="output_area">

    <div class="prompt"></div>



<div class="output_svg output_subarea ">
<?xml version="1.0" encoding="utf-8" standalone="no"?>
<!DOCTYPE svg PUBLIC "-//W3C//DTD SVG 1.1//EN"
  "http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd">
<!-- Created with matplotlib (https://matplotlib.org/) -->
<svg height="248.518125pt" version="1.1" viewBox="0 0 386.834791 248.518125" width="386.834791pt" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
 <defs>
  <style type="text/css">
*{stroke-linecap:butt;stroke-linejoin:round;}
  </style>
 </defs>
 <g id="figure_1">
  <g id="patch_1">
   <path d="M 0 248.518125 
L 386.834791 248.518125 
L 386.834791 0 
L 0 0 
z
" style="fill:none;"/>
  </g>
  <g id="axes_1">
   <g id="patch_2">
    <path d="M 30.103125 224.64 
L 364.903125 224.64 
L 364.903125 7.2 
L 30.103125 7.2 
z
" style="fill:#ffffff;"/>
   </g>
   <g id="matplotlib.axis_1">
    <g id="xtick_1">
     <g id="line2d_1">
      <defs>
       <path d="M 0 0 
L 0 3.5 
" id="m657296cf5c" style="stroke:#000000;stroke-width:0.8;"/>
      </defs>
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="81.555073" xlink:href="#m657296cf5c" y="224.64"/>
      </g>
     </g>
     <g id="text_1">
      <!-- 2020-04 -->
      <defs>
       <path d="M 19.1875 8.296875 
L 53.609375 8.296875 
L 53.609375 0 
L 7.328125 0 
L 7.328125 8.296875 
Q 12.9375 14.109375 22.625 23.890625 
Q 32.328125 33.6875 34.8125 36.53125 
Q 39.546875 41.84375 41.421875 45.53125 
Q 43.3125 49.21875 43.3125 52.78125 
Q 43.3125 58.59375 39.234375 62.25 
Q 35.15625 65.921875 28.609375 65.921875 
Q 23.96875 65.921875 18.8125 64.3125 
Q 13.671875 62.703125 7.8125 59.421875 
L 7.8125 69.390625 
Q 13.765625 71.78125 18.9375 73 
Q 24.125 74.21875 28.421875 74.21875 
Q 39.75 74.21875 46.484375 68.546875 
Q 53.21875 62.890625 53.21875 53.421875 
Q 53.21875 48.921875 51.53125 44.890625 
Q 49.859375 40.875 45.40625 35.40625 
Q 44.1875 33.984375 37.640625 27.21875 
Q 31.109375 20.453125 19.1875 8.296875 
z
" id="DejaVuSans-50"/>
       <path d="M 31.78125 66.40625 
Q 24.171875 66.40625 20.328125 58.90625 
Q 16.5 51.421875 16.5 36.375 
Q 16.5 21.390625 20.328125 13.890625 
Q 24.171875 6.390625 31.78125 6.390625 
Q 39.453125 6.390625 43.28125 13.890625 
Q 47.125 21.390625 47.125 36.375 
Q 47.125 51.421875 43.28125 58.90625 
Q 39.453125 66.40625 31.78125 66.40625 
z
M 31.78125 74.21875 
Q 44.046875 74.21875 50.515625 64.515625 
Q 56.984375 54.828125 56.984375 36.375 
Q 56.984375 17.96875 50.515625 8.265625 
Q 44.046875 -1.421875 31.78125 -1.421875 
Q 19.53125 -1.421875 13.0625 8.265625 
Q 6.59375 17.96875 6.59375 36.375 
Q 6.59375 54.828125 13.0625 64.515625 
Q 19.53125 74.21875 31.78125 74.21875 
z
" id="DejaVuSans-48"/>
       <path d="M 4.890625 31.390625 
L 31.203125 31.390625 
L 31.203125 23.390625 
L 4.890625 23.390625 
z
" id="DejaVuSans-45"/>
       <path d="M 37.796875 64.3125 
L 12.890625 25.390625 
L 37.796875 25.390625 
z
M 35.203125 72.90625 
L 47.609375 72.90625 
L 47.609375 25.390625 
L 58.015625 25.390625 
L 58.015625 17.1875 
L 47.609375 17.1875 
L 47.609375 0 
L 37.796875 0 
L 37.796875 17.1875 
L 4.890625 17.1875 
L 4.890625 26.703125 
z
" id="DejaVuSans-52"/>
      </defs>
      <g transform="translate(60.663667 239.238438)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-52"/>
      </g>
     </g>
    </g>
    <g id="xtick_2">
     <g id="line2d_2">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="135.905722" xlink:href="#m657296cf5c" y="224.64"/>
      </g>
     </g>
     <g id="text_2">
      <!-- 2020-05 -->
      <defs>
       <path d="M 10.796875 72.90625 
L 49.515625 72.90625 
L 49.515625 64.59375 
L 19.828125 64.59375 
L 19.828125 46.734375 
Q 21.96875 47.46875 24.109375 47.828125 
Q 26.265625 48.1875 28.421875 48.1875 
Q 40.625 48.1875 47.75 41.5 
Q 54.890625 34.8125 54.890625 23.390625 
Q 54.890625 11.625 47.5625 5.09375 
Q 40.234375 -1.421875 26.90625 -1.421875 
Q 22.3125 -1.421875 17.546875 -0.640625 
Q 12.796875 0.140625 7.71875 1.703125 
L 7.71875 11.625 
Q 12.109375 9.234375 16.796875 8.0625 
Q 21.484375 6.890625 26.703125 6.890625 
Q 35.15625 6.890625 40.078125 11.328125 
Q 45.015625 15.765625 45.015625 23.390625 
Q 45.015625 31 40.078125 35.4375 
Q 35.15625 39.890625 26.703125 39.890625 
Q 22.75 39.890625 18.8125 39.015625 
Q 14.890625 38.140625 10.796875 36.28125 
z
" id="DejaVuSans-53"/>
      </defs>
      <g transform="translate(115.014316 239.238438)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-53"/>
      </g>
     </g>
    </g>
    <g id="xtick_3">
     <g id="line2d_3">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="192.06806" xlink:href="#m657296cf5c" y="224.64"/>
      </g>
     </g>
     <g id="text_3">
      <!-- 2020-06 -->
      <defs>
       <path d="M 33.015625 40.375 
Q 26.375 40.375 22.484375 35.828125 
Q 18.609375 31.296875 18.609375 23.390625 
Q 18.609375 15.53125 22.484375 10.953125 
Q 26.375 6.390625 33.015625 6.390625 
Q 39.65625 6.390625 43.53125 10.953125 
Q 47.40625 15.53125 47.40625 23.390625 
Q 47.40625 31.296875 43.53125 35.828125 
Q 39.65625 40.375 33.015625 40.375 
z
M 52.59375 71.296875 
L 52.59375 62.3125 
Q 48.875 64.0625 45.09375 64.984375 
Q 41.3125 65.921875 37.59375 65.921875 
Q 27.828125 65.921875 22.671875 59.328125 
Q 17.53125 52.734375 16.796875 39.40625 
Q 19.671875 43.65625 24.015625 45.921875 
Q 28.375 48.1875 33.59375 48.1875 
Q 44.578125 48.1875 50.953125 41.515625 
Q 57.328125 34.859375 57.328125 23.390625 
Q 57.328125 12.15625 50.6875 5.359375 
Q 44.046875 -1.421875 33.015625 -1.421875 
Q 20.359375 -1.421875 13.671875 8.265625 
Q 6.984375 17.96875 6.984375 36.375 
Q 6.984375 53.65625 15.1875 63.9375 
Q 23.390625 74.21875 37.203125 74.21875 
Q 40.921875 74.21875 44.703125 73.484375 
Q 48.484375 72.75 52.59375 71.296875 
z
" id="DejaVuSans-54"/>
      </defs>
      <g transform="translate(171.176654 239.238438)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-54"/>
      </g>
     </g>
    </g>
    <g id="xtick_4">
     <g id="line2d_4">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="246.418709" xlink:href="#m657296cf5c" y="224.64"/>
      </g>
     </g>
     <g id="text_4">
      <!-- 2020-07 -->
      <defs>
       <path d="M 8.203125 72.90625 
L 55.078125 72.90625 
L 55.078125 68.703125 
L 28.609375 0 
L 18.3125 0 
L 43.21875 64.59375 
L 8.203125 64.59375 
z
" id="DejaVuSans-55"/>
      </defs>
      <g transform="translate(225.527303 239.238438)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-55"/>
      </g>
     </g>
    </g>
    <g id="xtick_5">
     <g id="line2d_5">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="302.581047" xlink:href="#m657296cf5c" y="224.64"/>
      </g>
     </g>
     <g id="text_5">
      <!-- 2020-08 -->
      <defs>
       <path d="M 31.78125 34.625 
Q 24.75 34.625 20.71875 30.859375 
Q 16.703125 27.09375 16.703125 20.515625 
Q 16.703125 13.921875 20.71875 10.15625 
Q 24.75 6.390625 31.78125 6.390625 
Q 38.8125 6.390625 42.859375 10.171875 
Q 46.921875 13.96875 46.921875 20.515625 
Q 46.921875 27.09375 42.890625 30.859375 
Q 38.875 34.625 31.78125 34.625 
z
M 21.921875 38.8125 
Q 15.578125 40.375 12.03125 44.71875 
Q 8.5 49.078125 8.5 55.328125 
Q 8.5 64.0625 14.71875 69.140625 
Q 20.953125 74.21875 31.78125 74.21875 
Q 42.671875 74.21875 48.875 69.140625 
Q 55.078125 64.0625 55.078125 55.328125 
Q 55.078125 49.078125 51.53125 44.71875 
Q 48 40.375 41.703125 38.8125 
Q 48.828125 37.15625 52.796875 32.3125 
Q 56.78125 27.484375 56.78125 20.515625 
Q 56.78125 9.90625 50.3125 4.234375 
Q 43.84375 -1.421875 31.78125 -1.421875 
Q 19.734375 -1.421875 13.25 4.234375 
Q 6.78125 9.90625 6.78125 20.515625 
Q 6.78125 27.484375 10.78125 32.3125 
Q 14.796875 37.15625 21.921875 38.8125 
z
M 18.3125 54.390625 
Q 18.3125 48.734375 21.84375 45.5625 
Q 25.390625 42.390625 31.78125 42.390625 
Q 38.140625 42.390625 41.71875 45.5625 
Q 45.3125 48.734375 45.3125 54.390625 
Q 45.3125 60.0625 41.71875 63.234375 
Q 38.140625 66.40625 31.78125 66.40625 
Q 25.390625 66.40625 21.84375 63.234375 
Q 18.3125 60.0625 18.3125 54.390625 
z
" id="DejaVuSans-56"/>
      </defs>
      <g transform="translate(281.689641 239.238438)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-56"/>
      </g>
     </g>
    </g>
    <g id="xtick_6">
     <g id="line2d_6">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="358.743385" xlink:href="#m657296cf5c" y="224.64"/>
      </g>
     </g>
     <g id="text_6">
      <!-- 2020-09 -->
      <defs>
       <path d="M 10.984375 1.515625 
L 10.984375 10.5 
Q 14.703125 8.734375 18.5 7.8125 
Q 22.3125 6.890625 25.984375 6.890625 
Q 35.75 6.890625 40.890625 13.453125 
Q 46.046875 20.015625 46.78125 33.40625 
Q 43.953125 29.203125 39.59375 26.953125 
Q 35.25 24.703125 29.984375 24.703125 
Q 19.046875 24.703125 12.671875 31.3125 
Q 6.296875 37.9375 6.296875 49.421875 
Q 6.296875 60.640625 12.9375 67.421875 
Q 19.578125 74.21875 30.609375 74.21875 
Q 43.265625 74.21875 49.921875 64.515625 
Q 56.59375 54.828125 56.59375 36.375 
Q 56.59375 19.140625 48.40625 8.859375 
Q 40.234375 -1.421875 26.421875 -1.421875 
Q 22.703125 -1.421875 18.890625 -0.6875 
Q 15.09375 0.046875 10.984375 1.515625 
z
M 30.609375 32.421875 
Q 37.25 32.421875 41.125 36.953125 
Q 45.015625 41.5 45.015625 49.421875 
Q 45.015625 57.28125 41.125 61.84375 
Q 37.25 66.40625 30.609375 66.40625 
Q 23.96875 66.40625 20.09375 61.84375 
Q 16.21875 57.28125 16.21875 49.421875 
Q 16.21875 41.5 20.09375 36.953125 
Q 23.96875 32.421875 30.609375 32.421875 
z
" id="DejaVuSans-57"/>
      </defs>
      <g transform="translate(337.851978 239.238438)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-57"/>
      </g>
     </g>
    </g>
   </g>
   <g id="matplotlib.axis_2">
    <g id="ytick_1">
     <g id="line2d_7">
      <defs>
       <path d="M 0 0 
L -3.5 0 
" id="m7667c17bb5" style="stroke:#000000;stroke-width:0.8;"/>
      </defs>
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="30.103125" xlink:href="#m7667c17bb5" y="210.69707"/>
      </g>
     </g>
     <g id="text_7">
      <!-- 2,4 -->
      <defs>
       <path d="M 11.71875 12.40625 
L 22.015625 12.40625 
L 22.015625 4 
L 14.015625 -11.625 
L 7.71875 -11.625 
L 11.71875 4 
z
" id="DejaVuSans-44"/>
      </defs>
      <g transform="translate(7.2 214.496289)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-44"/>
       <use x="95.410156" xlink:href="#DejaVuSans-52"/>
      </g>
     </g>
    </g>
    <g id="ytick_2">
     <g id="line2d_8">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="30.103125" xlink:href="#m7667c17bb5" y="182.636279"/>
      </g>
     </g>
     <g id="text_8">
      <!-- 2,6 -->
      <g transform="translate(7.2 186.435498)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-44"/>
       <use x="95.410156" xlink:href="#DejaVuSans-54"/>
      </g>
     </g>
    </g>
    <g id="ytick_3">
     <g id="line2d_9">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="30.103125" xlink:href="#m7667c17bb5" y="154.575488"/>
      </g>
     </g>
     <g id="text_9">
      <!-- 2,8 -->
      <g transform="translate(7.2 158.374706)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-44"/>
       <use x="95.410156" xlink:href="#DejaVuSans-56"/>
      </g>
     </g>
    </g>
    <g id="ytick_4">
     <g id="line2d_10">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="30.103125" xlink:href="#m7667c17bb5" y="126.514696"/>
      </g>
     </g>
     <g id="text_10">
      <!-- 3,0 -->
      <defs>
       <path d="M 40.578125 39.3125 
Q 47.65625 37.796875 51.625 33 
Q 55.609375 28.21875 55.609375 21.1875 
Q 55.609375 10.40625 48.1875 4.484375 
Q 40.765625 -1.421875 27.09375 -1.421875 
Q 22.515625 -1.421875 17.65625 -0.515625 
Q 12.796875 0.390625 7.625 2.203125 
L 7.625 11.71875 
Q 11.71875 9.328125 16.59375 8.109375 
Q 21.484375 6.890625 26.8125 6.890625 
Q 36.078125 6.890625 40.9375 10.546875 
Q 45.796875 14.203125 45.796875 21.1875 
Q 45.796875 27.640625 41.28125 31.265625 
Q 36.765625 34.90625 28.71875 34.90625 
L 20.21875 34.90625 
L 20.21875 43.015625 
L 29.109375 43.015625 
Q 36.375 43.015625 40.234375 45.921875 
Q 44.09375 48.828125 44.09375 54.296875 
Q 44.09375 59.90625 40.109375 62.90625 
Q 36.140625 65.921875 28.71875 65.921875 
Q 24.65625 65.921875 20.015625 65.03125 
Q 15.375 64.15625 9.8125 62.3125 
L 9.8125 71.09375 
Q 15.4375 72.65625 20.34375 73.4375 
Q 25.25 74.21875 29.59375 74.21875 
Q 40.828125 74.21875 47.359375 69.109375 
Q 53.90625 64.015625 53.90625 55.328125 
Q 53.90625 49.265625 50.4375 45.09375 
Q 46.96875 40.921875 40.578125 39.3125 
z
" id="DejaVuSans-51"/>
      </defs>
      <g transform="translate(7.2 130.313915)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-51"/>
       <use x="63.623047" xlink:href="#DejaVuSans-44"/>
       <use x="95.410156" xlink:href="#DejaVuSans-48"/>
      </g>
     </g>
    </g>
    <g id="ytick_5">
     <g id="line2d_11">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="30.103125" xlink:href="#m7667c17bb5" y="98.453905"/>
      </g>
     </g>
     <g id="text_11">
      <!-- 3,2 -->
      <g transform="translate(7.2 102.253124)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-51"/>
       <use x="63.623047" xlink:href="#DejaVuSans-44"/>
       <use x="95.410156" xlink:href="#DejaVuSans-50"/>
      </g>
     </g>
    </g>
    <g id="ytick_6">
     <g id="line2d_12">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="30.103125" xlink:href="#m7667c17bb5" y="70.393114"/>
      </g>
     </g>
     <g id="text_12">
      <!-- 3,4 -->
      <g transform="translate(7.2 74.192333)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-51"/>
       <use x="63.623047" xlink:href="#DejaVuSans-44"/>
       <use x="95.410156" xlink:href="#DejaVuSans-52"/>
      </g>
     </g>
    </g>
    <g id="ytick_7">
     <g id="line2d_13">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="30.103125" xlink:href="#m7667c17bb5" y="42.332323"/>
      </g>
     </g>
     <g id="text_13">
      <!-- 3,6 -->
      <g transform="translate(7.2 46.131541)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-51"/>
       <use x="63.623047" xlink:href="#DejaVuSans-44"/>
       <use x="95.410156" xlink:href="#DejaVuSans-54"/>
      </g>
     </g>
    </g>
    <g id="ytick_8">
     <g id="line2d_14">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="30.103125" xlink:href="#m7667c17bb5" y="14.271531"/>
      </g>
     </g>
     <g id="text_14">
      <!-- 3,8 -->
      <g transform="translate(7.2 18.07075)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-51"/>
       <use x="63.623047" xlink:href="#DejaVuSans-44"/>
       <use x="95.410156" xlink:href="#DejaVuSans-56"/>
      </g>
     </g>
    </g>
   </g>
   <g id="line2d_15">
    <path clip-path="url(#p256a14affc)" d="M 45.321307 48.344888 
L 47.132995 36.624736 
L 48.944683 35.602018 
L 50.756372 32.541686 
L 52.56806 17.083636 
L 54.379748 25.589671 
L 56.191437 24.918924 
L 58.003125 31.790374 
L 59.814813 24.49486 
L 61.626502 35.629434 
L 63.43819 44.912742 
L 65.249878 26.550746 
L 67.061567 40.762032 
L 68.873255 35.87674 
L 70.684943 41.921553 
L 72.496631 40.153511 
L 74.30832 43.852181 
L 76.120008 54.396193 
L 77.931696 36.318888 
L 79.743385 48.666705 
L 81.555073 41.211174 
L 83.366761 46.236377 
L 85.17845 46.171138 
L 86.990138 59.26879 
L 88.801826 66.060395 
L 90.613515 52.867024 
L 92.425203 58.605482 
L 96.04858 65.97009 
L 99.671956 83.884213 
L 101.483644 85.54111 
L 103.295333 87.597189 
L 105.107021 85.915509 
L 106.918709 86.513052 
L 108.730398 92.24165 
L 110.542086 95.927025 
L 112.353774 104.422889 
L 114.165463 110.200771 
L 115.977151 98.680899 
L 117.788839 108.048077 
L 119.600528 110.38754 
L 121.412216 111.75901 
L 123.223904 118.051558 
L 125.035593 126.02917 
L 126.847281 132.664439 
L 128.658969 120.541184 
L 130.470657 129.832888 
L 132.282346 135.281183 
L 134.094034 130.220177 
L 135.905722 138.53269 
L 137.717411 144.533522 
L 139.529099 143.237021 
L 141.340787 133.274115 
L 144.964164 144.044095 
L 146.775852 147.727995 
L 148.587541 149.924817 
L 150.399229 158.975686 
L 152.210917 162.391403 
L 154.022606 151.741143 
L 155.834294 155.446721 
L 157.645982 158.87197 
L 159.45767 165.893627 
L 161.269359 150.104032 
L 163.081047 162.281712 
L 164.892735 176.263355 
L 166.704424 155.83984 
L 168.516112 172.391157 
L 170.3278 161.30328 
L 172.139489 183.88995 
L 173.951177 184.83467 
L 175.762865 188.598187 
L 177.574554 186.769221 
L 179.386242 173.041464 
L 181.19793 177.236084 
L 183.009619 174.363278 
L 184.821307 185.15286 
L 186.632995 190.309907 
L 188.444683 201.523598 
L 190.256372 207.435582 
L 192.06806 194.069096 
L 193.879748 176.678339 
L 195.691437 182.805976 
L 197.503125 191.53738 
L 199.314813 196.903711 
L 201.126502 200.489053 
L 202.93819 214.756364 
L 204.749878 180.251064 
L 206.561567 175.714403 
L 208.373255 178.082392 
L 210.184943 186.933241 
L 211.996631 187.427965 
L 213.80832 187.760027 
L 215.620008 189.106673 
L 219.243385 119.446217 
L 221.055073 151.008103 
L 222.866761 164.173855 
L 224.67845 160.340312 
L 226.490138 172.261924 
L 228.301826 186.442501 
L 230.113515 171.61984 
L 231.925203 178.224594 
L 233.736891 172.910846 
L 235.54858 181.740948 
L 237.360268 177.657769 
L 239.171956 189.963694 
L 240.983644 196.710578 
L 242.795333 178.509996 
L 244.607021 176.125653 
L 246.418709 182.499778 
L 248.230398 191.53738 
L 250.042086 190.832942 
L 251.853774 200.694561 
L 253.665463 199.876653 
L 255.477151 188.767211 
L 257.288839 189.963694 
L 259.100528 193.152789 
L 260.912216 185.794269 
L 262.723904 176.539697 
L 264.535593 183.268177 
L 266.347281 187.427965 
L 268.158969 164.060911 
L 269.970657 165.430254 
L 271.782346 162.721665 
L 273.594034 172.391157 
L 275.405722 166.010023 
L 277.217411 172.391157 
L 279.029099 167.305271 
L 280.840787 153.994709 
L 282.652476 148.161069 
L 284.464164 145.192266 
L 286.275852 150.373848 
L 288.087541 147.297978 
L 289.899229 154.668011 
L 291.710917 148.335164 
L 293.522606 126.453794 
L 295.334294 135.846693 
L 295.334294 135.846693 
" style="fill:none;stroke:#1f77b4;stroke-linecap:square;stroke-width:1.5;"/>
   </g>
   <g id="line2d_16">
    <path clip-path="url(#p256a14affc)" d="M 295.334294 135.846693 
" style="fill:none;stroke:#ff7f0e;stroke-linecap:square;stroke-width:1.5;"/>
   </g>
   <g id="line2d_17">
    <path clip-path="url(#p256a14affc)" d="M 297.145982 134.525524 
L 298.95767 139.445088 
L 300.769359 136.726753 
L 302.581047 142.665054 
L 304.392735 145.288055 
L 306.204424 127.299222 
L 308.016112 127.938897 
L 309.8278 128.000151 
L 311.639489 132.919715 
L 313.451177 130.20138 
L 315.262865 136.139681 
L 317.074554 138.762682 
L 318.886242 120.773849 
L 320.69793 121.413524 
L 322.509619 121.474778 
L 324.321307 126.394342 
L 326.132995 123.676006 
L 327.944683 129.614308 
L 329.756372 132.237309 
L 331.56806 114.248476 
L 333.379748 114.888151 
L 335.191437 114.949405 
L 337.003125 119.868969 
L 338.814813 117.150633 
L 340.626502 123.088935 
L 342.43819 125.711936 
L 344.249878 107.723103 
L 346.061567 108.362778 
L 347.873255 108.424032 
L 349.684943 113.343596 
" style="fill:none;stroke:#2ca02c;stroke-linecap:square;stroke-width:1.5;"/>
   </g>
   <g id="patch_3">
    <path d="M 30.103125 224.64 
L 30.103125 7.2 
" style="fill:none;stroke:#000000;stroke-linecap:square;stroke-linejoin:miter;stroke-width:0.8;"/>
   </g>
   <g id="patch_4">
    <path d="M 364.903125 224.64 
L 364.903125 7.2 
" style="fill:none;stroke:#000000;stroke-linecap:square;stroke-linejoin:miter;stroke-width:0.8;"/>
   </g>
   <g id="patch_5">
    <path d="M 30.103125 224.64 
L 364.903125 224.64 
" style="fill:none;stroke:#000000;stroke-linecap:square;stroke-linejoin:miter;stroke-width:0.8;"/>
   </g>
   <g id="patch_6">
    <path d="M 30.103125 7.2 
L 364.903125 7.2 
" style="fill:none;stroke:#000000;stroke-linecap:square;stroke-linejoin:miter;stroke-width:0.8;"/>
   </g>
   <g id="legend_1">
    <g id="patch_7">
     <path d="M 263.570313 59.234375 
L 357.903125 59.234375 
Q 359.903125 59.234375 359.903125 57.234375 
L 359.903125 14.2 
Q 359.903125 12.2 357.903125 12.2 
L 263.570313 12.2 
Q 261.570313 12.2 261.570313 14.2 
L 261.570313 57.234375 
Q 261.570313 59.234375 263.570313 59.234375 
z
" style="fill:#ffffff;opacity:0.8;stroke:#cccccc;stroke-linejoin:miter;"/>
    </g>
    <g id="line2d_18">
     <path d="M 265.570313 20.298438 
L 285.570313 20.298438 
" style="fill:none;stroke:#1f77b4;stroke-linecap:square;stroke-width:1.5;"/>
    </g>
    <g id="line2d_19"/>
    <g id="text_15">
     <!-- Train -->
     <defs>
      <path d="M -0.296875 72.90625 
L 61.375 72.90625 
L 61.375 64.59375 
L 35.5 64.59375 
L 35.5 0 
L 25.59375 0 
L 25.59375 64.59375 
L -0.296875 64.59375 
z
" id="DejaVuSans-84"/>
      <path d="M 41.109375 46.296875 
Q 39.59375 47.171875 37.8125 47.578125 
Q 36.03125 48 33.890625 48 
Q 26.265625 48 22.1875 43.046875 
Q 18.109375 38.09375 18.109375 28.8125 
L 18.109375 0 
L 9.078125 0 
L 9.078125 54.6875 
L 18.109375 54.6875 
L 18.109375 46.1875 
Q 20.953125 51.171875 25.484375 53.578125 
Q 30.03125 56 36.53125 56 
Q 37.453125 56 38.578125 55.875 
Q 39.703125 55.765625 41.0625 55.515625 
z
" id="DejaVuSans-114"/>
      <path d="M 34.28125 27.484375 
Q 23.390625 27.484375 19.1875 25 
Q 14.984375 22.515625 14.984375 16.5 
Q 14.984375 11.71875 18.140625 8.90625 
Q 21.296875 6.109375 26.703125 6.109375 
Q 34.1875 6.109375 38.703125 11.40625 
Q 43.21875 16.703125 43.21875 25.484375 
L 43.21875 27.484375 
z
M 52.203125 31.203125 
L 52.203125 0 
L 43.21875 0 
L 43.21875 8.296875 
Q 40.140625 3.328125 35.546875 0.953125 
Q 30.953125 -1.421875 24.3125 -1.421875 
Q 15.921875 -1.421875 10.953125 3.296875 
Q 6 8.015625 6 15.921875 
Q 6 25.140625 12.171875 29.828125 
Q 18.359375 34.515625 30.609375 34.515625 
L 43.21875 34.515625 
L 43.21875 35.40625 
Q 43.21875 41.609375 39.140625 45 
Q 35.0625 48.390625 27.6875 48.390625 
Q 23 48.390625 18.546875 47.265625 
Q 14.109375 46.140625 10.015625 43.890625 
L 10.015625 52.203125 
Q 14.9375 54.109375 19.578125 55.046875 
Q 24.21875 56 28.609375 56 
Q 40.484375 56 46.34375 49.84375 
Q 52.203125 43.703125 52.203125 31.203125 
z
" id="DejaVuSans-97"/>
      <path d="M 9.421875 54.6875 
L 18.40625 54.6875 
L 18.40625 0 
L 9.421875 0 
z
M 9.421875 75.984375 
L 18.40625 75.984375 
L 18.40625 64.59375 
L 9.421875 64.59375 
z
" id="DejaVuSans-105"/>
      <path d="M 54.890625 33.015625 
L 54.890625 0 
L 45.90625 0 
L 45.90625 32.71875 
Q 45.90625 40.484375 42.875 44.328125 
Q 39.84375 48.1875 33.796875 48.1875 
Q 26.515625 48.1875 22.3125 43.546875 
Q 18.109375 38.921875 18.109375 30.90625 
L 18.109375 0 
L 9.078125 0 
L 9.078125 54.6875 
L 18.109375 54.6875 
L 18.109375 46.1875 
Q 21.34375 51.125 25.703125 53.5625 
Q 30.078125 56 35.796875 56 
Q 45.21875 56 50.046875 50.171875 
Q 54.890625 44.34375 54.890625 33.015625 
z
" id="DejaVuSans-110"/>
     </defs>
     <g transform="translate(293.570313 23.798438)scale(0.1 -0.1)">
      <use xlink:href="#DejaVuSans-84"/>
      <use x="60.865234" xlink:href="#DejaVuSans-114"/>
      <use x="101.978516" xlink:href="#DejaVuSans-97"/>
      <use x="163.257812" xlink:href="#DejaVuSans-105"/>
      <use x="191.041016" xlink:href="#DejaVuSans-110"/>
     </g>
    </g>
    <g id="line2d_20">
     <path d="M 265.570313 34.976563 
L 285.570313 34.976563 
" style="fill:none;stroke:#ff7f0e;stroke-linecap:square;stroke-width:1.5;"/>
    </g>
    <g id="line2d_21"/>
    <g id="text_16">
     <!-- Test -->
     <defs>
      <path d="M 56.203125 29.59375 
L 56.203125 25.203125 
L 14.890625 25.203125 
Q 15.484375 15.921875 20.484375 11.0625 
Q 25.484375 6.203125 34.421875 6.203125 
Q 39.59375 6.203125 44.453125 7.46875 
Q 49.3125 8.734375 54.109375 11.28125 
L 54.109375 2.78125 
Q 49.265625 0.734375 44.1875 -0.34375 
Q 39.109375 -1.421875 33.890625 -1.421875 
Q 20.796875 -1.421875 13.15625 6.1875 
Q 5.515625 13.8125 5.515625 26.8125 
Q 5.515625 40.234375 12.765625 48.109375 
Q 20.015625 56 32.328125 56 
Q 43.359375 56 49.78125 48.890625 
Q 56.203125 41.796875 56.203125 29.59375 
z
M 47.21875 32.234375 
Q 47.125 39.59375 43.09375 43.984375 
Q 39.0625 48.390625 32.421875 48.390625 
Q 24.90625 48.390625 20.390625 44.140625 
Q 15.875 39.890625 15.1875 32.171875 
z
" id="DejaVuSans-101"/>
      <path d="M 44.28125 53.078125 
L 44.28125 44.578125 
Q 40.484375 46.53125 36.375 47.5 
Q 32.28125 48.484375 27.875 48.484375 
Q 21.1875 48.484375 17.84375 46.4375 
Q 14.5 44.390625 14.5 40.28125 
Q 14.5 37.15625 16.890625 35.375 
Q 19.28125 33.59375 26.515625 31.984375 
L 29.59375 31.296875 
Q 39.15625 29.25 43.1875 25.515625 
Q 47.21875 21.78125 47.21875 15.09375 
Q 47.21875 7.46875 41.1875 3.015625 
Q 35.15625 -1.421875 24.609375 -1.421875 
Q 20.21875 -1.421875 15.453125 -0.5625 
Q 10.6875 0.296875 5.421875 2 
L 5.421875 11.28125 
Q 10.40625 8.6875 15.234375 7.390625 
Q 20.0625 6.109375 24.8125 6.109375 
Q 31.15625 6.109375 34.5625 8.28125 
Q 37.984375 10.453125 37.984375 14.40625 
Q 37.984375 18.0625 35.515625 20.015625 
Q 33.0625 21.96875 24.703125 23.78125 
L 21.578125 24.515625 
Q 13.234375 26.265625 9.515625 29.90625 
Q 5.8125 33.546875 5.8125 39.890625 
Q 5.8125 47.609375 11.28125 51.796875 
Q 16.75 56 26.8125 56 
Q 31.78125 56 36.171875 55.265625 
Q 40.578125 54.546875 44.28125 53.078125 
z
" id="DejaVuSans-115"/>
      <path d="M 18.3125 70.21875 
L 18.3125 54.6875 
L 36.8125 54.6875 
L 36.8125 47.703125 
L 18.3125 47.703125 
L 18.3125 18.015625 
Q 18.3125 11.328125 20.140625 9.421875 
Q 21.96875 7.515625 27.59375 7.515625 
L 36.8125 7.515625 
L 36.8125 0 
L 27.59375 0 
Q 17.1875 0 13.234375 3.875 
Q 9.28125 7.765625 9.28125 18.015625 
L 9.28125 47.703125 
L 2.6875 47.703125 
L 2.6875 54.6875 
L 9.28125 54.6875 
L 9.28125 70.21875 
z
" id="DejaVuSans-116"/>
     </defs>
     <g transform="translate(293.570313 38.476563)scale(0.1 -0.1)">
      <use xlink:href="#DejaVuSans-84"/>
      <use x="60.818359" xlink:href="#DejaVuSans-101"/>
      <use x="122.341797" xlink:href="#DejaVuSans-115"/>
      <use x="174.441406" xlink:href="#DejaVuSans-116"/>
     </g>
    </g>
    <g id="line2d_22">
     <path d="M 265.570313 49.654688 
L 285.570313 49.654688 
" style="fill:none;stroke:#2ca02c;stroke-linecap:square;stroke-width:1.5;"/>
    </g>
    <g id="line2d_23"/>
    <g id="text_17">
     <!-- Holt-Winters -->
     <defs>
      <path d="M 9.8125 72.90625 
L 19.671875 72.90625 
L 19.671875 43.015625 
L 55.515625 43.015625 
L 55.515625 72.90625 
L 65.375 72.90625 
L 65.375 0 
L 55.515625 0 
L 55.515625 34.71875 
L 19.671875 34.71875 
L 19.671875 0 
L 9.8125 0 
z
" id="DejaVuSans-72"/>
      <path d="M 30.609375 48.390625 
Q 23.390625 48.390625 19.1875 42.75 
Q 14.984375 37.109375 14.984375 27.296875 
Q 14.984375 17.484375 19.15625 11.84375 
Q 23.34375 6.203125 30.609375 6.203125 
Q 37.796875 6.203125 41.984375 11.859375 
Q 46.1875 17.53125 46.1875 27.296875 
Q 46.1875 37.015625 41.984375 42.703125 
Q 37.796875 48.390625 30.609375 48.390625 
z
M 30.609375 56 
Q 42.328125 56 49.015625 48.375 
Q 55.71875 40.765625 55.71875 27.296875 
Q 55.71875 13.875 49.015625 6.21875 
Q 42.328125 -1.421875 30.609375 -1.421875 
Q 18.84375 -1.421875 12.171875 6.21875 
Q 5.515625 13.875 5.515625 27.296875 
Q 5.515625 40.765625 12.171875 48.375 
Q 18.84375 56 30.609375 56 
z
" id="DejaVuSans-111"/>
      <path d="M 9.421875 75.984375 
L 18.40625 75.984375 
L 18.40625 0 
L 9.421875 0 
z
" id="DejaVuSans-108"/>
      <path d="M 3.328125 72.90625 
L 13.28125 72.90625 
L 28.609375 11.28125 
L 43.890625 72.90625 
L 54.984375 72.90625 
L 70.3125 11.28125 
L 85.59375 72.90625 
L 95.609375 72.90625 
L 77.296875 0 
L 64.890625 0 
L 49.515625 63.28125 
L 33.984375 0 
L 21.578125 0 
z
" id="DejaVuSans-87"/>
     </defs>
     <g transform="translate(293.570313 53.154688)scale(0.1 -0.1)">
      <use xlink:href="#DejaVuSans-72"/>
      <use x="75.195312" xlink:href="#DejaVuSans-111"/>
      <use x="136.376953" xlink:href="#DejaVuSans-108"/>
      <use x="164.160156" xlink:href="#DejaVuSans-116"/>
      <use x="203.369141" xlink:href="#DejaVuSans-45"/>
      <use x="239.390625" xlink:href="#DejaVuSans-87"/>
      <use x="338.236328" xlink:href="#DejaVuSans-105"/>
      <use x="366.019531" xlink:href="#DejaVuSans-110"/>
      <use x="429.398438" xlink:href="#DejaVuSans-116"/>
      <use x="468.607422" xlink:href="#DejaVuSans-101"/>
      <use x="530.130859" xlink:href="#DejaVuSans-114"/>
      <use x="571.244141" xlink:href="#DejaVuSans-115"/>
     </g>
    </g>
   </g>
  </g>
 </g>
 <defs>
  <clipPath id="p256a14affc">
   <rect height="217.44" width="334.8" x="30.103125" y="7.2"/>
  </clipPath>
 </defs>
</svg>

</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[86]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">nowcast</span><span class="o">.</span><span class="n">index</span><span class="o">.</span><span class="n">freq</span> <span class="o">=</span> <span class="s1">&#39;D&#39;</span>
<span class="n">train</span><span class="p">,</span><span class="n">test</span> <span class="o">=</span> <span class="n">nowcast</span><span class="p">[</span><span class="s1">&#39;b&#39;</span><span class="p">][</span><span class="mi">10</span><span class="p">:],</span> <span class="n">nowcast</span><span class="p">[</span><span class="s1">&#39;b&#39;</span><span class="p">][</span><span class="o">-</span><span class="mi">1</span><span class="p">:]</span>
<span class="n">model</span> <span class="o">=</span> <span class="n">hw</span><span class="o">.</span><span class="n">ExponentialSmoothing</span><span class="p">(</span><span class="n">train</span><span class="p">,</span> <span class="n">trend</span><span class="o">=</span><span class="s1">&#39;mul&#39;</span><span class="p">,</span> <span class="n">seasonal</span><span class="o">=</span><span class="s1">&#39;mul&#39;</span><span class="p">,</span> <span class="n">damped</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">seasonal_periods</span><span class="o">=</span><span class="mi">7</span><span class="p">)</span><span class="o">.</span><span class="n">fit</span><span class="p">()</span>
<span class="n">pred</span> <span class="o">=</span> <span class="n">model</span><span class="o">.</span><span class="n">predict</span><span class="p">(</span><span class="n">start</span><span class="o">=</span><span class="n">test</span><span class="o">.</span><span class="n">index</span><span class="p">[</span><span class="mi">0</span><span class="p">],</span> <span class="n">end</span><span class="o">=</span><span class="n">test</span><span class="o">.</span><span class="n">index</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span><span class="o">+</span><span class="mi">70</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">plot</span><span class="p">(</span><span class="n">train</span><span class="o">.</span><span class="n">index</span><span class="p">,</span> <span class="n">train</span><span class="p">,</span> <span class="n">label</span><span class="o">=</span><span class="s1">&#39;Train&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">plot</span><span class="p">(</span><span class="n">test</span><span class="o">.</span><span class="n">index</span><span class="p">,</span> <span class="n">test</span><span class="p">,</span> <span class="n">label</span><span class="o">=</span><span class="s1">&#39;Test&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">plot</span><span class="p">(</span><span class="n">pred</span><span class="o">.</span><span class="n">index</span><span class="p">,</span> <span class="n">pred</span><span class="p">,</span> <span class="n">label</span><span class="o">=</span><span class="s1">&#39;Holt-Winters&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">legend</span><span class="p">(</span><span class="n">loc</span><span class="o">=</span><span class="s1">&#39;best&#39;</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[86]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>&lt;matplotlib.legend.Legend at 0x7ff19508af90&gt;</pre>
</div>

</div>

<div class="output_area">

    <div class="prompt"></div>



<div class="output_svg output_subarea ">
<?xml version="1.0" encoding="utf-8" standalone="no"?>
<!DOCTYPE svg PUBLIC "-//W3C//DTD SVG 1.1//EN"
  "http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd">
<!-- Created with matplotlib (https://matplotlib.org/) -->
<svg height="248.518125pt" version="1.1" viewBox="0 0 381.65 248.518125" width="381.65pt" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
 <defs>
  <style type="text/css">
*{stroke-linecap:butt;stroke-linejoin:round;}
  </style>
 </defs>
 <g id="figure_1">
  <g id="patch_1">
   <path d="M -0 248.518125 
L 381.65 248.518125 
L 381.65 0 
L -0 0 
z
" style="fill:none;"/>
  </g>
  <g id="axes_1">
   <g id="patch_2">
    <path d="M 39.65 224.64 
L 374.45 224.64 
L 374.45 7.2 
L 39.65 7.2 
z
" style="fill:#ffffff;"/>
   </g>
   <g id="matplotlib.axis_1">
    <g id="xtick_1">
     <g id="line2d_1">
      <defs>
       <path d="M 0 0 
L 0 3.5 
" id="m168dc6be6a" style="stroke:#000000;stroke-width:0.8;"/>
      </defs>
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="84.133916" xlink:href="#m168dc6be6a" y="224.64"/>
      </g>
     </g>
     <g id="text_1">
      <!-- 2020-04 -->
      <defs>
       <path d="M 19.1875 8.296875 
L 53.609375 8.296875 
L 53.609375 0 
L 7.328125 0 
L 7.328125 8.296875 
Q 12.9375 14.109375 22.625 23.890625 
Q 32.328125 33.6875 34.8125 36.53125 
Q 39.546875 41.84375 41.421875 45.53125 
Q 43.3125 49.21875 43.3125 52.78125 
Q 43.3125 58.59375 39.234375 62.25 
Q 35.15625 65.921875 28.609375 65.921875 
Q 23.96875 65.921875 18.8125 64.3125 
Q 13.671875 62.703125 7.8125 59.421875 
L 7.8125 69.390625 
Q 13.765625 71.78125 18.9375 73 
Q 24.125 74.21875 28.421875 74.21875 
Q 39.75 74.21875 46.484375 68.546875 
Q 53.21875 62.890625 53.21875 53.421875 
Q 53.21875 48.921875 51.53125 44.890625 
Q 49.859375 40.875 45.40625 35.40625 
Q 44.1875 33.984375 37.640625 27.21875 
Q 31.109375 20.453125 19.1875 8.296875 
z
" id="DejaVuSans-50"/>
       <path d="M 31.78125 66.40625 
Q 24.171875 66.40625 20.328125 58.90625 
Q 16.5 51.421875 16.5 36.375 
Q 16.5 21.390625 20.328125 13.890625 
Q 24.171875 6.390625 31.78125 6.390625 
Q 39.453125 6.390625 43.28125 13.890625 
Q 47.125 21.390625 47.125 36.375 
Q 47.125 51.421875 43.28125 58.90625 
Q 39.453125 66.40625 31.78125 66.40625 
z
M 31.78125 74.21875 
Q 44.046875 74.21875 50.515625 64.515625 
Q 56.984375 54.828125 56.984375 36.375 
Q 56.984375 17.96875 50.515625 8.265625 
Q 44.046875 -1.421875 31.78125 -1.421875 
Q 19.53125 -1.421875 13.0625 8.265625 
Q 6.59375 17.96875 6.59375 36.375 
Q 6.59375 54.828125 13.0625 64.515625 
Q 19.53125 74.21875 31.78125 74.21875 
z
" id="DejaVuSans-48"/>
       <path d="M 4.890625 31.390625 
L 31.203125 31.390625 
L 31.203125 23.390625 
L 4.890625 23.390625 
z
" id="DejaVuSans-45"/>
       <path d="M 37.796875 64.3125 
L 12.890625 25.390625 
L 37.796875 25.390625 
z
M 35.203125 72.90625 
L 47.609375 72.90625 
L 47.609375 25.390625 
L 58.015625 25.390625 
L 58.015625 17.1875 
L 47.609375 17.1875 
L 47.609375 0 
L 37.796875 0 
L 37.796875 17.1875 
L 4.890625 17.1875 
L 4.890625 26.703125 
z
" id="DejaVuSans-52"/>
      </defs>
      <g transform="translate(63.24251 239.238437)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-52"/>
      </g>
     </g>
    </g>
    <g id="xtick_2">
     <g id="line2d_2">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="128.032517" xlink:href="#m168dc6be6a" y="224.64"/>
      </g>
     </g>
     <g id="text_2">
      <!-- 2020-05 -->
      <defs>
       <path d="M 10.796875 72.90625 
L 49.515625 72.90625 
L 49.515625 64.59375 
L 19.828125 64.59375 
L 19.828125 46.734375 
Q 21.96875 47.46875 24.109375 47.828125 
Q 26.265625 48.1875 28.421875 48.1875 
Q 40.625 48.1875 47.75 41.5 
Q 54.890625 34.8125 54.890625 23.390625 
Q 54.890625 11.625 47.5625 5.09375 
Q 40.234375 -1.421875 26.90625 -1.421875 
Q 22.3125 -1.421875 17.546875 -0.640625 
Q 12.796875 0.140625 7.71875 1.703125 
L 7.71875 11.625 
Q 12.109375 9.234375 16.796875 8.0625 
Q 21.484375 6.890625 26.703125 6.890625 
Q 35.15625 6.890625 40.078125 11.328125 
Q 45.015625 15.765625 45.015625 23.390625 
Q 45.015625 31 40.078125 35.4375 
Q 35.15625 39.890625 26.703125 39.890625 
Q 22.75 39.890625 18.8125 39.015625 
Q 14.890625 38.140625 10.796875 36.28125 
z
" id="DejaVuSans-53"/>
      </defs>
      <g transform="translate(107.141111 239.238437)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-53"/>
      </g>
     </g>
    </g>
    <g id="xtick_3">
     <g id="line2d_3">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="173.394406" xlink:href="#m168dc6be6a" y="224.64"/>
      </g>
     </g>
     <g id="text_3">
      <!-- 2020-06 -->
      <defs>
       <path d="M 33.015625 40.375 
Q 26.375 40.375 22.484375 35.828125 
Q 18.609375 31.296875 18.609375 23.390625 
Q 18.609375 15.53125 22.484375 10.953125 
Q 26.375 6.390625 33.015625 6.390625 
Q 39.65625 6.390625 43.53125 10.953125 
Q 47.40625 15.53125 47.40625 23.390625 
Q 47.40625 31.296875 43.53125 35.828125 
Q 39.65625 40.375 33.015625 40.375 
z
M 52.59375 71.296875 
L 52.59375 62.3125 
Q 48.875 64.0625 45.09375 64.984375 
Q 41.3125 65.921875 37.59375 65.921875 
Q 27.828125 65.921875 22.671875 59.328125 
Q 17.53125 52.734375 16.796875 39.40625 
Q 19.671875 43.65625 24.015625 45.921875 
Q 28.375 48.1875 33.59375 48.1875 
Q 44.578125 48.1875 50.953125 41.515625 
Q 57.328125 34.859375 57.328125 23.390625 
Q 57.328125 12.15625 50.6875 5.359375 
Q 44.046875 -1.421875 33.015625 -1.421875 
Q 20.359375 -1.421875 13.671875 8.265625 
Q 6.984375 17.96875 6.984375 36.375 
Q 6.984375 53.65625 15.1875 63.9375 
Q 23.390625 74.21875 37.203125 74.21875 
Q 40.921875 74.21875 44.703125 73.484375 
Q 48.484375 72.75 52.59375 71.296875 
z
" id="DejaVuSans-54"/>
      </defs>
      <g transform="translate(152.502999 239.238437)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-54"/>
      </g>
     </g>
    </g>
    <g id="xtick_4">
     <g id="line2d_4">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="217.293007" xlink:href="#m168dc6be6a" y="224.64"/>
      </g>
     </g>
     <g id="text_4">
      <!-- 2020-07 -->
      <defs>
       <path d="M 8.203125 72.90625 
L 55.078125 72.90625 
L 55.078125 68.703125 
L 28.609375 0 
L 18.3125 0 
L 43.21875 64.59375 
L 8.203125 64.59375 
z
" id="DejaVuSans-55"/>
      </defs>
      <g transform="translate(196.401601 239.238437)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-55"/>
      </g>
     </g>
    </g>
    <g id="xtick_5">
     <g id="line2d_5">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="262.654895" xlink:href="#m168dc6be6a" y="224.64"/>
      </g>
     </g>
     <g id="text_5">
      <!-- 2020-08 -->
      <defs>
       <path d="M 31.78125 34.625 
Q 24.75 34.625 20.71875 30.859375 
Q 16.703125 27.09375 16.703125 20.515625 
Q 16.703125 13.921875 20.71875 10.15625 
Q 24.75 6.390625 31.78125 6.390625 
Q 38.8125 6.390625 42.859375 10.171875 
Q 46.921875 13.96875 46.921875 20.515625 
Q 46.921875 27.09375 42.890625 30.859375 
Q 38.875 34.625 31.78125 34.625 
z
M 21.921875 38.8125 
Q 15.578125 40.375 12.03125 44.71875 
Q 8.5 49.078125 8.5 55.328125 
Q 8.5 64.0625 14.71875 69.140625 
Q 20.953125 74.21875 31.78125 74.21875 
Q 42.671875 74.21875 48.875 69.140625 
Q 55.078125 64.0625 55.078125 55.328125 
Q 55.078125 49.078125 51.53125 44.71875 
Q 48 40.375 41.703125 38.8125 
Q 48.828125 37.15625 52.796875 32.3125 
Q 56.78125 27.484375 56.78125 20.515625 
Q 56.78125 9.90625 50.3125 4.234375 
Q 43.84375 -1.421875 31.78125 -1.421875 
Q 19.734375 -1.421875 13.25 4.234375 
Q 6.78125 9.90625 6.78125 20.515625 
Q 6.78125 27.484375 10.78125 32.3125 
Q 14.796875 37.15625 21.921875 38.8125 
z
M 18.3125 54.390625 
Q 18.3125 48.734375 21.84375 45.5625 
Q 25.390625 42.390625 31.78125 42.390625 
Q 38.140625 42.390625 41.71875 45.5625 
Q 45.3125 48.734375 45.3125 54.390625 
Q 45.3125 60.0625 41.71875 63.234375 
Q 38.140625 66.40625 31.78125 66.40625 
Q 25.390625 66.40625 21.84375 63.234375 
Q 18.3125 60.0625 18.3125 54.390625 
z
" id="DejaVuSans-56"/>
      </defs>
      <g transform="translate(241.763489 239.238437)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-56"/>
      </g>
     </g>
    </g>
    <g id="xtick_6">
     <g id="line2d_6">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="308.016783" xlink:href="#m168dc6be6a" y="224.64"/>
      </g>
     </g>
     <g id="text_6">
      <!-- 2020-09 -->
      <defs>
       <path d="M 10.984375 1.515625 
L 10.984375 10.5 
Q 14.703125 8.734375 18.5 7.8125 
Q 22.3125 6.890625 25.984375 6.890625 
Q 35.75 6.890625 40.890625 13.453125 
Q 46.046875 20.015625 46.78125 33.40625 
Q 43.953125 29.203125 39.59375 26.953125 
Q 35.25 24.703125 29.984375 24.703125 
Q 19.046875 24.703125 12.671875 31.3125 
Q 6.296875 37.9375 6.296875 49.421875 
Q 6.296875 60.640625 12.9375 67.421875 
Q 19.578125 74.21875 30.609375 74.21875 
Q 43.265625 74.21875 49.921875 64.515625 
Q 56.59375 54.828125 56.59375 36.375 
Q 56.59375 19.140625 48.40625 8.859375 
Q 40.234375 -1.421875 26.421875 -1.421875 
Q 22.703125 -1.421875 18.890625 -0.6875 
Q 15.09375 0.046875 10.984375 1.515625 
z
M 30.609375 32.421875 
Q 37.25 32.421875 41.125 36.953125 
Q 45.015625 41.5 45.015625 49.421875 
Q 45.015625 57.28125 41.125 61.84375 
Q 37.25 66.40625 30.609375 66.40625 
Q 23.96875 66.40625 20.09375 61.84375 
Q 16.21875 57.28125 16.21875 49.421875 
Q 16.21875 41.5 20.09375 36.953125 
Q 23.96875 32.421875 30.609375 32.421875 
z
" id="DejaVuSans-57"/>
      </defs>
      <g transform="translate(287.125377 239.238437)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-48"/>
       <use x="354.199219" xlink:href="#DejaVuSans-57"/>
      </g>
     </g>
    </g>
    <g id="xtick_7">
     <g id="line2d_7">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="351.915385" xlink:href="#m168dc6be6a" y="224.64"/>
      </g>
     </g>
     <g id="text_7">
      <!-- 2020-10 -->
      <defs>
       <path d="M 12.40625 8.296875 
L 28.515625 8.296875 
L 28.515625 63.921875 
L 10.984375 60.40625 
L 10.984375 69.390625 
L 28.421875 72.90625 
L 38.28125 72.90625 
L 38.28125 8.296875 
L 54.390625 8.296875 
L 54.390625 0 
L 12.40625 0 
z
" id="DejaVuSans-49"/>
      </defs>
      <g transform="translate(331.023978 239.238437)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-50"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
       <use x="254.492188" xlink:href="#DejaVuSans-45"/>
       <use x="290.576172" xlink:href="#DejaVuSans-49"/>
       <use x="354.199219" xlink:href="#DejaVuSans-48"/>
      </g>
     </g>
    </g>
   </g>
   <g id="matplotlib.axis_2">
    <g id="ytick_1">
     <g id="line2d_8">
      <defs>
       <path d="M 0 0 
L -3.5 0 
" id="m27552975d2" style="stroke:#000000;stroke-width:0.8;"/>
      </defs>
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="39.65" xlink:href="#m27552975d2" y="222.77935"/>
      </g>
     </g>
     <g id="text_8">
      <!-- 0 -->
      <g transform="translate(26.2875 226.578569)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-48"/>
      </g>
     </g>
    </g>
    <g id="ytick_2">
     <g id="line2d_9">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="39.65" xlink:href="#m27552975d2" y="188.638983"/>
      </g>
     </g>
     <g id="text_9">
      <!-- 1000 -->
      <g transform="translate(7.2 192.438201)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-49"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-48"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
      </g>
     </g>
    </g>
    <g id="ytick_3">
     <g id="line2d_10">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="39.65" xlink:href="#m27552975d2" y="154.498615"/>
      </g>
     </g>
     <g id="text_10">
      <!-- 2000 -->
      <g transform="translate(7.2 158.297834)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-50"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-48"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
      </g>
     </g>
    </g>
    <g id="ytick_4">
     <g id="line2d_11">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="39.65" xlink:href="#m27552975d2" y="120.358248"/>
      </g>
     </g>
     <g id="text_11">
      <!-- 3000 -->
      <defs>
       <path d="M 40.578125 39.3125 
Q 47.65625 37.796875 51.625 33 
Q 55.609375 28.21875 55.609375 21.1875 
Q 55.609375 10.40625 48.1875 4.484375 
Q 40.765625 -1.421875 27.09375 -1.421875 
Q 22.515625 -1.421875 17.65625 -0.515625 
Q 12.796875 0.390625 7.625 2.203125 
L 7.625 11.71875 
Q 11.71875 9.328125 16.59375 8.109375 
Q 21.484375 6.890625 26.8125 6.890625 
Q 36.078125 6.890625 40.9375 10.546875 
Q 45.796875 14.203125 45.796875 21.1875 
Q 45.796875 27.640625 41.28125 31.265625 
Q 36.765625 34.90625 28.71875 34.90625 
L 20.21875 34.90625 
L 20.21875 43.015625 
L 29.109375 43.015625 
Q 36.375 43.015625 40.234375 45.921875 
Q 44.09375 48.828125 44.09375 54.296875 
Q 44.09375 59.90625 40.109375 62.90625 
Q 36.140625 65.921875 28.71875 65.921875 
Q 24.65625 65.921875 20.015625 65.03125 
Q 15.375 64.15625 9.8125 62.3125 
L 9.8125 71.09375 
Q 15.4375 72.65625 20.34375 73.4375 
Q 25.25 74.21875 29.59375 74.21875 
Q 40.828125 74.21875 47.359375 69.109375 
Q 53.90625 64.015625 53.90625 55.328125 
Q 53.90625 49.265625 50.4375 45.09375 
Q 46.96875 40.921875 40.578125 39.3125 
z
" id="DejaVuSans-51"/>
      </defs>
      <g transform="translate(7.2 124.157467)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-51"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-48"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
      </g>
     </g>
    </g>
    <g id="ytick_5">
     <g id="line2d_12">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="39.65" xlink:href="#m27552975d2" y="86.21788"/>
      </g>
     </g>
     <g id="text_12">
      <!-- 4000 -->
      <g transform="translate(7.2 90.017099)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-52"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-48"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
      </g>
     </g>
    </g>
    <g id="ytick_6">
     <g id="line2d_13">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="39.65" xlink:href="#m27552975d2" y="52.077513"/>
      </g>
     </g>
     <g id="text_13">
      <!-- 5000 -->
      <g transform="translate(7.2 55.876732)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-53"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-48"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
      </g>
     </g>
    </g>
    <g id="ytick_7">
     <g id="line2d_14">
      <g>
       <use style="stroke:#000000;stroke-width:0.8;" x="39.65" xlink:href="#m27552975d2" y="17.937146"/>
      </g>
     </g>
     <g id="text_14">
      <!-- 6000 -->
      <g transform="translate(7.2 21.736364)scale(0.1 -0.1)">
       <use xlink:href="#DejaVuSans-54"/>
       <use x="63.623047" xlink:href="#DejaVuSans-48"/>
       <use x="127.246094" xlink:href="#DejaVuSans-48"/>
       <use x="190.869141" xlink:href="#DejaVuSans-48"/>
      </g>
     </g>
    </g>
   </g>
   <g id="line2d_15">
    <path clip-path="url(#pa6d2dffbe1)" d="M 54.868182 99.635045 
L 56.331469 73.517664 
L 57.794755 70.991276 
L 59.258042 63.173132 
L 60.721329 17.083636 
L 62.184615 43.883825 
L 63.647902 41.903683 
L 65.111189 61.192991 
L 66.574476 40.64049 
L 68.037762 71.059557 
L 69.501049 92.499708 
L 70.964336 46.683335 
L 72.427622 83.315949 
L 73.890909 71.674084 
L 75.354196 85.944757 
L 76.817483 81.916194 
L 78.280769 90.212303 
L 79.744056 111.27691 
L 81.207343 72.766576 
L 82.670629 100.283712 
L 84.133916 84.34016 
L 85.597203 95.299218 
L 87.06049 95.162657 
L 88.523776 119.846142 
L 89.987063 130.702779 
L 91.45035 108.44326 
L 92.913636 118.71951 
L 95.84021 130.566218 
L 97.303497 143.334715 
L 98.766783 154.05479 
L 100.23007 155.89837 
L 101.693357 158.117494 
L 103.156643 156.308055 
L 104.61993 156.956722 
L 106.083217 162.863005 
L 107.546503 166.379463 
L 109.00979 173.719642 
L 110.473077 178.15789 
L 111.936364 168.87171 
L 113.39965 176.553293 
L 114.862937 178.294451 
L 116.326224 179.284522 
L 117.78951 183.552068 
L 119.252797 188.36586 
L 120.716084 191.916458 
L 122.179371 185.122525 
L 123.642657 190.448422 
L 125.105944 193.213792 
L 126.569231 190.653264 
L 128.032517 194.750108 
L 129.495804 197.378917 
L 130.959091 196.832671 
L 132.422378 192.223721 
L 135.348951 197.174074 
L 136.812238 198.676251 
L 138.275524 199.52976 
L 139.738811 202.738954 
L 141.202098 203.831446 
L 142.665385 200.212567 
L 144.128671 201.544041 
L 145.591958 202.704814 
L 147.055245 204.889797 
L 148.518531 199.598041 
L 151.445105 207.689308 
L 152.908392 201.680603 
L 154.371678 206.699237 
L 155.834965 203.490042 
L 157.298252 209.464607 
L 158.761538 209.669449 
L 160.224825 210.454677 
L 161.688112 210.079133 
L 163.151399 206.869939 
L 164.614685 207.92829 
L 166.077972 207.211342 
L 167.541259 209.73773 
L 169.004545 210.796081 
L 170.467832 212.810363 
L 171.931119 213.732153 
L 173.394406 211.513029 
L 174.857692 207.791729 
L 176.320979 209.225624 
L 177.784266 211.035064 
L 179.247552 212.025134 
L 180.710839 212.639661 
L 182.174126 214.756364 
L 183.637413 208.645238 
L 185.100699 207.552746 
L 186.563986 208.133132 
L 188.027273 210.113274 
L 190.953846 210.283976 
L 192.417133 210.557098 
L 193.88042 200.758813 
L 195.343706 184.439717 
L 196.806993 199.939444 
L 198.27028 204.377692 
L 199.733566 203.182779 
L 202.66014 210.010853 
L 204.123427 206.494395 
L 205.586713 208.167273 
L 207.05 206.835798 
L 208.513287 208.986642 
L 209.976573 208.030711 
L 211.43986 210.7278 
L 212.903147 211.990994 
L 214.366434 208.235553 
L 215.82972 207.655167 
L 217.293007 209.157343 
L 218.756294 211.035064 
L 220.21958 210.898502 
L 221.682867 212.673801 
L 223.146154 212.53724 
L 224.609441 210.488818 
L 226.072727 210.7278 
L 227.536014 211.342327 
L 228.999301 209.874291 
L 230.462587 207.757588 
L 231.925874 209.328045 
L 233.389161 210.215695 
L 234.852448 204.343552 
L 236.315734 204.753236 
L 237.779021 203.933867 
L 239.242308 206.699237 
L 240.705594 204.923938 
L 242.168881 206.699237 
L 243.632168 205.299482 
L 245.095455 201.031936 
L 246.558741 198.846952 
L 248.022028 197.65204 
L 249.485315 199.700462 
L 250.948601 198.505549 
L 252.411888 201.270919 
L 253.875175 198.915233 
L 255.338462 188.604842 
L 256.801748 193.486915 
L 256.801748 193.486915 
" style="fill:none;stroke:#1f77b4;stroke-linecap:square;stroke-width:1.5;"/>
   </g>
   <g id="line2d_16">
    <path clip-path="url(#pa6d2dffbe1)" d="M 256.801748 193.486915 
" style="fill:none;stroke:#ff7f0e;stroke-linecap:square;stroke-width:1.5;"/>
   </g>
   <g id="line2d_17">
    <path clip-path="url(#pa6d2dffbe1)" d="M 256.801748 190.581283 
L 258.265035 191.400778 
L 259.728322 193.934062 
L 261.191608 191.1649 
L 262.654895 194.202527 
L 264.118182 192.308801 
L 265.581469 183.102792 
L 267.044755 185.911052 
L 268.508042 185.245623 
L 269.971329 188.27645 
L 271.434615 184.964831 
L 272.897902 188.598795 
L 274.361189 186.334373 
L 275.824476 175.324171 
L 277.287762 178.683782 
L 278.751049 177.888714 
L 280.214336 181.514345 
L 281.677622 177.554503 
L 283.140909 181.901328 
L 284.604196 179.193987 
L 286.067483 166.027656 
L 287.530769 170.046361 
L 288.994056 169.096516 
L 290.457343 173.433139 
L 291.920629 168.698781 
L 293.383916 173.897656 
L 294.847203 170.661166 
L 296.31049 154.918441 
L 297.773776 159.72494 
L 299.237063 158.590329 
L 300.70035 163.776721 
L 302.163636 158.117066 
L 303.626923 164.334227 
L 305.09021 160.465649 
L 306.553497 141.644734 
L 308.016783 147.392739 
L 309.48007 146.037591 
L 310.943357 152.239489 
L 312.406643 145.474538 
L 313.86993 152.908504 
L 315.333217 148.284969 
L 316.796503 125.786795 
L 318.25979 132.659869 
L 319.723077 131.041521 
L 321.186364 138.456833 
L 322.64965 130.371741 
L 324.112937 139.259547 
L 325.576224 133.734414 
L 327.03951 106.843871 
L 328.502797 115.061198 
L 329.966084 113.128772 
L 331.429371 121.993797 
L 332.892657 112.33215 
L 334.355944 122.956793 
L 335.819231 116.355072 
L 337.282517 84.218639 
L 338.745804 94.041902 
L 340.209091 91.734734 
L 341.672378 102.33157 
L 343.135664 90.787387 
L 344.598951 103.486688 
L 346.062238 95.599587 
L 347.525524 57.198668 
L 348.988811 68.940253 
L 350.452098 66.186015 
L 351.915385 78.851395 
L 353.378671 65.05959 
L 354.841958 80.23677 
L 356.305245 70.815194 
L 357.768531 24.934347 
L 359.231818 38.967118 
" style="fill:none;stroke:#2ca02c;stroke-linecap:square;stroke-width:1.5;"/>
   </g>
   <g id="patch_3">
    <path d="M 39.65 224.64 
L 39.65 7.2 
" style="fill:none;stroke:#000000;stroke-linecap:square;stroke-linejoin:miter;stroke-width:0.8;"/>
   </g>
   <g id="patch_4">
    <path d="M 374.45 224.64 
L 374.45 7.2 
" style="fill:none;stroke:#000000;stroke-linecap:square;stroke-linejoin:miter;stroke-width:0.8;"/>
   </g>
   <g id="patch_5">
    <path d="M 39.65 224.64 
L 374.45 224.64 
" style="fill:none;stroke:#000000;stroke-linecap:square;stroke-linejoin:miter;stroke-width:0.8;"/>
   </g>
   <g id="patch_6">
    <path d="M 39.65 7.2 
L 374.45 7.2 
" style="fill:none;stroke:#000000;stroke-linecap:square;stroke-linejoin:miter;stroke-width:0.8;"/>
   </g>
   <g id="legend_1">
    <g id="patch_7">
     <path d="M 159.883594 59.234375 
L 254.216406 59.234375 
Q 256.216406 59.234375 256.216406 57.234375 
L 256.216406 14.2 
Q 256.216406 12.2 254.216406 12.2 
L 159.883594 12.2 
Q 157.883594 12.2 157.883594 14.2 
L 157.883594 57.234375 
Q 157.883594 59.234375 159.883594 59.234375 
z
" style="fill:#ffffff;opacity:0.8;stroke:#cccccc;stroke-linejoin:miter;"/>
    </g>
    <g id="line2d_18">
     <path d="M 161.883594 20.298437 
L 181.883594 20.298437 
" style="fill:none;stroke:#1f77b4;stroke-linecap:square;stroke-width:1.5;"/>
    </g>
    <g id="line2d_19"/>
    <g id="text_15">
     <!-- Train -->
     <defs>
      <path d="M -0.296875 72.90625 
L 61.375 72.90625 
L 61.375 64.59375 
L 35.5 64.59375 
L 35.5 0 
L 25.59375 0 
L 25.59375 64.59375 
L -0.296875 64.59375 
z
" id="DejaVuSans-84"/>
      <path d="M 41.109375 46.296875 
Q 39.59375 47.171875 37.8125 47.578125 
Q 36.03125 48 33.890625 48 
Q 26.265625 48 22.1875 43.046875 
Q 18.109375 38.09375 18.109375 28.8125 
L 18.109375 0 
L 9.078125 0 
L 9.078125 54.6875 
L 18.109375 54.6875 
L 18.109375 46.1875 
Q 20.953125 51.171875 25.484375 53.578125 
Q 30.03125 56 36.53125 56 
Q 37.453125 56 38.578125 55.875 
Q 39.703125 55.765625 41.0625 55.515625 
z
" id="DejaVuSans-114"/>
      <path d="M 34.28125 27.484375 
Q 23.390625 27.484375 19.1875 25 
Q 14.984375 22.515625 14.984375 16.5 
Q 14.984375 11.71875 18.140625 8.90625 
Q 21.296875 6.109375 26.703125 6.109375 
Q 34.1875 6.109375 38.703125 11.40625 
Q 43.21875 16.703125 43.21875 25.484375 
L 43.21875 27.484375 
z
M 52.203125 31.203125 
L 52.203125 0 
L 43.21875 0 
L 43.21875 8.296875 
Q 40.140625 3.328125 35.546875 0.953125 
Q 30.953125 -1.421875 24.3125 -1.421875 
Q 15.921875 -1.421875 10.953125 3.296875 
Q 6 8.015625 6 15.921875 
Q 6 25.140625 12.171875 29.828125 
Q 18.359375 34.515625 30.609375 34.515625 
L 43.21875 34.515625 
L 43.21875 35.40625 
Q 43.21875 41.609375 39.140625 45 
Q 35.0625 48.390625 27.6875 48.390625 
Q 23 48.390625 18.546875 47.265625 
Q 14.109375 46.140625 10.015625 43.890625 
L 10.015625 52.203125 
Q 14.9375 54.109375 19.578125 55.046875 
Q 24.21875 56 28.609375 56 
Q 40.484375 56 46.34375 49.84375 
Q 52.203125 43.703125 52.203125 31.203125 
z
" id="DejaVuSans-97"/>
      <path d="M 9.421875 54.6875 
L 18.40625 54.6875 
L 18.40625 0 
L 9.421875 0 
z
M 9.421875 75.984375 
L 18.40625 75.984375 
L 18.40625 64.59375 
L 9.421875 64.59375 
z
" id="DejaVuSans-105"/>
      <path d="M 54.890625 33.015625 
L 54.890625 0 
L 45.90625 0 
L 45.90625 32.71875 
Q 45.90625 40.484375 42.875 44.328125 
Q 39.84375 48.1875 33.796875 48.1875 
Q 26.515625 48.1875 22.3125 43.546875 
Q 18.109375 38.921875 18.109375 30.90625 
L 18.109375 0 
L 9.078125 0 
L 9.078125 54.6875 
L 18.109375 54.6875 
L 18.109375 46.1875 
Q 21.34375 51.125 25.703125 53.5625 
Q 30.078125 56 35.796875 56 
Q 45.21875 56 50.046875 50.171875 
Q 54.890625 44.34375 54.890625 33.015625 
z
" id="DejaVuSans-110"/>
     </defs>
     <g transform="translate(189.883594 23.798437)scale(0.1 -0.1)">
      <use xlink:href="#DejaVuSans-84"/>
      <use x="60.865234" xlink:href="#DejaVuSans-114"/>
      <use x="101.978516" xlink:href="#DejaVuSans-97"/>
      <use x="163.257812" xlink:href="#DejaVuSans-105"/>
      <use x="191.041016" xlink:href="#DejaVuSans-110"/>
     </g>
    </g>
    <g id="line2d_20">
     <path d="M 161.883594 34.976562 
L 181.883594 34.976562 
" style="fill:none;stroke:#ff7f0e;stroke-linecap:square;stroke-width:1.5;"/>
    </g>
    <g id="line2d_21"/>
    <g id="text_16">
     <!-- Test -->
     <defs>
      <path d="M 56.203125 29.59375 
L 56.203125 25.203125 
L 14.890625 25.203125 
Q 15.484375 15.921875 20.484375 11.0625 
Q 25.484375 6.203125 34.421875 6.203125 
Q 39.59375 6.203125 44.453125 7.46875 
Q 49.3125 8.734375 54.109375 11.28125 
L 54.109375 2.78125 
Q 49.265625 0.734375 44.1875 -0.34375 
Q 39.109375 -1.421875 33.890625 -1.421875 
Q 20.796875 -1.421875 13.15625 6.1875 
Q 5.515625 13.8125 5.515625 26.8125 
Q 5.515625 40.234375 12.765625 48.109375 
Q 20.015625 56 32.328125 56 
Q 43.359375 56 49.78125 48.890625 
Q 56.203125 41.796875 56.203125 29.59375 
z
M 47.21875 32.234375 
Q 47.125 39.59375 43.09375 43.984375 
Q 39.0625 48.390625 32.421875 48.390625 
Q 24.90625 48.390625 20.390625 44.140625 
Q 15.875 39.890625 15.1875 32.171875 
z
" id="DejaVuSans-101"/>
      <path d="M 44.28125 53.078125 
L 44.28125 44.578125 
Q 40.484375 46.53125 36.375 47.5 
Q 32.28125 48.484375 27.875 48.484375 
Q 21.1875 48.484375 17.84375 46.4375 
Q 14.5 44.390625 14.5 40.28125 
Q 14.5 37.15625 16.890625 35.375 
Q 19.28125 33.59375 26.515625 31.984375 
L 29.59375 31.296875 
Q 39.15625 29.25 43.1875 25.515625 
Q 47.21875 21.78125 47.21875 15.09375 
Q 47.21875 7.46875 41.1875 3.015625 
Q 35.15625 -1.421875 24.609375 -1.421875 
Q 20.21875 -1.421875 15.453125 -0.5625 
Q 10.6875 0.296875 5.421875 2 
L 5.421875 11.28125 
Q 10.40625 8.6875 15.234375 7.390625 
Q 20.0625 6.109375 24.8125 6.109375 
Q 31.15625 6.109375 34.5625 8.28125 
Q 37.984375 10.453125 37.984375 14.40625 
Q 37.984375 18.0625 35.515625 20.015625 
Q 33.0625 21.96875 24.703125 23.78125 
L 21.578125 24.515625 
Q 13.234375 26.265625 9.515625 29.90625 
Q 5.8125 33.546875 5.8125 39.890625 
Q 5.8125 47.609375 11.28125 51.796875 
Q 16.75 56 26.8125 56 
Q 31.78125 56 36.171875 55.265625 
Q 40.578125 54.546875 44.28125 53.078125 
z
" id="DejaVuSans-115"/>
      <path d="M 18.3125 70.21875 
L 18.3125 54.6875 
L 36.8125 54.6875 
L 36.8125 47.703125 
L 18.3125 47.703125 
L 18.3125 18.015625 
Q 18.3125 11.328125 20.140625 9.421875 
Q 21.96875 7.515625 27.59375 7.515625 
L 36.8125 7.515625 
L 36.8125 0 
L 27.59375 0 
Q 17.1875 0 13.234375 3.875 
Q 9.28125 7.765625 9.28125 18.015625 
L 9.28125 47.703125 
L 2.6875 47.703125 
L 2.6875 54.6875 
L 9.28125 54.6875 
L 9.28125 70.21875 
z
" id="DejaVuSans-116"/>
     </defs>
     <g transform="translate(189.883594 38.476562)scale(0.1 -0.1)">
      <use xlink:href="#DejaVuSans-84"/>
      <use x="60.818359" xlink:href="#DejaVuSans-101"/>
      <use x="122.341797" xlink:href="#DejaVuSans-115"/>
      <use x="174.441406" xlink:href="#DejaVuSans-116"/>
     </g>
    </g>
    <g id="line2d_22">
     <path d="M 161.883594 49.654687 
L 181.883594 49.654687 
" style="fill:none;stroke:#2ca02c;stroke-linecap:square;stroke-width:1.5;"/>
    </g>
    <g id="line2d_23"/>
    <g id="text_17">
     <!-- Holt-Winters -->
     <defs>
      <path d="M 9.8125 72.90625 
L 19.671875 72.90625 
L 19.671875 43.015625 
L 55.515625 43.015625 
L 55.515625 72.90625 
L 65.375 72.90625 
L 65.375 0 
L 55.515625 0 
L 55.515625 34.71875 
L 19.671875 34.71875 
L 19.671875 0 
L 9.8125 0 
z
" id="DejaVuSans-72"/>
      <path d="M 30.609375 48.390625 
Q 23.390625 48.390625 19.1875 42.75 
Q 14.984375 37.109375 14.984375 27.296875 
Q 14.984375 17.484375 19.15625 11.84375 
Q 23.34375 6.203125 30.609375 6.203125 
Q 37.796875 6.203125 41.984375 11.859375 
Q 46.1875 17.53125 46.1875 27.296875 
Q 46.1875 37.015625 41.984375 42.703125 
Q 37.796875 48.390625 30.609375 48.390625 
z
M 30.609375 56 
Q 42.328125 56 49.015625 48.375 
Q 55.71875 40.765625 55.71875 27.296875 
Q 55.71875 13.875 49.015625 6.21875 
Q 42.328125 -1.421875 30.609375 -1.421875 
Q 18.84375 -1.421875 12.171875 6.21875 
Q 5.515625 13.875 5.515625 27.296875 
Q 5.515625 40.765625 12.171875 48.375 
Q 18.84375 56 30.609375 56 
z
" id="DejaVuSans-111"/>
      <path d="M 9.421875 75.984375 
L 18.40625 75.984375 
L 18.40625 0 
L 9.421875 0 
z
" id="DejaVuSans-108"/>
      <path d="M 3.328125 72.90625 
L 13.28125 72.90625 
L 28.609375 11.28125 
L 43.890625 72.90625 
L 54.984375 72.90625 
L 70.3125 11.28125 
L 85.59375 72.90625 
L 95.609375 72.90625 
L 77.296875 0 
L 64.890625 0 
L 49.515625 63.28125 
L 33.984375 0 
L 21.578125 0 
z
" id="DejaVuSans-87"/>
     </defs>
     <g transform="translate(189.883594 53.154687)scale(0.1 -0.1)">
      <use xlink:href="#DejaVuSans-72"/>
      <use x="75.195312" xlink:href="#DejaVuSans-111"/>
      <use x="136.376953" xlink:href="#DejaVuSans-108"/>
      <use x="164.160156" xlink:href="#DejaVuSans-116"/>
      <use x="203.369141" xlink:href="#DejaVuSans-45"/>
      <use x="239.390625" xlink:href="#DejaVuSans-87"/>
      <use x="338.236328" xlink:href="#DejaVuSans-105"/>
      <use x="366.019531" xlink:href="#DejaVuSans-110"/>
      <use x="429.398438" xlink:href="#DejaVuSans-116"/>
      <use x="468.607422" xlink:href="#DejaVuSans-101"/>
      <use x="530.130859" xlink:href="#DejaVuSans-114"/>
      <use x="571.244141" xlink:href="#DejaVuSans-115"/>
     </g>
    </g>
   </g>
  </g>
 </g>
 <defs>
  <clipPath id="pa6d2dffbe1">
   <rect height="217.44" width="334.8" x="39.65" y="7.2"/>
  </clipPath>
 </defs>
</svg>

</div>

</div>

</div>
</div>

</div>
    </div>
  </div>
</body>

 


</html>
