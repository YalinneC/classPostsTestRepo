#Responses Week 6

##Historicizing sources

For the historicizing project, we're going to be focusing on different aspects of the technologies we're examining. One aspect is the historical part; how the technology came about and what its importantce was in its specific context of development. The other part is its relation to the writing practices boutd to the technology. I've chosen to start with one source per category that addresses that "realm" of information: 

**[Håkon W Lie | Cascading HTML style sheets -- a proposal](http://www.w3.org/People/howcome/p/cascade.html)**

This is one of the very first documents that proposed the idea of cascading style sheets. It is actually quite heavily skewed toward this idea that would one day become "media queries," although the proposal doesn't use this term; he says that these style sheets should be able to "provide logic to make presentation decisions based on the user's environment; e.g. the size of the screen or the current date." This document laid out the idea of CSS styles; writing in such a way that the publisher has some leverage over his content's presentation; but where the user still has some sense of control. Lie explains early in the Proposal that the lack of control of presentation had been a "source of much frustration among professions that are used to be in control of paper-based publishing."

Though much of the proposal is unspecific to the idea of media queries or responsive content presentation, he says in a section titled "limitations" that "there should be a way of adding and subtracting style sheets from within the document." This is a very tangible concern that Lie recognized that would later be addressed by the official implementation and recommendation of media queries.

**[Pete LePage | Use CSS media queries for responsiveness](https://developers.google.com/web/fundamentals/layouts/rwd-fundamentals/use-media-queries?hl=en)**

There's a lot of technical documentation out there for all of these "soft" technologies, and while they are important and I will certainly be referencing many of them for this project, I really like these articles that are technical in nature, but also offer some sense of practical application and *reason* for choosing one way over another for certain things.

LePage goes over many of the basics for implementing media queries, but also talks about performance concerns and why one might use the `media` attribute in the head link or the `@media` rule embedded in the CSS file as opposed to the `@import` syntax. He also explains many of the common queries used, including `min-device-width`, but he also explains that this query is strongly discouraged, noting accessibility issues in certain devices and browsers that may report improper numbers (device vs screen width). This brings up the issue of old and new technologies, and how we are adjusting our writing practice to support older "legacy" technologies.

There are also other sections of the article that talk about the proper way to use media queries in setting content size and choosing breakpoints, which, while not particular to media queries, are important parts of RWD.

---
Memo notes

The main direction of my project will be to examine how media queries and RWD in general have come about as a response to the growing importance of accessibility, social justice, and equal opportunity. They come about as an awareness of the vast landscape of mediational means that many users and readers are coming through, and they address issues in recent history regarding the quick pace of advancing technology and the prevalence of so-called "legacy" technologies. A lot of the issues that come up are about RWD "best practice"—how do we leverage these technologies to bring content-first design and delivery, while increasing accessibility and technological efficiency.

Some of the recurring issues/themes I've noticed:
- browser support (a big one)
- device width vs screen width
- viewport tags
- publishers control over presentation
- user view flexibility
- performance issues
- mobile-first RWD (min width queries)