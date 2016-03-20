# Sitelen Sitelen Renderer
HTML, CSS, SVG renderer of Sitelen Sitelen or Sitelen Suwi style of Toki Pona text.

## Introduction
I created Sitelen Sitelen Renderer because I am fascinated by combining the artifical language Toki Pona with the non-linear writing style 'Sitelen Sitelen' by Jonathan Gabel. Unlike other work with Sitelen Sitelen I want the writings to be generated by the computer. My [first attempt](http://nullelement.org/2015/05/living-toki-pona-using-flexbox-layout-and-sitelen-sitelen/) was in the beginning of 2015 when I experimented with CSS Flexbox using SVG for the Glyphs. The algorithm was limited and doomed so in October 2015 I started anew, and set out to create SVG-only sitelen sitelen that can be exported and reused. This is still a hobby project that I work on in my spare time.

On this page you can type (proper) Toki Pona. The text is parsed into structures that can be rendered in the style of Sitelen Sitelen. By hovering at the top of the glyphs you can choose the form that you like. You can even download the self-contained SVG which you can then use wherever.

Mind that this project is very much in alpha, many language constructs are not implemented yet. If you find them you can add them to the issue list. Also check out the Toki Pona [proverbs](http://smoishele.com/sitelensitelen/examples/proverbs/proverbs.html) from Sonja's book generated by Sitelen Sitelen Renderer.</p>

Cheers!

## Attributions

This live sitelen sitelen sandbox web app is made possible by the great work done work before me.

[Toki Pona](http://tokipona.org/) is an artificial language invented in 2001 by Sonja Lang as an attempt to understand the meaning of life in 120 words. In my own search, I am convinced this language should not be used to translate large bodies of text or as an actual means of communication but as a personal tool for soul searching.
        
[Sitelen Sitelen or Sitelen Suwi](http://www.jonathangabel.com/archive/2012/projects_t47.html) is a project created by Jonathan Gabel in 2012 who created a non-linear writing style for Toki Pona inspired by Mayan script. I try to keep the algorithm behind the Sitelen Sitelen Renderer in the spirit of Jonathan's project and allow for the different ways of drawing the sitelen sitelen.
        
The Sitelen Sitelen Renderer parses text based on the [context-free grammar by Zach Tomaszewski](http://www2.hawaii.edu/~chin/661F12/projects.html) in 2012. I am continuing to improve this grammar now that I find it to give wrong parses in more exotic sentences.

The grammar is parsed using a parser based on the [JavaScript implementation of the CYK parsing algorithm](https://github.com/lagodiuk/cyk-js) by Yurii Lahodiuk. I altered it a bit so that the output fits more to what I need for the non-linear writing system.

The [vectorized glyphs](http://forums.tokipona.org/viewtopic.php?f=7&p=13786#p13786) are based on the excellent work by jan Same. To make my SVGs scalable I sadly had to get rid of the non-uniform stroke widths. Also I have slightly different ideas about how to use the containers so I took the liberty of slightly altering some glyphs.
