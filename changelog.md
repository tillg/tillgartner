---
title: To Do & Changelog
---

# To do

- Add Google tracking and ideally have a report of the site usage available to the site readers...
- Learn about fixed URLs for posts so they can be referenced
- Add comments
- Posts that have a cover image should show it on the blog post overview page (aka home page)
- Make a collection _softwareWeNeed_
- Have the last build date & time displayed in the footer of the pages.
- Have the generated site be automatically checked for broken links
- Give the recipes their images back...

# Changelog

## Monday, April 22nd 2019

- Changed the `site.webmanifest` to have a proper name when saving the website shortcut on iOS screen.

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
