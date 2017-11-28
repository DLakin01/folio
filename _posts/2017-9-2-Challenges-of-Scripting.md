---
layout: post
title: Challenges of Scripting
---

The biggest challenge I’ve faced in learning to develop my own code and web applications is keeping the order of events, function calls, and code blocks straight in my head. As someone coming from a largely academic/literary background, I’m used to ideas and text flowing straight down the page, from top to bottom. To be sure, some tools for web development, like HTML and CSS, function in similar ways, but when it came to learning my first bits of JavaScript I was very much thrown for a loop (sorry for the terrible pun).

When working in JavaScript, what’s important is not necessarily what comes first, but what bit of code is called and inserted into what. A function halfway down the page when viewed in a text editor may be called as an argument for another function near the top, which itself may have other functions and operations nested inside it that can call other elements from elsewhere in the document. A developer must take into account scope, when certain DOM elements will be fully loaded, and how different files can or can’t “talk” to each other.

I reached a breakthrough of sorts when putting together the code for the Bloc Jams website. I was getting stuck on the different variables used as arguments for functions, the placement of the functions themselves, and how documents like album.js worked together as a whole. Then, at one point, without really noticing the transition, I found myself understanding that function A and function B didn’t have to have the same arguments, and that variables assigned in one part of the code could be passed in under a different name in another.

My concern going forward is that I still don’t have the required mental and organizational fluency with JavaScript, and that if I zoom out to the more birds-eye view required to construct a working application, I will lose the granularity required to put together functions that do what I need them to. The solution may be to take each task separately - to spend time mapping out the broad view of whatever application I’m developing and, once it’s complete, dive into the building of individual blocks of code. It would also be an iterative process, returning to the broader view whenever necessary.

With that in mind, it’ll be one more step at a time as I continue on my Bloc journey. Just got to keep from getting overwhelmed by things, and keep an eye on where I’m going!
