---
title: To Do & Changelog
---

# To do

- Automatically resize images when generating site
  - See [this article](https://www.kevan.tv/articles/automatic-image-resizing-with-jekyll-and-imagemagick/)
- Learn about fixed URLs for posts so they can be referenced
- Add xith disqus
- Posts that have a cover image should show it on the blog post overview page (aka home page)
- Make a collection _softwareWeNeed_
- Have the generated site be automatically checked for broken links
- Give the recipes their images back...
- Make bookmarks page available
- Make a cool 404 page, [for example](http://ati.tn/)

# Changelog

## Sunday, April 28th 2019, Munich, Café Wiener Platz / Gartner parent's home

- Switched to the Gem Based version of the TeXt Theme (remotely loaded from Github)
- Changed the logo to blue ;)
- Switched off `show_edit_on_github`
- Started having tests for broken links

## Tuesday, April 23rd 2019, Waterfront Bar over lunch

- Fixed Google Analytics
- Have the last build date & time displayed in the footer of the pages.

## Monday, April 22nd 2019

- Changed the `site.webmanifest` to have a proper name when saving the website shortcut on iOS screen.
- Added Google ID for tracking on Google analytics. TODO: Does it work?

## Friday, April 19th 2019

- Moved to my URL http://tillgartner.com

## April 18th 2019

- Added Icons
- Made the recipes work

## April 13th 2019

While being in Hongkong, I set up my new site with jekyll.

problems I was facing or things that I just spent time on:

- The font on the color of the links as they were displayed by the TeXt theme, so I had to dig in the CSS - as soon as you go CSS at least one hour is wasted...

### Images

Images in the posts didn't show when published on github pages - they do show up when running jekyll locally...

Things I tried and that did NOT work:

```yml
url: https://tillg.github.io # the base hostname & protocol for your site e.g. https://www.someone.com
baseurl: /tillgartner # does not include hostname
```

To make it work I had to add the site url to the image like so:

```
![sugar cane]({{ site.baseurl }}/img/2015-06/sugarcane1.jpg)
```

It doesn't look like the best way to me, but currently I can't find a begtter solution.
