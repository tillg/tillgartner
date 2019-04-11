title=My static website - Work in progress
type=post
date=2016-08-08
status=published
pic=/img/2016-08/static_site.jpg
category=tech
~~~~~~

##Table of Contents  
[Criteria](#criteria)  
[Generators](#generators)  
[Evaluation Matrix](#matrix)  
[Editors](#editors)  

OK, everytbody does it, even I do it: Static websites. It's fast, it's safe, it does the computing where it belongs (as long as you don't need fancy customization, why should a server think about what the page looks like at read time?). This very site is static (built with [JBake](http://jbake.org/) and hosted on [Github](https://github.com/)). It was fun setting it up, it works great - but I couldn't explain my mother how to use it or how to publish some content on it. And that's what a CMs should be about: It has to be usable in the first place.

Therefore I need anotrher setup. I plan to have a look at some different static web site systems, and set up a list of criteria against which I plan to test the different generators...

<a name="criteria"/>
## Criteria
</a>

* Themes
    * Many
    * Beautiful 
    * Responsive 
- Easy to write
    - Editor with preview
    - Easy handling and referencing of pics
    - Pictures in preview
    - Videos
    - Tables
    - Code with syntax highlighting
	- Automated checking of consistency, i.e. the generated website is correct, complete, the pointers don't point to Nirwana...
* Being able to create an [Accelerated Mobile Page](https://www.ampproject.org/) 
* Functional features & pages
    * Tags, tag pages, tag cloud (could also be an extension)
    * Publishable on Github (it's very fast, free and reliable)
    * Make website private. i.e. accessible only for registered members
    * Publish by email
    * Comment by email
    * Push news to registered users by email
    - Resize pics for fast delivery
    - Easy to create new themes, Themes should be just CSS
    - Based on other HTML, i.e. Bootstrap themes
- Extensible architecture 
    - Can add stuff, i.e. Picture resizing process
    - At least a programming language I know a bit - or that I am curious to learn (that basically boils it down to Java and JavaScript)
    - The generated HTML should be as simple as possible. All formatting sits in the CSS

<a name="generators"/>
## Generators
</a>

When scanning the literature (and Github). this is the list of generators rthat I should probably have a look at:

- Jekyll - Done
- Harp JS - Done
- Hugo - Done
- Metalsmith - Done
- Nikola - Done
- Octopress - Done
- Hexo - Done
- Hyde - Done
- Pelican- Done
- Nanoc - Done
- Middleman - Done
- Lektor - Done
- Gatsby - Done
- Expose - Done
- Wintersmith - Done
- Doc pad - Done
- kirby - Done

<a name="matrix"/>
## Evaluation Matrix
</a>

| Generator                                 | Programming language | Themes                  | Formats                                    | Comment                 |
| :-----------                              | :-----------         | :--------------         |:----------                                 |:-------------------     |
| [Jekyll](https://jekyllrb.com/)           | Ruby --              | Lots ++                 | Markdown, Textile, Liquid ++               |                         |
| *[Harp JS](https://harpjs.com/)*          | NodeJS  ++           | Some 00                 | Markdown, EJS, Jade, LESS, Stylus... ++    |                         |
| [Hugo](https://gohugo.io/)                | GO --                | Some 00                 | Markdown, asciidoc, reStructure ++         |                         |
| *[Metalsmith](http://www.metalsmith.io/)* | Node JS --           |                         |                                            | Looks very flexible. Also see http://dbushell.com/2015/05/11/wordpress-to-metalsmith/   |
| [Nikola](https://getnikola.com/)          | Python --            | Few --                  | reStructuredText, Markdown,                | Looks just so so... |
| [Octopress](http://octopress.org/)        | Python --            | Some 00                 |                                            | Is just a package around Jekyll.|
| *[Hexo](https://hexo.io/)*                | Node JS ++           | Some 00                 | Markdown, different flavors, Jekyll Plugins ++ | Looks very flexible, uses standard template engines (EJS, Jade, Swig...), allows to integrate scripts and plugins. ++|
| [Hyde](http://hyde.github.io/)            | Python --            | Little --               |                                            |                         |
| [Pelican](http://blog.getpelican.com/)    | Python --            |                         |                                            |                         |
| [Nanoc](http://nanoc.ws/)                 | Ruby --              |                         |                                            |                         |
| [Moddleman](https://middlemanapp.com/)    | Python --            |                         |                                            |                         |
| [Lektor](https://www.getlektor.com/)      | Python --            |                         |                                            |                         |
| [Gatsby](https://github.com/gatsbyjs/gatsby)| Node JS, React     | No --                   | Markdown 00                                | Looks very flexible, but pretty complex...|
| [Expose](https://github.com/Jack000/Expose)| Shell scripts --    |                         | Markdown and picture folders               | Specifically for picture sites.|
| *[Wintersmith](http://wintersmith.io/)*   | Node JS, CoffeeScript ++ | Little --           | Markdown, Jade, ...                        | Looks very flexible, LESS, Sass, Stylus. Might be a bit complex...| 
| [DocPad](http://docpad.org/)              | Node JS ++           | No --                   | Markdown and others ++                     | Looks flexible but complex |
| [kirby](https://getkirby.com/)            | PHP --               |                         | Markdown                                   |                             |

As a result I should have a closer look at *[Harp JS](https://harpjs.com/)*, *[Metalsmith](http://www.metalsmith.io/)*, *[Hexo](https://hexo.io/)* and *[Wintersmith](http://wintersmith.io/)*.

After quickly reading thru the websites of the above tools I decided to give it a try with *[Metalsmith](http://www.metalsmith.io/)*.

<a name="editors"/>
## Editors
</a> 

When you think of a static site generation from a base of Markdown files, it quickly becomes natural to look for a good editor. What we want from our editor:

* Preview Markdown
* Preview including the CSS and other transformations that our site generator uses - to make sure we see the same result as it will be displayed in production
* Preview including images. This might be non trivial since the images might be located on a different path in DEV as in PROD...
 Overa ll this means the editor must launch a compilation / composition process that produces the web view every time the Markdown source has been modified.

Editor we look at

| Editor                                | Markdown / HTML Preview           | Comments                          |
|:------------------                    | :----------------------           | :-------------------------        |
| Visual Code                           | ?                                 | Might have something suitable     |
| Atom                                  |                                   |                                   |
| Brackets                              |                                   |                                   |
| [Caret.io](https://caret.io/)         |                                   |                                   |
| [IA Writer](https://ia.net/writer)    | Claims so...                      |                                   |

... probably some more...

# History
* August 2016: Started this page
* Jan 2017: Continued while being in Thailand with the family, Tomi & Beate