#Responses Week 7

##Structuring the historicizing project

The project assignment identifies two specific goals: "... address 1) the political and rhetorical movements motivating a soft web technologies development, and 2) how this particular technology is shaped by print media."

**Media queries**

Personally, I'm a fan of single-page websites that use fixed nav and jump links to organize information- but only if that information is concise enough and well-distributed, visually and semantically. There needs to be good use of visual hierarchy and white space as well as logical information structure to make it work. So, I'm going to address the two parts of the project in reverse, to give my final deliverable more of a narrative-style stream. I'm going to try it out, at least for the draft of this project. If it ends up not working well/based on the feedback I get, I might decide to do it differently. As far as information organization goes, here's an outline for the topics to be covered. Main topics are in bold, supporting ideas/details follow each. See the "topic details" section below for more thorough explanations:

| — **Overview**

| — — What are media queries?

| — — What are they used for?

| — **Historical context (project goal #2)**

| — — Print designers as God - publisher control over presenation

| — — 1830's - masses encourge change of publishers' focus

| — — relationship w/ print, constraints and new affordance

| — — issues of accessibility and equal opportunity

| — **Exigence - need for a new technology** *(may combine this.....)*

| — — 1994 Håkon W Lie original proposal

| — — 2006-2012: drafts for the w3c

| — — — Final standardization and spec

| — **Media queries as shaped in current issues (project goal #1)** *(.....with this)*

| — — emergence of RWD

| — — difference of devices and browser support

| — **Conclusion/Trajectory**

| — — implications

| — — reason vs practicality; use and standards; personal opinions

| — — rethinking the why and subsequently the how of implementation


##Section details

Note: this will be more throughly fleshed out/properly annotated and documented later.


###Overview
Media queries are a CSS rule officially included in CSS3. They are a way for the writer to structure content and web pages in such a way that they "ask" browers certain details when they are fetched: size of the screen and size of the browser window are the most important, and those are what I'll be focusing on. They are used to conditionally load rules (primarily certain CSS rules; sometimes entire files) based on the return of these items. Media queries are one of the key compenents in proper Responsive Web Design (more on this later).

###Historical context
I'm going a little out of order with the project guidlines, but I think this makes sense as an introductory background. In print, the writer/designer is God. Print designers have full control over the layout and presentation of their page; they can be 100% certain that they way they see their printed designs is the way the reader will see it as well. This might be considered an advantage of print *or* a severe limitation. In the early days of the web, designers wanted to be sure that their sites were being seen as designed. The web tried to emulate the printed page in every aspect; layout and design alike.

However, the web has evolved and no longer are people coming to access information in the same way as before. This has happened throughout history: one of the biggest turning points of journalism was in the 1830s with the introduction of "penny papers," which brough newspapers and information to the masses in a new and affordable way. This forced publishers to rethink about what and and for whom they were writing. The idea is the same for the web: people aren't coming to the web from the same standardized desktop any more. We are reaching new markets and new demographics with mobile technologies; less than two-thirds of Americans have home internet access, but 90% now have mobile phones. It's all about seeing where your market is and meeting them there, using technologies that are accessible and provide equal opportunities.

Media queries are a direct response to this changing standard. They are the embodiment of Haas' heralded "human design decisions" in computer technologies.

###Exigence/Current Issues

"When a new medium borrows from an existing one, some of what it borrows makes sense, but much of the borrowing is thoughtless, “ritual,” and often constrains the new medium. Over time, the new medium develops its own conventions, throwing off existing conventions that don’t make sense." John Allsopp, 2001

The print-imitation, desktop-delivered form of web writing and design doesn't fit this model. This is where media queries (and responsive design as a whole) come into play. Thinking back to the Haas reading, this is exactly what she means when she claims that technology is not a linear progression of one technology to the next, and that "old" is not necessarily obsolete when the "new" comes in. There is a place for print, but the web is not print. The web may have evolved from print, yes, but it has adopted new characteristics and new technologies that no longer fit that mode of writing and design. I wrote in a previous response:

*Computer technologies (and writing technologies in general) are, by nature, material conventions and therefore are the product of social constructs and human design decisions. To understand computers as writing tools and their designs, we must see them as tools with histories; that is, they are built upon layers of other writing technologies (alphabets, writing and logic systems, even the physical manifestations of writing) and they are the product of conscious human design decisions (139). This follows the Vygotskian assertion that tools and technologies are not created, but rather culturally and socially "appropriated" (138) and evolved.*

We have to see the web and page design as "the product of social constructs and human design decisions," and media queries are a concrete example of this. The Lie proposal for CSS all the way back in 1994 illustrates some of these tangible concerns, noting the need to be able to adjust to the user, and for the publisher/writer to be able to leverage the capabilities of the web in such a way where he has some semblance of control, but that affords flexibility for the convenience of the user.

*Note: talk about technical specs and recommendation here. will add soon.*

There are many different browsers and models of mobile devices out there; the writer can no longer design for a standardized set of screens. This is why media queries are so important. They are a response to the changing landscape of devices out there to address these issues of accecibility and new demographics; they are implemented because writers and designers now realize that while the web may have evolved from print, there are certain characteristics that are no longer issues of constraint or limitation. They are an evolution; the web can live side by side with print, as old and new technologies must do according to Haas, but it is now its own mode of delivery.

###Conclusion
I'll come back to this once I've organized and narrowed down my thoughts a bit more.
