# Principles of Creating Maps

Maps are a powerful form for visualization and storytelling. If used correctly, they can hit the sweet spot of visualization that's anchored in past experience but pushes the viewer to see and understand something new.

But mapmaking as a non-expert activity is relatively new - you can't (yet) export from Excel to a map, and a lot of the knowledge you need for it is locked up in books or supposedly something you need a degree for.

And so it's a little easy to mess up, and when you do, cartographers, like other trolls, love schadenfreude. So let's start with principles you can follow.

I'll be mushing together a few sources for this part. One of them is [mapschool.io](http://mapschool.io/), a free and simple introduction to maps. Another is [101 Things to Learn in Art School](http://www.amazon.com/101-Things-Learn-Art-School/dp/0262016214).

## Begin

Art is the result of process.

> We don't use templates for our visualizations, just like we don't use madlibs for our articles

[Amanda Cox](http://amandacox.tumblr.com/), NYT Graphics Desk

Start with nothing. Record your process. Iterate from nothing again, learning from your process. This is how you learn.

Your process might be recorded in `git` or it might be in your notes. But the key is: don't cheat too soon. If something you do is a mistake, the more you do it the more you will realize that.

---

Art speak: Composition is the foundation of image making. Visualization speak: position is the most important signal, and integrality is evil.

The central challenge of most visualization is **making things look different**. We have different channels to do this, like position, color, animation, sound, texture, shape, symbol.

Using more than two of these channels at once leads to integrality: the channels interfere and it's much harder to differentiate between things.

Here are the cheat codes:

* Design in Black and White First
* Multiple things = multiple graphics

---

Maps are **data attached to shapes**.

Let's talk about data. There are three types of data you'll visualize: categories, rates, and absolute numbers. Figure out which one you're dealing with before you make any visual decisions, because everything starts here.

Categories are the easiest: all you need to communicate is **difference**. You can get extra points if you the ways you represent categories are kind of self-explaining - red for republicans, blue for democrats, and so on.

Rates and absolute numbers are usually convertible into each other. For instance, Washington, DC has a bunch of gunshot detectors. Each detector records some number of gunshots, but they were installed at different times. So, don't just show how many, show how many **per** time since installation. Not too hard.

Rates and absolutes are sensitive to being attached to shapes. California has tons of homeowners going into debt because it has tons of homeowners, and it has tons of homeowners because it has lots of population, since it's huge. If Delaware had the same numbers, it would be unusual.

The cheat codes:

* Determine your data and shapes early, and let them determine the visual

---

**Data is not information.**

> Chastising the Spanish artist for painting unrepresentative cubistic abstractions, a layman withdrew a photograph of his wife from his pocket and held it up to Picasso with the admonition, “Why can’t you paint realistically, like that?” “Is that what your wife really looks like?” Picasso asked. “Yes,” replied the man. “Well, she’s very small, and quite flat.”

In other words: processing, analysis, aggregation, visualization **is all the same process**. Good visualization comes from good data, by result of good processing. You do not make world-sized maps. Population maps do not have pictures of everyone.

Here are the cheat codes:

* Transparent process & real data makes processing okay. Create the curtains and give people a rope to pull them back.
* Learn at least one tool for processing data. Fiona and QGIS are great.

---

A map is an expression of its medium.

Web maps are not paper maps on the internet. They are both less and more limited, and a good process works within their limitations in a smart way.

To be specific: to learn the limitations **you need to find them**. Make maps of way too much data and see when your browser (or your phone) crashes. Try combining map projections and see what happens.

Here is the cheat code:

* Early on, you might not have the guts to tell yourself your work sucks when it does. Collaborate with someone who does and read their work like it's your job.
* Find ways to fail more quickly. Start a 'maps blog' that posts way more often with way less editorial guidance.

---

Conception cannot precede execution.

Discover what you're going to make by making it. Design web maps in code, not in Photoshop.

---


## References

* http://www.cs.ubc.ca/~tmm/talks/vizbi11/networkbio12-4x4.pdf
* http://webstaff.itn.liu.se/~jimjo/courses/AIV-2009/papers/bostock.pdf
* http://wtf.tw/ref/white.pdf
