---
title: Changelog
---

# April 13th 2019

While being in Hongkong, I set up my new site with jekyll.

problems I was facing or things that I just spent time on:

* I didn't like the font on the color of the links as they were displayed by the TeXt theme, so I had to dig in the CSS - as soon as you go CSS at least one hour is wasted...
* Images in the posts didn't show when published on github pages - they do show up when running jekyll locally...
  * Things I tried and that did NOT work:
    * ```yml
    * url: https://tillg.github.io # the base hostname & protocol for your site e.g. https://www.someone.com
	baseurl: /tillgartner # does not include hostname
    * ```