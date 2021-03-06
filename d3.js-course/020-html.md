---
title: Understanding HTML
layout: dataviz
last_modified_at: 2017-08-12
permalink: d3-viz-course/understanding-html
categories: [adv]
---

[D3.js](https://d3js.org/) stands for **Data-Driven-Document**.  
The **Document** here refers to the DOM, the Document Object Model of the web platform.

The DOM is the way for the browser to keep in memory, interpret and manipulate a structured content.

The language used to build a Document is called HTML (Hyper Text Markup Language). It's based on XML, nodes, attributes...

A text file that contains HTML markup need to be saved with the extension `.html`, this way the browser knows the typo of file is going to read in order to interpret correctly.

> Understanding HTML is essential if you want to work with D3.

Here a minimal, valid, HTML source that can be put within a file named such as `index.html`. There are three main tags that are:

- `html`: the main container
- `head`: this tag will include additional functionalities, libraries, etc, stuff not visible
- `body`: this tag will include all the content, text, images, videos, etc, stuff that **is** visible

```html
<!DOCTYPE html>
<html>
  <head></head>
  <body></body>   
</html>
```

> Pro-Tip: Indentation is Key!

Look at the indentation. The browser doesn't care but we, as human, actually do! A clean and well structured document is key to continue to work with it without geting lost at some point.

The above document won't render anything because the `body` tag is empty, let fill it with something, let's say, a sentence. Before that, you need to know that text will be rendered according to the given tag associated with.  
This sentence:

```html
<h1>This will look like a title</h1>
```

will be rendered differently then:

```html
<p>This will look like a title</p>
```

Got it?

We need to put within the `body` otherwise it won't be visible:

<lineselect lines="4-4" ></lineselect>

```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <h1>This will look like a title</h1>
  </body>
</html>
```

Now we can see something on screen, not something very fancy but it's a start.

What about adding something more cutting-edge, like an image? Here we are:

```html
<img src="http://placekitten.com/200/300" />
```

Remember, it should be placed within the `body` tag in order to make it visible.

Go to the next lesson: [Understanding CSS](understanding-css)