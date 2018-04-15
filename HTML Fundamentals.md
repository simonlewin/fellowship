# HTML Fundamentals

## Intro

### Industry Overview

Languages

* Backend - PHP, Ruby, Python, Java, C (C++, C#, objectiveC), JavaScript
* Frontend - HTML, CSS, JavaScript

Different Tech Companies

* Agencies
* Startups
* Corporations
* Any business - web is marketing

Different Roles

* Every project different
  * Product owners
  * Project Managers
  * UX
  * Designers
  * FE Developers (FE Designers, UI Developers)
  * Back End Devs
  * Full Stack Devs
  * Sys Admin
  * Various others: clients, admin staff, investors

HTML & CSS used for 

* Front End Development
* Websites
* Apps
* Art

Link to [Hello & Welcome](https://gitpitch.com/develop-me/fellowship-wk1-beg-html-css#/) presentation

## Basic HTML

HTML is a data structure - used to wrap content

CSS is a data structure - used to wrap style

JS is a programming language - used for interaction _the interaction layer_

Some html... `<html lang="en">`

A closer look: open angle bracket `<`, element - e.g. `html`, attribute - e.g. `lang=` and parameter in double quotes e.g. `"en"`, more attributes?, close bracket `>`, content

Closing tag - open angle bracket `<`, forward slash `/`, element name e.g. `p`, close angle bracket `>`

Two self closing elements:

  * input `<input type="input" firstname="name" />`
  * image `<img />`

Tip - start typing `<htm..` in Sublime Text (subl), auto complete with _Tab_ and subl gives you a HTML template (with file saved as HTML)

### HTML sectioning elements

`<body>` - contains all content can only be one

`<header>` header - for links, etc.

`<footer>` footer

`<article>` an 'article of content', usually with a header (taken out of website and used elsewhere e.g. about blurb)

`<aside>` for related content

`<nav>` navigation

`<main>` element used to wrap all (main) content - Ruth doesn't use becasue of history

`<div>` 'invisible box' usually a better element to use

`<section>` section element if it wasn't an article or to section off

Accessibility - putting the right elements in the right place e.g. `<footer>` instead of `<div>`

### HTML content elements

Headers `<h1>` ... `<hn>` typically n=1 to 6 although now you can have as many as you like

Paragraph `<p>` for text

Lists: `<ul>` unordered list, `<ol>` ordered list, `<dl>` description list

List items `<li>`

  * `<li>` direct child of `<ul>` and `<ul>` is a direct parent of `<li>`
  * Parent & child - what's inside and outside, tabbing to see what's inside and out

Description list `<dl></dl>` for defining terms `<dt>` term element and `<dd>` definition element used for q & a

Anchor `<a>` element - hyperlink - with href (hyperlink reference) attribute e.g. `<a href="https://www.google.com"></a>`

Blackquote `<blockquote>` should have a `cite=""` attribute, there is also a citation element `<cite>`

The HTML `<q>` element indicates that the enclosed text is a short inline quotation

The HTML Details Element `<details>` is used to create a _disclosure widget_ in which information is visible only when the widget is toggled into an "open" state. A summary or label can be provided using the `<summary>` element e.g.

    <details>
      <summary>Summary</summary>
      <p>More detailed explanation</p>
    </details>

Image element `<img />` - is self closing and needs a mandatory source (`src=""`) attribute for the image URL and an alternative text (`alt=""`) attribute to describe the image, e.g.

    `<img src="" alt="A boat sailing on the sea" />`

The HTML `<button>` element represents a clickable button used in toolbars, forms, etc.

Tree structure

Parents and children e.g. `<header>` child of `<article>`, `<header>` parent of `<h1>`, etc.

    <article>
      <header>
        <h1>My Website</h1>
      </header>
    </article>

Link to [01: Basic HTML](https://gitpitch.com/develop-me/fellowship-wk1-beg-html-css?p=day01/01basicHTML#/) presentation

See: [MDN web docs **HTML elements** reference](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)

- - - -

### Exercise 1 - Review

* Needs a `<header></header>`
* Needs navigation with `<nav></nav>`
  * either `<ul>` or inline list (see exercise 2) ok
* Good practice to use `<header></header>` element when you use a header `<h1></h1>` etc.
* Tip - if you type `Lorum...` and autocomplete with Tab in subl it gives 'Lorum ipsum, etc.'
* "Recent Work" is either another article or a section
* Needs a `<header>`
* If another article then images are probably a separate `<section>` - rather than a `<div>` which doesn't hold any value. Down to experience about how the section will get used.
* In footer copyright - reference the code for the character: `&copy` or `&#169`

- - - -

### Exercise 2 - Review

* `<header>` with `<nav>` and inline `<a href=""></a>` links 
* Reusable content definitely `<article>` with a `<header>`
* If not main content then it's probably an `<aside>`, with a `<header>` but with less weight

- - - -

## More HTML 

### HTML Text Elements

`<b>`, `<strong>` - The [HTML Strong Importance Element](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/strong) indicates that its contents have strong importance. Browsers typically render the contents in bold type.

Note: `<font>` legacy element (& others) - no longer used, use CSS instead

`<em>` - emphasis _italicised_, legacy `<i>` - italic

`<span>` like a `<div>` for text used for styling text

`<sup>`, `<sub>` - super and sub-script

`<time>` - date & time

`<code>` - inline code element

`<pre>` - preformatted text

### Media Elements

`<img src="" alt="" />` - image (self closing)

`<video src=""></video>` - video tag

`<video src="" controls="controls"></video>` - video tag with controls

`<audio src=""></audio>` - audio tag

`<video src="" controls autoplay></video>` - video tag with shortcut for controls and autoplay

`<audio>` with multiple `<source>` elements (see: [MDN **source** element](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/source))

`<picture>` - picture element (see: [MDN **picture** element](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/picture]) with `min-width` attribute

`<figure>` - figure element, use with `<figcaption>`, which is not "alt text" but an actual desciption

`<canvas>` - the graphic canvas element - use with either the canvas scripting API or the WebGL API to draw graphics and animations

### Tables

For displaying data NOT for layout
Except email clients which don't render CSS so use tables

* Link to [More HTML](https://gitpitch.com/develop-me/fellowship-wk1-beg-html-css?p=day01/02moreHTML#/) presentation

- - - -

## Googling things...

For HTML [w3schools.com](https://www.w3schools.com/) often comes up first but it's not good and it's not [w3c.org](https://www.w3.org/) the World Wide Web Consortium (W3C) who develop Web standards

Better to use MDN web docs - for example [MDN web docs HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)

And [devdocs.io](http://devdocs.io/)

On Stackoverflow - remember that it's devs answering another devs questions - somebody's opionion - take with 'pinch of salt'

Others like [CCS Tricks](https://css-tricks.com/) - is kept up-to-date

Note that for resources like [HTML5 Rocks](https://www.html5rocks.com/en/), [Smashing Magazine](https://www.smashingmagazine.com/), [sitepen](https://www.sitepen.com/), and [codrops](https://tympanus.net/codrops/) - check the date the article was written, stuff is different now

- - - -

## Talk of the day

"Resilience" by Jeremy Keith at View Source Conference 2016 [https://youtu.be/W7wj7EDrSko](https://youtu.be/W7wj7EDrSko)

    <foo>
      Content
    </foo>

    selector{
      property: value;
    }

JavaScript - imperative language, more power but will throw an error and stop parsing JS

HTML/CSS - declarative language with loose error handling so won't throw an error - liberal in what they accept

1. Identify core functionality e.g. providing the news, ability to send & receive messages, the ability to share photos, write/edit/share, etc.

2. Make that functionality available using simplest technology - news: HTML, social: form field, photo: form field w. large files, write/edit/etc: text area - works, accessible but it sucks

3. Enhance! - e.g. layout, beautiful typography, Ajax, websockets, file API, CSS filters, local storage, service workers

Technical credit of 1 & 2 

"Tiny ponies"

- - - -

## Metadata

All the stuff in the `<head>`

Use [HTML5 Boilerplate](https://html5boilerplate.com/) - "a professional front-end template for building fast, robust, and adaptable web apps or sites"

On GitHub see: [HTML5 Boilerplate](https://github.com/h5bp/html5-boilerplate/blob/master/dist/doc/html.md)

`<title></title>` - title element defines the title of the document, shown in a browser's title bar or on the page's tab

`<meta>` - represents metadata that cannot be represented by other HTML meta-related elements

`charset="utf-8"` attribute - declares the page's character encoding

`http-equiv=" " ...` attribute - contains the name of a HTTP header, hence the attribute name http-equiv(alent). It defines an instruction that can alter server and user-agent behaviour. Use `ie=edge` if available. Explained here on [HTML5 Boilerplate](https://github.com/h5bp/html5-boilerplate/blob/master/dist/doc/html.md#x-ua-compatible)

`name="description" content="This is a description"` - `name` defines the name of a piece of document-level metadata. In this case `description` which contains a short summary of the content of the page. Several browsers use this as the default description of bookmarked pages. `content` the value for the `name` attribute.

`name="viewport"...` - gives hints about the size of the initial size of the viewport. Used by mobile devices only. Makes sure pixel == pixel on retina and zoom works on touch.

`link rel="apple-touch-icon"...` - names a relationship of the linked document to the current document. For example, to do with website icons, favicon.ico, etc.

`link rel="stylesheet"` - or link to external files e.g. CSS (instead of writing CSS in the `<head>` as this quickly becomes unmanageable)

`script src="... .js"` - or link to external JS file (instead of writing `<script>` code in `<head>` or `<body>`)

Note: load JS at the bottom of the page before close of `<body>` tag - to improve page load/peformance

HTML5 Boilerplate mentions a simple web app manifest file... this is to do with PWA - Progressive Web App - an installable version of a web app, this needs:

* manifest file - information about an application (such as name, author, icon, and description) in a JSON text file (for example: [MDN web docs - Web App Manifest](https://developer.mozilla.org/en-US/docs/Web/Manifest))
* service worker - still have a workable app if not on-line
* https - secure version of http (hypertext transfer protocol) - encrypted

Link to [Metadata](https://gitpitch.com/develop-me/fellowship-wk1-beg-html-css?p=day01/03metadata) presentation
