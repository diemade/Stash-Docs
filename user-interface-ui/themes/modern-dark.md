---
layout: clean
title: Modern Dark
nav_order: 6
parent: Themes
grand_parent: User Interface (UI)

---

<details markdown="block">
  <summary>
    Table of Contents
  </summary>
  {: .text-delta }
1. TOC
{:toc}
</details>

This theme was inspired by Plex Interface. Installation is quick and easy, so you should be ready to install it in just a few simple steps. 

Feel free to experiment with CSS and modify it to fit your needs. In case you have any issues or improvements, DM me on Discord!

{: .note }
The Images and Markers pages are hidden on mobile in this theme to keep a perfect 2x3 nav menu. Those pages can be restored by commenting out or removing the following section:

```css
div[data-rb-event-key="/images"] {
   display: none;
}
div[data-rb-event-key="/scenes/markers"] {
   display: none;
}
```

## Screenshots

![Modern Dark preview #1](/assets/user-interface-ui/themes/modern-dark-1.jpg)

## Install

1. Open User **Interface** Configuration panel in **settings**. (http://localhost:9999/settings?tab=interface)
2. Tick/Enable Custom CSS ✅ 
3. Copy&Paste [CSS Code](#css-code) to the Custom CSS text area. 
4. In your config.yml file, update the value of the `theme_color` property to `#191919`.

Enjoy!

## CSS Code

```css
/* Modern Dark Theme by cj13 v1.2 */
 :root {
     --nav-color: #212121;
     --body-color: #191919;
     --card-color: #2a2a2a;
     --plex-yelow: #e5a00d;
     --tag-color: #555555;
}
 #scrubber-position-indicator {
     background-color: #e5a00d;
}
 .scrubber-tags-background {
     background-color: #e5a00d;
     opacity: 30%;
}
 body {
     width: 100%;
     height: 100%;
     background: var(--body-color);
}
 .text-white {
     color: #cbced2 !important;
}
 #root {
     position: absolute;
     width: 100%;
     height: 100%;
     z-index: 2;
}
 div.react-select__menu, div.dropdown-menu {
     background-color: var(--card-color);
}
 * {
     scrollbar-color: hsla(0, 0%, 100%, .2) transparent;
}
 .bg-dark {
     background-color: var(--nav-color)!important;
}
 .card {
     background-color: #30404d;
     border-radius: 3px;
     box-shadow: 0 0 0 1px rgba(16, 22, 26, .4), 0 0 0 rgba(16, 22, 26, 0), 0 0 0 rgba(16, 22, 26, 0);
     padding: 20px;
     background-color: var(--card-color);
}
 .text-input, .text-input:focus, .text-input[readonly], .text-input:disabled {
     background-color: var(--card-color);
}
 #scrubber-forward {
     background-color: transparent;
     border: 1px solid #555;
}
 .scrubber-button {
     background-color: transparent;
     border: 1px solid #555;
}
 .bg-secondary {
     background-color: var(--card-color) !important;
}
 .text-white {
     color: #eee !important;
}
 .border-secondary {
     border-color: #2f3335 !important;
}
 .btn-secondary.filter-item.col-1.d-none.d-sm-inline.form-control {
     background-color: rgba(0, 0, 0, .15);
}
 .btn-secondary {
     color: #eee;
     background-color: rgba(0, 0, 0, .15);
     border-color: var(--tag-color);
}
 .pagination .btn:last-child {
     border-right: 1px solid var(--tag-color);
}
 .pagination .btn:first-child {
     border-left: 1px solid var(--tag-color);
}
 a {
     color: hsla(0, 0%, 100%, .45);
}
 .btn.active {
     background-color: #2f3335;
     color: #f5f8fa;
}
 minimal.w-100.active.btn.btn-primary {
     background-color: #2f3335;
     color: #f5f8fa;
}
 .btn-primary {
     color: #fff;
     background-color: #cc7b19;
     border-color: #cc7b19;
     font-weight: bold;
}
 .btn-primary:hover {
     color: #fff;
     background-color: #e59029;
     border-color: #e59029 font-weight: bold;
}
 .nav-tabs .nav-link.active {
     color: #eee;
}
 .nav-tabs .nav-link.active:hover {
     border-bottom-color: #eee;
     outline: 0;
}
 .nav-tabs .nav-link {
     color: hsla(0,0%,100%,.65);
}
 .tag-item {
     background-color: var(--tag-color);
     color: #fff;
}
 .input-control, .input-control:focus {
     background-color: rgba(16, 22, 26, .3);
}
 #performer-page .image-container .performer {
     background-color: rgba(0, 0, 0, .45);
     box-shadow: 0 0 2px rgba(0, 0, 0, .35);
}
 .btn-primary:not(:disabled):not(.disabled).active, .btn-primary:not(:disabled):not(.disabled):active, .show>.btn-primary.dropdown-toggle {
     color: #fff;
     border-color: #eee;
}
 .nav-pills .nav-link.active, .nav-pills .show>.nav-link {
     background-color: var(--nav-color);
}
 .btn-primary.focus, .btn-primary:focus, .btn-primary:not(:disabled):not(.disabled).active:focus, .btn-primary:not(:disabled):not(.disabled):active:focus, .show>.btn-primary.dropdown-toggle:focus {
     box-shadow: none;
}
 .btn-primary:not(:disabled):not(.disabled).active, .btn-primary:not(:disabled):not(.disabled):active, .show>.btn-primary.dropdown-toggle {
     color: #fff;
     background-color: #2f3335;
     border-color: #eee;
}
 input[type="range"]::-moz-range-track {
     background: hsla(0, 0%, 100%, .25);
}
 input[type="range"]::-moz-range-thumb {
     background: #bcbcbc;
}
 div.react-select__control {
     background-color: hsla(0, 0%, 39.2%, .4);
     color: #182026;
     border-color: var(--card-color);
     cursor: pointer;
}
 .scene-wall-item-text-container {
     background: radial-gradient(farthest-corner at 50% 50%, rgba(50, 50, 50, .5) 50%, #323232 100%);
     color: #eee;
}
 .filter-container, .operation-container {
     background-color: rgba(0, 0, 0, .15);
     box-shadow: none;
     margin-top: -10px;
     padding: 10px;
}
 .container-fluid, .container-lg, .container-md, .container-sm, .container-xl {
     width: 100%;
     margin-right: 0px;
     margin-left: 0px;
}
 .btn-link {
     font-weight: 500;
     color: #eee;
     text-decoration: none;
}
 button.minimal.brand-link.d-none.d-md-inline-block.btn.btn-primary {
     text-transform: uppercase;
     font-weight: bold;
}
 a:hover {
     color: hsla(0, 0%, 100%, .7);
}
 option {
     background-color: var(--nav-color);
}
 .folder-list .btn-link {
     color: #2c2e30;
}
 #performer-scraper-popover {
     z-index: 10;
}
 .filter-container, .operation-container {
     background-color: transparent;
}
 .search-item {
     background-color: var(--card-color);
}
 .selected-result {
     background-color: var(--card-color);
}
 .selected-result:hover {
     background-color: var(--card-color);
}
 .performer-select-active .react-select__control, .studio-select-active .react-select__control {
     background-color: hsla(0, 0%, 39.2%, .4);
}
 #scene-edit-details .edit-buttons-container {
     margin: 0px;
     background: var(--body-color);
}
 #tasks-panel .tasks-panel-queue {
     background: var(--body-color);
}
 .job-table.card {
     background-color: var(--card-color);
}
 .modal-header, .modal-body, .modal-footer {
     background-color: #2d3744;
     background-repeat: no-repeat;
     background-size: cover;
     background-attachment: fixed;
    /* background-position: center;
     */
}
 .folder-list .btn-link {
     color: #fff;
}
 .modal-header, .modal-body, .modal-footer {
     background-color: #30404d;
     color: #f5f8fa;
     background-repeat: no-repeat;
     background-size: cover;
     background-attachment: fixed;
     background-position: center;
}
 @media (max-width: 575.98px) and (orientation: portrait) {
     .scene-card-preview-image {
         height: calc(100vw * (9 / 16));
    }
     .gallery-tabs .mr-auto.nav.nav-tabs {
         display: grid;
         grid-auto-flow: column;
         text-align: center;
         left: 0;
         right: 0;
         position: fixed;
    }
     .VideoPlayer.portrait .video-js {
         height: 56.25vw;
    }
     .gallery-container .tab-content {
         top: 3rem;
         position: fixed;
         height: calc(100vh - 6.5rem);
    }
     .gallery-tabs {
         display: none;
    }
     .btn-toolbar {
         padding-top: 1rem;
    }
     body {
         padding: 0rem 0 5rem;
    }
     .scene-tabs .mr-auto.nav.nav-tabs {
         background-color: #121212;
         display: grid;
         grid-auto-flow: column;
         height: 3rem;
         left: 0;
         margin: 0;
         margin-bottom: 0;
         max-height: 3rem;
         padding-bottom: 2.2rem;
         padding-top: 0.1rem;
         position: fixed;
         right: 0;
         text-align: center;
         top: calc(100vw * (9 / 16));
         white-space: nowrap;
         z-index: 20;
    }
     .scene-tabs.order-xl-first.order-last {
         height: calc(100vh - (100vw * (9 / 16) + 8.5rem));
         top: calc((100vw * (9 / 16)) + 5rem);
         position: fixed;
    }
     .tab-content {
         overflow-y: auto;
         overflow-x: hidden;
    }
     .studio-card {
         width: 100%;
         height: 294px;
    }
     .movie-card {
         width: 45%;
    }
     .performer-card-image {
         height: 19rem;
    }
     .performer-card {
         width: 14rem;
         height: 27.5rem;
    }
     .scene-performers .performer-card-image {
         height: 19rem;
    }
     .scene-performers .performer-card {
         width: 14rem;
         height: 27.5rem;
    }
     .movie-card .TruncatedText {
         display: none;
    }
     .nav-tabs .nav-link.active:hover {
         outline: 0;
         border-bottom: 2px solid 
    }
     #performer-details-tab-edit{
         display: none;
    }
     #performer-details-tab-operations{
         display: none;
    }
     .scene-tabs .ml-auto.btn-group {
         position: fixed;
         right: 1rem;
         top: calc((100vw * (9 / 16)) + 2.7rem);
    }
     .stats-element {
         flex-grow: 1;
         margin: auto 0rem;
    }
     .stats {
         margin-left: 0px;
    }
     .top-nav {
         bottom: 0;
         top: auto;
    }
     div[data-rb-event-key="/images"] {
         display: none;
    }
     div[data-rb-event-key="/scenes/markers"] {
         display: none;
    }
     .row.justify-content-center.scene-performers {
         max-height: 450px;
         display: flex;
         flex-direction: column;
         overflow: auto;
         border-top: solid 2px #2d3035;
         border-bottom: solid 2px #2d3035;
         padding-top: .5rem;
         padding-bottom: .5rem;
    }
     .scene-tabs {
         max-height: 100%;
    }
}
 dd {
     word-break: break-word;
}
 .btn-secondary {
     color: hsla(0,0%,100%,.65);
}
 .btn-secondary:hover {
     color: white;
     z-index: 0;
     border-color: var(--nav-color);
     background-color: rgba(0, 0, 0, .15);
}
 .btn-secondary:not(:disabled):not(.disabled):active, .btn-secondary:not(:disabled):not(.disabled).active, .show>.btn-secondary.dropdown-toggle {
     background-color: rgba(0, 0, 0, .35);
}
 .btn-secondary:focus, .btn-secondary.focus {
     background-color: rgba(0, 0, 0, .35);
}
 .scrubber-wrapper {
     background-color: rgba(0, 0, 0, .3);
     border-style: ridge;
     border-color: #555555;
}
 a.minimal:hover:not(:disabled), button.minimal:hover:not(:disabled) {
     background: none;
     color: white;
}
 .btn-primary:not(:disabled):not(.disabled).active, .btn-primary:not(:disabled):not(.disabled):active, .show>.btn-primary.dropdown-toggle {
     color: var(--plex-yelow);
     border-bottom: solid;
     background: none;
}
 a.minimal, button.minimal {
     color: hsla(0,0%,100%,.65);
}
 .nav-pills .nav-link.active, .nav-pills .show>.nav-link {
     background: none;
     border-left: solid;
     color: var(--plex-yelow);
}
 .nav-link {
     color: hsla(0,0%,100%,.65);
}
 .nav-link:hover, .nav-link:focus {
     color: white;
     background-color: hsla(0,0%,100%,.08);
}
 .navbar-dark .navbar-nav .nav-link:hover, .navbar-dark .navbar-nav .nav-link:focus {
     background-color: transparent;
}
 .btn-secondary:not(:disabled):not(.disabled):active, .btn-secondary:not(:disabled):not(.disabled).active, .show>.btn-secondary.dropdown-toggle {
     background: none;
     color: var(--plex-yelow);
     border-bottom: solid;
}
 .nav-tabs .nav-link.active {
     color: var(--plex-yelow);
     background: none;
}
 .nav-tabs .nav-link:hover {
     border-bottom: none;
}
 .custom-control-input:checked~.custom-control-label:before {
     color: #fff;
     border-color: var(--plex-yelow);
     background-color: var(--plex-yelow);
}
 .custom-switch .custom-control-input:disabled:checked~.custom-control-label:before {
     background-color: var(--plex-yelow);
}
 .btn-primary.disabled, .btn-primary:disabled {
     color: #fff;
     background-color: #e59029;
     border-color: #e59029;
     font-weight: bold;
}
 .btn-primary:focus, .btn-primary.focus {
     background-color: #cc7b19;
     border-color: #cc7b19;
     font-weight: bold;
}
 .btn-danger {
     color: hsla(0,0%,100%,.75);
     background-color: #b32;
     border-color: #b32;
     font-weight: bold;
}
 .btn-danger:hover {
     color: white;
     background-color: #b32;
     border-color: #b32;
}
 .brand-link {
     background-color: var(--nav-color)!important;
}
 .hover-popover-content {
     max-width: 32rem;
     text-align: center;
     background: var(--nav-color);
}
 .progress-bar {
     background-color: var(--plex-yelow);
}
 .modal-header, .modal-body, .modal-footer {
     background-color: var(--body-color);
}
 .btn-secondary.disabled, .btn-secondary:disabled {
     background-color: var(--card-color);
     border-color: var(--card-color);
     border-left: none!important;
     border-right: none!important;
}
 #queue-viewer .current {
     background-color: var(--card-color);
}
 .tab-content .card-popovers .btn {
     padding-left: .4rem;
     padding-right: .4rem;
}
/* .gallery-tabs, .scene-tabs, .scene-player-container {
     background-color: var(--nav-color);
}
 */
 .react-select__menu-portal {
     z-index: 2;
}
 .video-js .vjs-play-progress {
     background-color: #e5a00d;
}
```