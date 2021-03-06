# Mapache free theme for [Ghost](https://github.com/tryghost/ghost/)

[![Ghost version](https://img.shields.io/badge/Ghost-3.x-brightgreen.svg)](https://github.com/TryGhost/Ghost)
[![Donate](https://img.shields.io/badge/donate-paypal-blue.svg)](https://www.paypal.me/godofredoninja)

> Minimalist and Elegant theme.

Hi. I created this theme for ghost especially for you.
It is available for free so you can use on your site. If you have any suggestions to improve the theme,  you can send me a tweet [@GodoFredoNinja](https://goo.gl/y3aivK)

## If you have a :heart: heart and value my work. :pray: Please, help me with a small donation [Here](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=4H53Q4RTPSFQW&source=url) or [PayPal](https://www.paypal.me/godofredoninja). It'll help motivate me to update the theme with many improvements

[![donate](./donate.gif)](https://www.paypal.me/godofredoninja)

:arrow_right: If you still don't have a **Hosting for your Ghost**. Use [Digital Ocean](https://m.do.co/c/710a27a3b3de) using my [referral link]((https://m.do.co/c/710a27a3b3de)) and you will get free a **$100 in credit over 60 days** to use in [Digital Ocean]((https://m.do.co/c/710a27a3b3de)). This way you will also be helping me.

![mapache theme for ghost](./screenshot.png)

## Featured

- Support for different [languages](http://themes.ghost.org/docs/i18n#section-how-to-add-any-language) (en - es - de - ko - fr - pt)
- Light Mode / Dark Mode
- First navigation menu for the header of the page
- Second navigation menu for the footer of the page
- 404 error page
- Pagination Infinite Scroll
- Instagram Feed in footer of Post
- Optional menu in the footer
- [AMP](https://github.com/godofredoninja/Hodor-AMP-Template-for-Ghost) Template (Accelerated Mobile Pages)
- Social Media
- Members / Subscription
- Very fast search engine
- Related Articles (6 articles)
- Different templates for the Home Page
- Different templates for publishing posts
- Page for (About Us - Podcast - Tag - Authors - Newsletter)
- 5 lates articles in the sidebar (post)
- Tag Cloud in the sidebar
- Previous and next articles buttons
- Support for comments (Disqus)
- Support for counter comments (Disqus)
- Buttons to share the article (Facebook - Twitter - Reddit - Linkedin - Pinterest)
- Beautiful gallery viewer
- Sticky content in the sidebar
- YouTube, Vimeo, kickstarter, dailymotion => Responsive
- Lazy image loading for better performance only in backgrounds
- Code syntax [Prismjs](http://prismjs.com/index.html#languages-list) Supported all syntax.

## Table of Contents

- [Web Browser Support for Mapache](#web-browser-support-for-mapache)
- [Ghost Settings](#ghost-settings)
- [Mapache Settings](#mapache-settings)
  - [1. Social Media](#1-social-media)
  - [2. Footer Menu](#2-footer-menu)
  - [3. Instagram](#3-instagram)
  - [4. Comments](#4-comments)
  - [5. Search](#5-search)
- [Home](#home-page)
  - [Tech](#home-page)
  - [Personal](#home-page)
  - [Blog](#home-page)
  - [Travel](#home-page)
  - [Travel with Featured Article](#home-page)
  - [Fashion Concept](#home-page)
- [Post](#post-format)
  - [Default Post](##post-format)
  - [Post Full Header](##post-format)
  - [Post Image](##post-format)
  - [Post Image Single](##post-format)
  - [Post Video](##post-format)
  - [Post Single](##post-format)
- [Page](#page)
  - [About Us](#about-us-page)
  - [Contact](#contact-page)
  - [Newsletter](#newsletter-page)
- [Archive](#authors-page)
  - [Authors](#authors-page)
  - [Tags](#tags-page)
  - [Podcast](#podcast-page)
- [Category](#category)
  - [Default Category](#category---defautl)
  - [Category with header](#category-with-header)
- [Members / Subscription](#members--subscription)
- [AMP](#amp)
- [Theme Translation](#theme-translation)
- [Change Theme Color](#change-theme-color)
- [PrismJS code syntax](#prismjs-code-syntax)

## Web Browser Support for mapache

mapache supports the following web [browsers](https://caniuse.com/#search=CSS%20Variables)

## Ghost Settings

Enable the following checkbox on the Labs page in the Ghost admin panel.

![ghost labs](./documentation/ghost-settings.jpg)

## Mapache Settings

> You don't have to add all the Mapache configurations. only the ones you need

### 1. Social Media

> Facebook and Twitter is not necessary because I use them from the ghost settings

Add the Social Links only for the services you want to appear in the header section of your website. Pay attention as enabling too many services will cause menu problems.

:arrow_right: `Dashboard -> Code injection -> Site Footer`

```html
<script>
var followSocialMedia = {
  'youtube': ['YOUR_URL','YOUR_TITLE'],
  'instagram': ['YOUR_URL','YOUR_TITLE'],
  'github': ['YOUR_URL','YOUR_TITLE'],
  'pinterest': ['YOUR_URL','YOUR_TITLE'],
  'linkedin': ['YOUR_URL','YOUR_TITLE'],
  'rss': ['YOUR_URL','YOUR_TITLE'],

  /*
  'snapchat': ['YOUR_URL','YOUR_TITLE'],
  'dribbble': ['YOUR_URL','YOUR_TITLE'],
  'spotify': ['YOUR_URL','YOUR_TITLE'],
  'codepen': ['YOUR_URL','YOUR_TITLE'],
  'behance': ['YOUR_URL','YOUR_TITLE'],
  'flickr': ['YOUR_URL','YOUR_TITLE'],
  'telegram': ['YOUR_URL','YOUR_TITLE'],
  'vimeo': ['YOUR_URL','YOUR_TITLE'],
  'twitch': ['YOUR_URL','YOUR_TITLE'],
  'vk': ['YOUR_URL','YOUR_TITLE'],
  'slack': ['YOUR_URL','YOUR_TITLE'],
  'tumblr': ['YOUR_URL','YOUR_TITLE'],
  'discord': ['YOUR_URL','YOUR_TITLE'],
  */
};
</script>
```

:point_right: For those who are commented it is necessary to add those icons through `SVG`

It is not necessary to add all the icons. Only the icons you need.

:arrow_right: `Dashboard -> Code injection -> Site Footer`

```html
<svg aria-hidden="true" style="position: absolute; width: 0; height: 0; overflow: hidden;" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
    <defs>
        <!-- discord -->
        <symbol id="icon-discord" viewBox="0 0 24 24">
        <title>discord</title>
        <path d="M20.222 0c1.406 0 2.54 1.137 2.607 2.475v21.525l-2.677-2.273-1.47-1.338-1.604-1.398 0.67 2.205h-14.038c-1.402 0-2.54-1.065-2.54-2.476v-16.24c0-1.338 1.14-2.477 2.545-2.477l16.507-0.003zM14.104 5.683h-0.030l-0.202 0.2c2.073 0.6 3.076 1.537 3.076 1.537-1.336-0.668-2.54-1.002-3.744-1.137-0.87-0.135-1.74-0.064-2.475 0h-0.2c-0.47 0-1.47 0.2-2.81 0.735-0.467 0.203-0.735 0.336-0.735 0.336s1.002-1.002 3.21-1.537l-0.135-0.135s-1.672-0.064-3.477 1.27c0 0-1.805 3.144-1.805 7.020 0 0 1 1.74 3.743 1.806 0 0 0.4-0.533 0.805-1.002-1.54-0.468-2.14-1.404-2.14-1.404s0.134 0.066 0.335 0.2h0.060c0.030 0 0.044 0.015 0.060 0.030v0.006c0.016 0.016 0.030 0.030 0.060 0.030 0.33 0.136 0.66 0.27 0.93 0.4 0.466 0.202 1.065 0.403 1.8 0.536 0.93 0.135 1.996 0.2 3.21 0 0.6-0.135 1.2-0.267 1.8-0.535 0.39-0.2 0.87-0.4 1.397-0.737 0 0-0.6 0.936-2.205 1.404 0.33 0.466 0.795 1 0.795 1 2.744-0.060 3.81-1.8 3.87-1.726 0-3.87-1.815-7.020-1.815-7.020-1.635-1.214-3.165-1.26-3.435-1.26l0.056-0.020zM14.272 10.096c0.703 0 1.27 0.6 1.27 1.335 0 0.74-0.57 1.34-1.27 1.34s-1.27-0.6-1.27-1.334c0.002-0.74 0.573-1.338 1.27-1.338zM9.729 10.096c0.7 0 1.266 0.6 1.266 1.335 0 0.74-0.57 1.34-1.27 1.34s-1.27-0.6-1.27-1.334c0-0.74 0.57-1.338 1.27-1.338z"></path>
        </symbol>
        <!-- flickr -->
        <symbol id="icon-flickr" viewBox="0 0 21 24">
        <title>flickr</title>
        <path d="M16.714 1.714c2.129 0 3.857 1.728 3.857 3.857v12.857c0 2.129-1.728 3.857-3.857 3.857h-12.857c-2.129 0-3.857-1.728-3.857-3.857v-12.857c0-2.129 1.728-3.857 3.857-3.857h12.857zM9.348 12c0-1.567-1.272-2.839-2.839-2.839s-2.839 1.272-2.839 2.839 1.272 2.839 2.839 2.839 2.839-1.272 2.839-2.839zM16.902 12c0-1.567-1.272-2.839-2.839-2.839s-2.839 1.272-2.839 2.839 1.272 2.839 2.839 2.839 2.839-1.272 2.839-2.839z"></path>
        </symbol>
        <!-- tumblr -->
        <symbol id="icon-tumblr" viewBox="0 0 15 24">
        <title>tumblr</title>
        <path d="M12.643 17.799l1.071 3.174c-0.402 0.603-2.223 1.286-3.857 1.313-4.862 0.080-6.696-3.455-6.696-5.946v-7.286h-2.25v-2.879c3.375-1.219 4.192-4.272 4.379-6.013 0.013-0.107 0.107-0.161 0.161-0.161h3.268v5.679h4.46v3.375h-4.473v6.938c0 0.938 0.348 2.237 2.143 2.196 0.589-0.013 1.379-0.188 1.795-0.388z"></path>
        </symbol>
        <!-- dribbble -->
        <symbol id="icon-dribbble" viewBox="0 0 21 24">
        <title>dribbble</title>
        <path d="M13.714 20.089c-0.134-0.777-0.643-3.455-1.875-6.67-0.013 0-0.040 0.013-0.054 0.013 0 0-5.21 1.821-6.897 5.491-0.080-0.067-0.201-0.147-0.201-0.147 1.527 1.246 3.469 2.009 5.598 2.009 1.219 0 2.371-0.254 3.429-0.696zM11.237 11.96c-0.214-0.496-0.455-0.991-0.71-1.487-4.527 1.353-8.866 1.246-9.013 1.246-0.013 0.094-0.013 0.188-0.013 0.281 0 2.25 0.857 4.313 2.25 5.866v0c2.397-4.272 7.138-5.799 7.138-5.799 0.121-0.040 0.241-0.067 0.348-0.107zM9.804 9.121c-1.527-2.705-3.147-4.902-3.268-5.063-2.451 1.152-4.272 3.415-4.848 6.134 0.228 0 3.897 0.040 8.116-1.071zM18.964 13.393c-0.188-0.054-2.638-0.83-5.478-0.388 1.152 3.174 1.621 5.759 1.714 6.281 1.969-1.326 3.362-3.442 3.763-5.893zM8.183 3.469c-0.013 0-0.013 0-0.027 0.013 0 0 0.013-0.013 0.027-0.013zM16.085 5.411c-1.54-1.366-3.576-2.196-5.799-2.196-0.71 0-1.406 0.094-2.076 0.254 0.134 0.174 1.795 2.357 3.295 5.116 3.308-1.232 4.554-3.134 4.58-3.174zM19.071 11.906c-0.027-2.076-0.763-3.991-1.996-5.491-0.027 0.027-1.433 2.063-4.902 3.482 0.201 0.415 0.402 0.844 0.589 1.272 0.067 0.147 0.121 0.308 0.188 0.455 3.027-0.388 6.013 0.268 6.121 0.281zM20.571 12c0 5.679-4.607 10.286-10.286 10.286s-10.286-4.607-10.286-10.286 4.607-10.286 10.286-10.286 10.286 4.607 10.286 10.286z"></path>
        </symbol>
        <!-- vk -->
        <symbol id="icon-vk" viewBox="0 0 26 24">
        <title>vk</title>
        <path d="M25.674 6.964c0.201 0.549-0.429 1.835-2.009 3.938-2.598 3.455-2.879 3.134-0.737 5.129 2.062 1.915 2.491 2.839 2.558 2.96 0 0 0.857 1.5-0.951 1.513l-3.429 0.054c-0.737 0.147-1.714-0.522-1.714-0.522-1.286-0.884-2.491-3.174-3.429-2.879 0 0-0.964 0.308-0.938 2.371 0.013 0.442-0.201 0.683-0.201 0.683s-0.241 0.254-0.71 0.295h-1.54c-3.388 0.214-6.375-2.906-6.375-2.906s-3.268-3.375-6.134-10.112c-0.188-0.442 0.013-0.656 0.013-0.656s0.201-0.254 0.763-0.254l3.67-0.027c0.348 0.054 0.589 0.241 0.589 0.241s0.214 0.147 0.321 0.429c0.603 1.5 1.379 2.866 1.379 2.866 1.339 2.759 2.25 3.228 2.772 2.946 0 0 0.683-0.415 0.536-3.75-0.054-1.205-0.388-1.754-0.388-1.754-0.308-0.415-0.884-0.536-1.138-0.576-0.201-0.027 0.134-0.509 0.576-0.723 0.656-0.321 1.821-0.335 3.201-0.321 1.085 0.013 1.393 0.080 1.808 0.174 1.272 0.308 0.844 1.487 0.844 4.326 0 0.911-0.174 2.183 0.482 2.598 0.281 0.188 0.978 0.027 2.692-2.893 0 0 0.804-1.393 1.433-3.013 0.107-0.295 0.335-0.415 0.335-0.415s0.214-0.121 0.509-0.080l3.857-0.027c1.165-0.147 1.353 0.388 1.353 0.388z"></path>
        </symbol>
        <!-- slack -->
        <symbol id="icon-slack" viewBox="0 0 22 24">
        <title>slack</title>
        <path d="M20.344 10.393c1.098 0 1.942 0.804 1.942 1.902 0 0.857-0.442 1.46-1.246 1.741l-2.304 0.79 0.75 2.237c0.067 0.201 0.094 0.415 0.094 0.629 0 1.058-0.857 1.942-1.915 1.942-0.844 0-1.594-0.522-1.862-1.326l-0.737-2.21-4.152 1.42 0.737 2.196c0.067 0.201 0.107 0.415 0.107 0.629 0 1.045-0.857 1.942-1.929 1.942-0.844 0-1.58-0.522-1.848-1.326l-0.737-2.183-2.049 0.71c-0.214 0.067-0.442 0.121-0.67 0.121-1.085 0-1.902-0.804-1.902-1.888 0-0.83 0.536-1.58 1.326-1.848l2.089-0.71-1.406-4.192-2.089 0.723c-0.214 0.067-0.429 0.107-0.643 0.107-1.071 0-1.902-0.817-1.902-1.888 0-0.83 0.536-1.58 1.326-1.848l2.103-0.71-0.71-2.129c-0.067-0.201-0.107-0.415-0.107-0.629 0-1.058 0.857-1.942 1.929-1.942 0.844 0 1.58 0.522 1.848 1.326l0.723 2.143 4.152-1.406-0.723-2.143c-0.067-0.201-0.107-0.415-0.107-0.629 0-1.058 0.871-1.942 1.929-1.942 0.844 0 1.594 0.536 1.862 1.326l0.71 2.156 2.17-0.737c0.188-0.054 0.375-0.080 0.576-0.080 1.045 0 1.942 0.777 1.942 1.848 0 0.83-0.643 1.527-1.393 1.781l-2.103 0.723 1.406 4.232 2.196-0.75c0.201-0.067 0.415-0.107 0.616-0.107zM9.71 13.902l4.152-1.406-1.406-4.219-4.152 1.433z"></path>
        </symbol>
        <!-- behance -->
        <symbol id="icon-behance" viewBox="0 0 21 24">
        <title>behance</title>
        <path d="M16.714 1.714c2.129 0 3.857 1.728 3.857 3.857v12.857c0 2.129-1.728 3.857-3.857 3.857h-12.857c-2.129 0-3.857-1.728-3.857-3.857v-12.857c0-2.129 1.728-3.857 3.857-3.857h12.857zM6.683 6.629h-4.969v10.54h5.116c1.915 0 3.71-0.911 3.71-3.054 0-1.326-0.629-2.304-1.915-2.679 0.938-0.455 1.433-1.138 1.433-2.196 0-2.103-1.567-2.612-3.375-2.612zM6.388 10.888h-2.357v-2.464h2.183c0.83 0 1.594 0.228 1.594 1.205 0 0.897-0.589 1.259-1.42 1.259zM6.509 15.375h-2.478v-2.906h2.531c1.018 0 1.661 0.442 1.661 1.513s-0.763 1.393-1.714 1.393zM15.214 15.804c-1.232 0-1.875-0.723-1.875-1.942h5.504c0.013-0.134 0.013-0.268 0.013-0.402 0-2.25-1.326-4.138-3.723-4.138-2.317 0-3.911 1.754-3.911 4.045 0 2.384 1.5 4.004 3.911 4.004 1.835 0 3.013-0.817 3.576-2.558h-1.848c-0.201 0.643-1.018 0.991-1.647 0.991zM15.080 10.902c1.045 0 1.567 0.629 1.661 1.634h-3.402c0.067-1.004 0.737-1.634 1.741-1.634zM12.911 7.339h4.272v1.031h-4.272v-1.031z"></path>
        </symbol>
        <!-- spotify -->
        <symbol id="icon-spotify" viewBox="0 0 21 24">
        <title>spotify</title>
        <path d="M15.094 16.205c0-0.375-0.147-0.522-0.402-0.683-1.728-1.031-3.737-1.54-5.987-1.54-1.313 0-2.571 0.174-3.844 0.455-0.308 0.067-0.563 0.268-0.563 0.696 0 0.335 0.254 0.656 0.656 0.656 0.121 0 0.335-0.067 0.496-0.107 1.045-0.214 2.143-0.362 3.254-0.362 1.969 0 3.83 0.482 5.317 1.379 0.161 0.094 0.268 0.147 0.442 0.147 0.335 0 0.629-0.268 0.629-0.643zM16.379 13.326c0-0.362-0.134-0.616-0.469-0.817-2.049-1.219-4.647-1.888-7.339-1.888-1.728 0-2.906 0.241-4.058 0.563-0.429 0.121-0.643 0.415-0.643 0.857s0.362 0.804 0.804 0.804c0.188 0 0.295-0.054 0.496-0.107 0.938-0.254 2.063-0.442 3.362-0.442 2.545 0 4.862 0.67 6.536 1.661 0.147 0.080 0.295 0.174 0.509 0.174 0.455 0 0.804-0.362 0.804-0.804zM17.826 10.004c0-0.496-0.214-0.75-0.536-0.938-2.317-1.353-5.491-1.982-8.518-1.982-1.781 0-3.415 0.201-4.875 0.629-0.375 0.107-0.723 0.429-0.723 0.991 0 0.549 0.415 0.978 0.964 0.978 0.201 0 0.388-0.067 0.536-0.107 1.299-0.362 2.705-0.496 4.112-0.496 2.786 0 5.679 0.616 7.54 1.728 0.188 0.107 0.321 0.161 0.536 0.161 0.509 0 0.964-0.402 0.964-0.964zM20.571 12c0 5.679-4.607 10.286-10.286 10.286s-10.286-4.607-10.286-10.286 4.607-10.286 10.286-10.286 10.286 4.607 10.286 10.286z"></path>
        </symbol>
        <!-- codepen -->
        <symbol id="icon-codepen" viewBox="0 0 24 24">
        <title>codepen</title>
        <path d="M2.893 15.656l8.076 5.384v-4.808l-4.473-2.987zM2.063 13.728l2.585-1.728-2.585-1.728v3.455zM13.031 21.040l8.076-5.384-3.603-2.411-4.473 2.987v4.808zM12 14.438l3.643-2.438-3.643-2.438-3.643 2.438zM6.496 10.754l4.473-2.987v-4.808l-8.076 5.384zM19.353 12l2.585 1.728v-3.455zM17.504 10.754l3.603-2.411-8.076-5.384v4.808zM24 8.344v7.313c0 0.335-0.174 0.67-0.455 0.857l-10.969 7.313c-0.174 0.107-0.375 0.174-0.576 0.174s-0.402-0.067-0.576-0.174l-10.969-7.313c-0.281-0.188-0.455-0.522-0.455-0.857v-7.313c0-0.335 0.174-0.67 0.455-0.857l10.969-7.313c0.174-0.107 0.375-0.174 0.576-0.174s0.402 0.067 0.576 0.174l10.969 7.313c0.281 0.188 0.455 0.522 0.455 0.857z"></path>
        </symbol>
        <!-- twitch -->
        <symbol id="icon-twitch" viewBox="0 0 24 24">
        <title>twitch</title>
        <path d="M12 5.813v5.813h-1.942v-5.813h1.942zM17.33 5.813v5.813h-1.942v-5.813h1.942zM17.33 15.991l3.388-3.402v-10.647h-15.991v14.049h4.366v2.906l2.906-2.906h5.33zM22.661 0v13.567l-5.813 5.813h-4.366l-2.906 2.906h-2.906v-2.906h-5.33v-15.509l1.46-3.871h19.862z"></path>
        </symbol>
        <!-- vimeo -->
        <symbol id="icon-vimeo" viewBox="0 0 24 24">
        <title>vimeo</title>
        <path d="M22.888 6.938c-0.094 2.116-1.58 5.022-4.446 8.719-2.973 3.844-5.464 5.772-7.527 5.772-1.272 0-2.344-1.179-3.214-3.522-0.589-2.143-1.179-4.299-1.768-6.455-0.643-2.344-1.353-3.509-2.103-3.509-0.161 0-0.723 0.335-1.701 1.018l-1.031-1.313c1.071-0.951 2.129-1.915 3.188-2.839 1.42-1.259 2.504-1.888 3.228-1.955 1.701-0.161 2.732 0.991 3.134 3.469 0.415 2.679 0.723 4.353 0.884 4.996 0.496 2.223 1.018 3.335 1.607 3.335 0.455 0 1.138-0.71 2.063-2.156 0.911-1.446 1.393-2.545 1.46-3.295 0.121-1.246-0.362-1.862-1.46-1.862-0.522 0-1.058 0.121-1.621 0.348 1.071-3.509 3.121-5.21 6.147-5.116 2.237 0.067 3.295 1.527 3.161 4.366z"></path>
        </symbol>
        <!-- snapchat -->
        <symbol id="icon-snapchat" viewBox="0 0 22 24">
        <title>snapchat</title>
        <path d="M11.357 1.714c2.411-0.027 4.406 1.326 5.411 3.496 0.308 0.656 0.362 1.674 0.362 2.397 0 0.857-0.067 1.701-0.121 2.558 0.107 0.054 0.254 0.094 0.375 0.094 0.482 0 0.884-0.362 1.366-0.362 0.455 0 1.112 0.321 1.112 0.857 0 1.286-2.692 1.045-2.692 2.17 0 0.201 0.080 0.388 0.161 0.576 0.643 1.406 1.862 2.759 3.308 3.362 0.348 0.147 0.696 0.228 1.071 0.308 0.241 0.054 0.375 0.228 0.375 0.469 0 0.911-2.317 1.286-2.933 1.379-0.268 0.415-0.067 1.393-0.777 1.393-0.549 0-1.098-0.174-1.688-0.174-0.281 0-0.563 0.013-0.83 0.067-1.594 0.268-2.129 1.982-4.741 1.982-2.518 0-3.121-1.714-4.674-1.982-0.281-0.054-0.563-0.067-0.844-0.067-0.603 0-1.179 0.201-1.661 0.201-0.75 0-0.522-0.991-0.804-1.42-0.616-0.094-2.933-0.469-2.933-1.379 0-0.241 0.134-0.415 0.375-0.469 0.375-0.080 0.723-0.161 1.071-0.308 1.433-0.589 2.679-1.955 3.308-3.362 0.080-0.188 0.161-0.375 0.161-0.576 0-1.125-2.705-0.911-2.705-2.156 0-0.522 0.616-0.857 1.085-0.857 0.415 0 0.83 0.348 1.353 0.348 0.147 0 0.295-0.027 0.429-0.094-0.054-0.844-0.121-1.688-0.121-2.545 0-0.723 0.054-1.754 0.362-2.411 1.179-2.545 3.174-3.469 5.839-3.496z"></path>
        </symbol>
        <!-- telegram -->
        <symbol id="icon-telegram" viewBox="0 0 24 24">
        <title>telegram</title>
        <path d="M15.924 17.504l1.969-9.281c0.174-0.817-0.295-1.138-0.83-0.938l-11.571 4.46c-0.79 0.308-0.777 0.75-0.134 0.951l2.96 0.924 6.871-4.326c0.321-0.214 0.616-0.094 0.375 0.121l-5.558 5.022-0.214 3.054c0.308 0 0.442-0.134 0.603-0.295l1.446-1.393 3 2.21c0.549 0.308 0.938 0.147 1.085-0.509zM24 12c0 6.629-5.371 12-12 12s-12-5.371-12-12 5.371-12 12-12 12 5.371 12 12z"></path>
        </symbol>
    </defs>
</svg>
```

### 2. Footer Menu

You can add an additional menu bar at the footer of the page

:arrow_right: `Dashboard -> Design -> Secondary Navigation`

### 3. Instagram

I get the last 10 images then show 6 randomly It will only be shown in the footer of the Post

First, you will need to get your account `userName` and `userId` and `accessToken` from the following URLs:

- User ID: [codeofaninja.com/tools/find-instagram-user-id](https://codeofaninja.com/tools/find-instagram-user-id)
- Access Token: [instagram.pixelunion.net](http://instagram.pixelunion.net/)

:arrow_right: `Dashboard -> Code injection -> Site Footer`

```html
<script>
var instagramFeed  = {
  token: 'Token_app_instagram',
  userId: 'User_ID',
  userName: 'User_Name',
};
</script>
```

### 4. Comments

Mapache supports Disqus comments as well as comment counting

??? First, you will need to get your account `disqusShortName`

:arrow_right: `Dashboard -> Code injection -> Site Footer`

```html
<script>
var disqusShortName = 'YOUR_DISQUS_SHORTCUT_HERE';
</script>
```

### 5. Search

> The default search engine will only search the titles of the post

**Setup a Custom integration**

1. Go in your Ghost's `dashboard -> Integrations -> Add custom integration`
2. Set a name: `GodoFredo Themes Search`
3. Get the Content API Key and replace the demo key with this one
4. Get the admin domain. This will be different in some cases

![ghost api](./documentation/ghost-api.jpg)

:arrow_right: `Dashboard -> Code injection -> Site Footer`

```html
<script>
  var searchSettings = {
    key: 'ADD_YOUR_API_KEY',
    url: 'https://demo.ghost.io',
  };
</script>
```

OR - Adding parameters to the search

```html
<script>
var searchSettings = {
  key: 'ADD_YOUR_API_KEY',
  url: 'https://demo.ghost.io',
  /* This is optional */
  options: {
    keys: [
        'title',
    ],
    limit: 10,
  },
  /* This is optional to perform filtering of the ghost api */
  api: {
    resource: 'posts',
    parameters: {
      limit: 'all',
      fields: ['title', 'slug'],
      filter: '',
      include: '',
      order: '',
      formats: '',
    },
  },
}
</script>
```

The search engine that includes Mapache is very powerful, supports almost all languages and you can customize to your liking.

Read more about the search engine [Read More](https://github.com/HauntedThemes/ghost-search)

### 6. Twitter widget in the sidebar

```html
<script>
var twitterFeed = 'YOUR_TWITTER_USER_NAME';
</script>
```

## Home Page

> Mapache - come with 6 Home page with different layout options

- First back up your `routes` in your ghost settings  `Dashboard -> Labs -> Routes -> Download current routes.yml`
- Re-download the Route and edit `routes.yml` line `collections -> template`
  - `index` ??? **Personal**
  - `godo-home-blog` ??? **Blog**
  - `godo-home-travel` ??? **Travel**
  - `godo-home-travel-featured` ??? **Travel With Featured Post**
  - `godo-home-fashion-concept` ??? **Fashion Concept**

:loudspeaker: If you plan to use (Personal, Blog, Travel, Fashion) for your home page, Rename or delete the file `home.hbs`

**Personal** -  Edit `package.json` and change `"posts_per_page": 10`

**Blog** - Edit `package.json` and change `"posts_per_page": 10`

**Fashion** - Edit `package.json` and change `"posts_per_page": 12`

```yaml
collections:
  /:
    permalink: /{slug}/
    template:
      # - godo-home-blog
      # - godo-home-travel
      # - godo-home-travel-featured
      # - godo-home-fashion-concept
      - index
```

![mapache demo 01](./documentation/mapache-home-01.jpg)

![mapache demo 02](./documentation/mapache-home-02.jpg)

## Post Format

 > Mapache has different templates for post formats. I will mention some of them.

 ![Post Format](./documentation/mapache-post-format.jpg)

 1. **Post Full Header** ??? It will have the full title of the post and will include the sidebar.

 2. **Post Image** ??? This template will have a very large featured image and the header background will also be transparent and include the sidebar.

 3. **Post Image Single** ??? It's similar to post image. The difference is that you won't have a sidebar.

 4. **Post Single** ??? Includes the featured image at the top but does not include the sidebar

 5. **Post Not Image** ??? The sidebar doesn't have the featured image either.

 6. **Post Video** ??? The first video found will move to the top of the page.
    - vimeo
    - Dailymotion
    - Youtube
    - Twitch
    - kickstarter

> Add video where convenient. When you change the theme you will not have problems and not have Problem in your AMP Template

![Post Format 01](./documentation/mapache-post-format-01.jpg)

![Post Format 02](./documentation/mapache-post-format-02.jpg)

## Page

### About Us Page

> Mapache has a beautifull page for - about us

- Create a new page
- Choose your favorite url and title
- Template dropdown -> Select `Page About Us`
- You have to add a section of `html` and add the rows and columns. you can guide yourself with the capture of the image
- Publish the page
- To add the page to the navigation

```html
<section class="row">
<div class="col s12 l6">
<!-- Content here -->

</div>
<div class="col s12 l6">
<!-- The image here -->


</div>
</section> <!-- close Row -->
<section class="row">
<div class="col s12 l6 u-hide-before-lg">
<!-- Content here -->

</div>
<div class="col s12 l6">
<!-- The image here -->

</div>
</section> <!-- close Row -->
```

![About us](./documentation/mapache-about-us.jpg)

### Contact Page

- Create a new page
- Choose your favorite url and title
- Template dropdown -> Select `Page Contact`
- Publish the page
- To add the page to the navigation

:arrow_right: I am using [FORMSPREE](https://formspree.io/) for sending emails. Please replace with your email. I recommend having an email dedicated especially to FORMSPREE.

```html
<div class="u-fontSize20 u-maxWidth740 u-marginAuto u-marginBottom40 u-textAlignCenter">
  We???re here for you! Please contact us using the form below.
</div>

<!-- FORMSPREE replace with your email -->
<form action="https://formspree.io/your@email.com" class="contact-form u-marginBottom40 u-marginAuto" method="POST">
  <input name="name" type="text" class="u-marginBottom30" placeholder="Your Name" required>
  <input name="email" type="email" class="u-marginBottom30" placeholder="Your Email" required>
  <textarea name="message" class="u-marginBottom40" placeholder="Type Message" required></textarea>
  <button type="submit" class="button button--large button--dark">Send Message</button>
</form>
```

:arrow_right: PHONE - ADDRESS - EMAIL

```html
<div class="pae u-textAlignCenter u-maxWidth1000 u-marginAuto">
  <div class="row">
    <div class="col s12 m4 u-marginBottom30">
      <div class="pae-icon">
        <svg viewBox="0 0 24 24" width="64" height="64" stroke="currentColor" stroke-width="1" fill="none" stroke-linecap="round" stroke-linejoin="round"><rect x="5" y="2" width="14" height="20" rx="2" ry="2"></rect><line x1="12" y1="18" x2="12" y2="18"></line></svg>
      </div>
      <h4 class="pae-title">PHONE</h4>
      <div class="pae-des u-fontSizeBase">
        <p>+51 987 659 249</p>
        <p>+51 01 424 0827</p>
      </div>
    </div>

    <div class="col s12 m4 u-marginBottom30">
      <div class="pae-icon">
        <svg viewBox="0 0 24 24" width="64" height="64" stroke="currentColor" stroke-width="1" fill="none" stroke-linecap="round" stroke-linejoin="round"><path d="M21 10c0 7-9 13-9 13s-9-6-9-13a9 9 0 0 1 18 0z"></path><circle cx="12" cy="10" r="3"></circle></svg>
      </div>
      <h4 class="pae-title">ADDRESS</h4>
      <div class="pae-des u-fontSizeBase">
        <p>Parque de la Reserva, Jr. Madre de Dios, Cercado de Lima, Per??</p>
      </div>
    </div>

    <div class="col s12 m4 u-marginBottom30">
      <div class="pae-icon">
        <svg viewBox="0 0 24 24" width="64" height="64" stroke="currentColor" stroke-width="1" fill="none" stroke-linecap="round" stroke-linejoin="round"><path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"></path><polyline points="22,6 12,13 2,6"></polyline></svg>
      </div>
      <h4 class="pae-title">EMAIL</h4>
      <div class="pae-des u-fontSizeBase">
        <p>hello@godofredo.ninja</p>
        <p>test@godofredo.ninja</p>
      </div>
    </div>
  </div>
</div>
```

:arrow_right: Google Maps

```html
<div class="contact-maps u-textAlignCenter">
  <div class="video-responsive">
    <!-- ADD_YOUR_IFRAME_GOOGLE_MAPS -->
  </div>
</div>
```

![contact](./documentation/mapache-contact.jpg)

### Newsletter Page

- Create a new page
- Choose your favorite url and title
- Template dropdown -> Select `Archive Newsletter`
- Publish the page
- To add the page to the navigation

:arrow_right: I am using [Mailchimp](https://mailchimp.com/) for Newsletter. Please replace the form action url

```html
<div class="godo-ne">
  <!-- Replace => Action -->
  <form id="godo-form" class="godo-ne-form" action="YOUR_URL_OF_LIST_Mailchimp" method="get">
      <label for="fieldEmail">Email Address</label>
      <div class="godo-ne-form-group">
        <input id="fieldEmail" class="godo-ne-input" name="EMAIL" type="email" placeholder="yourname@example.com" required="">
        <button class="godo-ne-button button button--dark button--large" type="submit">Subscribe</button>
      </div>
      <small>No marketing campaigns. No jibber jabber. Unsubscribe anytime.</small>
  </form>
  <div class="godo-ne-success u-hide">
    <h3>?????? Nice! Please check your email</h3>
    <p>Click on the link in your inbox to confirm your subscription</p>
  </div>
</div>
```

:arrow_right: Testimonies Copy the code and paste into an HTML section in Ghost

```html
<div class="godo-n-q">

  <div class="godo-n-q-i">
    <img src="http://localhost:2368/assets/images/avatar.png" alt="Hello">
    <h3>Tim Cook</h3>
    <div class="godo-n-q-d">CEO, Apple</div>
    <blockquote>"This is a pretty fantastic newsletter tbh, I definitely recommend it"</blockquote>
  </div>

  <div class="godo-n-q-i u-hide-before-md">
    <img src="http://localhost:2368/assets/images/avatar.png" alt="Hello">
    <h3>Satya Nadella</h3>
    <div class="godo-n-q-d">CEO, Microsoft</div>
    <blockquote>"Finally, this newsletter is something we can really agree on"</blockquote>
  </div>

  <div class="godo-n-q-i u-hide-before-md">
    <img src="http://localhost:2368/assets/images/avatar.png" alt="Hello">
    <h3>John O'Nolan</h3>
    <div class="godo-n-q-d">CEO, Ghost</div>
    <blockquote>"I should really get around to organising some quotes one of these days"</blockquote>
  </div>

  </div>
```

![newsletter](./documentation/mapache-newsletter.jpg)

### Authors Page

- Create a new page
- Choose your favorite url and title
- Template dropdown -> Select `Archive Author`
- Publish the page
- To add the page to the navigation

![Archive Authors](./documentation/mapache-author.jpg)

### Tags Page

> A page will be displayed with all tags sorted from highest to lowest number of articles.

- Create a new page
- Choose your favorite url and title
- Template dropdown -> Select `Archive Tags`
- Publish the page
- To add the page to the navigation

![Archive Tags](./documentation/mapache-tags.jpg)

### Podcast Page

- Create a new page
- Choose your favorite title
- Use the url `podcast`
- In your articles use the internal tags `#podcast`
- First back up your routes in your ghost settings `Labs -> Routes -> Download current routes.yml`
- Re-download the Route and edit `routes.yml` line `routes`

```yaml
routes:
  /podcast/:
    controller: channel
    filter: tag:[hash-podcast]
    data:
      post: page.podcast
    limit: 10
    template: godo-podcast
```

- In an `HTML` block in your ghost editor add this code for your content.

```html
<p class="spc-h-e">The Podcast</p>

<p class="spc-des">Updates and behind the scenes stories about the world of Ghost. Hosted by Ghost founders <em>John O'Nolan</em> &amp; <em>Hannah Wolfe</em>.</p>

<div class="spc-buttons buttonSet">

    <a class="button" href="https://itunes.apple.com/">
    <img src="http://localhost:2368/assets/images/icon-itunes.png" alt="iTunes Logo" rel="presentation"/>
    <span>iTunes</span>
  </a>

  <a class="button" href="https://www.pocketcasts.com/">
    <img src="http://localhost:2368/assets/images/icon-pocketcasts.png" alt="Pocket Casts Logo" rel="presentation"/>
    <span>Pocket Casts</span>
  </a>

  <a class="button" href="https://anchor.fm/">
    <img src="http://localhost:2368/assets/images/icon-rss.png" style="height:15px" alt="RSS Icon" rel="presentation"/>
    <span>RSS</span>
  </a>

</div>
```

![podcast Page](./documentation/mapache-podcast.jpg)

### Category

To create new categories we are going to have to use the [Ghost Routes](https://ghost.org/docs/api/v3/handlebars-themes/routing/routes/).

#### Category - Defautl

- We'll call a template `godo-template-category` that I created exclusively for the categories. It is also possible to use other templates, see the templates that this commented.
- First back up your routes in your ghost settings `Labs -> Routes -> Download current routes.yml`
- Re-download the Route and edit `routes.yml` line `routes`

```yaml
routes:
  /Your_Category_Name/:
    controller: channel
    filter: tag:[add_your_tag]
    order: published_at desc
    template:
      - godo-template-category
      # - godo-home-blog
      # - godo-home-travel
      # - godo-home-travel-featured
      # - godo-home-fashion-concept
```

#### Category with Header

We are going to create a category with information such as title and description, as well as an article counter. To get this data to the category will be using the [property data of the routes](https://ghost.org/docs/api/v3/handlebars-themes/routing/routes/#loading-data).

- Create a new page
- Choose your favorite title for Category
- The `URL` has to be the same as the `data` property
- First back up your routes in your ghost settings `Labs -> Routes -> Download current routes.yml`
- Re-download the Route and edit `routes.yml` line `routes`

```yaml
routes:
  /Your_Category_Name/:
    controller: channel
    order: published_at desc
    filter: tag:[add_your_tag]
    data:
      post: page.ADD_YOUR_URL_OF_PAGE
    template: godo-template-category-header
```

Look at the image to understand better

![Category](./documentation/mapache-category.jpg)

## Members / Subscription

Subscribers can be enabled via a checkbox on the Labs page :arrow_right: `Dashboard -> Labs -> Enable Memebers`

:smile: Once enabled, different parts of the theme will appear:

- Login In and Sign Up buttons in the header.
- Header subscription Dropdown
- Footer subscription form.
- Post Sidebar subscription form.

In order for the theme to be fully compatible with member subscription flows you have to add the following routes.

```yaml
routes:
  /signup/: members/signup
  /signin/: members/signin
  /account/: members/account
  /membership/: members/membership
```

To edit plans features, you can edit the `members/membership.hbs` file.

For more information about Members, connecting Stripe and setting the package price, I highly recommend checking the official [Ghost documentation](https://ghost.org/docs/members/introduction/).

![podcast Page](./documentation/members.jpg)

## AMP

??? *Mapache has a nice page for **AMP***

- Navigation
- links to followers in social media
- Tags
- Related Articles (6 articles)
- Buttons to share the article (Facebook - Twitter - Whatsapp)

To customize the AMP page [read here](https://github.com/godofredoninja/Hodor-AMP-Ghost)

## Theme Translation

**Mapache supports:**

- `en` ??? English default language
- `es` ??? Spanish
- `de` ??? German - By [Frederik Niedernolte](https://github.com/MaluNoPeleke)
- `ko` ??? Korean - By [SHGroup](https://github.com/sunghun7511)
- `fr` ??? French - By [Letroll](https://github.com/letroll)
- `pl` ??? Polish - By [kacperduras](https://github.com/kacperduras)
- `pt` ??? Brazilian Portuguese - By *Renato Rattes*
- `sr` ??? Serbian - By [Marjan Pani??](https://github.com/neoartdoo)
- `uk` ??? Ukrainian - By [Maksim](https://github.com/partizan007)
- `tr` ??? :tr: Turkish by [@tolgaaaltas](https://github.com/tolgaaaltas)


![Publication Language for ghost](./documentation/language.jpg)

if you want to have in another language you just have to copy `locales>en.json` and rename the file then translate to your favorite language:

Just enter the [language/locale tag](https://www.w3schools.com/tags/ref_language_codes.asp) of the files to use (e.g.: `fr.json` for French, `zh.json` for Chinese, `ja.json` for Japanese)

## Change Theme Color

> It is very easy to customize with your favorite colors.

![ghost themes colors](./documentation/themes.jpg)

To change the color of the Mapache theme select one of the theme styles below and copy it into the:

`Setting -> Code Injection -> Blog Header`

```html
<!-- 1.- Theme Mapache Deep Orange -->
<style>
  :root {
    --header-logo-color:#fff;
    --header-bg-color:#d25704;
    --header-color:#ffc79e;
    --header-color-hover:#fff4de;
    --header-menu-color:#ffc79e;
    --header-menu-color-hover:#fff4de;
    --composite-color:#007d85;
    --composite-color-hover: #0b97a0;
  }
</style>

<!-- 2.-Theme Mapache Blue Dark -->
<style>
  :root{
    --header-logo-color:#fff;
    --header-bg-color:#1e3757;
    --header-menu-color:#c1cbdb;
    --header-menu-color-hover:#fcffff;
    --header-color:#c1cbdb;
    --header-color-hover:#fcffff;
    --composite-color:#007d85;
    --composite-color-hover: #0b97a0;
  }
</style>

<!-- 3.-Theme Mapache Red -->
<style>
  :root{
    --header-logo-color:#fff;
    --header-bg-color:#c43235;
    --header-menu-color:#ffbbb4;
    --header-menu-color-hover:#fff0ec;
    --header-color:#ffbbb4;
    --header-color-hover:#fff0ec;
    --composite-color:#ff5b5e;
    --composite-color-hover: #c75d5f;
  }
</style>

<!-- 4.-Theme Mapache Blue -->
<style>
  :root{
    --header-logo-color:#fff;
    --header-bg-color:#0273d4;
    --header-menu-color:#ddecfa;
    --header-menu-color-hover:#fff;
    --header-color:#ddecfa;
    --header-color-hover:#fff;
    --composite-color:#0389FF;
    --composite-color-hover: #0273D4;
  }
</style>

<!-- 5.-Theme Mapache Bluen Semi Dark -->
<style>
  :root{
    --header-logo-color:#fff;
    --header-bg-color:#01579b;
    --header-menu-color:#ddecfa;
    --header-menu-color-hover:#fff;
    --header-color:#ddecfa;
    --header-color-hover:#fff;
    --composite-color:#0392FF;
    --composite-color-hover: #01579B;
    }
</style>

<!-- 6.-Theme Mapache Black -->
<style>
  :root{
    --header-logo-color:#fff;
    --header-bg-color:#000;
    --header-menu-color:hsla(0,0%,100%,0.9);
    --header-menu-color-hover:#fff;
    --header-color:hsla(0,0%,100%,0.9);
    --header-color-hover:#fff;
  }
</style>
```

### PrismJS code syntax

Make your code stand out. WIth the PrismJS code highlighter. PrismJS allows you to select which languge you embeded and performs code highlighting according to the language. Neat!

Take a look at the [Prismjs Supported Language List](http://prismjs.com/#languages-list) to find your coding language.

![Prism JS](./documentation/primsjs.jpg)

### Credits

- [Hodor AMP](https://github.com/godofredoninja/Hodor-AMP-Ghost)
- [Normalize](https://necolas.github.io/normalize.css/)
- [Ghost Search](https://github.com/HauntedThemes/ghost-search)
- [Prismjs](http://prismjs.com/)
- [lightgallery.js](https://github.com/sachinchoolur/lightgallery.js/)
- [Lazysizes](https://github.com/aFarkas/lazysizes)
- [Fonts](https://fonts.googleapis.com/css?family=Merriweather:300i,400,700|Roboto|Roboto+Mono:300i,400,500,700)
- [Safari Light - Mockup](https://www.uplabs.com/posts/safari-light-version)

## Copyright & License

Copyright (c) 2017 - 2019 GodoFredoNinja - Released under the [GPLv3 license](LICENSE).
