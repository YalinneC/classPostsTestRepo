#Responses Week 3

##Introduction | HTML & CSS
*Duckett, Jon*

The intro to this textbook briefly talks about the main web technologies that the rest of the writing intends to teach. It describes the content/structure duties performed by HTML and the styling capabilites of CSS and how the two work together to create front-end web pages. It also gives a brief overview of how *browsers* are used retrieve and interpret these pages.

The important information, I think, is on pages 9 and 10, wherein Duckett describes the basic functionality of the web as most user know it; how DNS servers work and what it actually means when a user types a URL into their browser and visits a page. It describes how the request bounces all over (sometimes across country borders and oceans, even) and is directed to the proper location determined by the Domain Name System servers. Request are routed to the proper IP where the page/files are hosted on a server and sent back to the user through their browser. I think it's cool that the book starts of with such a practical, informative overview of how the "internet" as most people understand it actually works.

##Chapter 1: Structure | HTML & CSS
*Duckett, Jon*

Structure is important to web page design. Duckett explains that oftentimes, web pages are essentially electronic versions of the print media they are trying to mimic: News sites emulate the headers, text, and images of newpapers; forms emulate headers, textboxes, and checkboxes *(this might even be an interesting foray into further discussion on Haas' article from last week regarding the non-linearity and coexsistence of "old" and "new" technologies)*. Browsers interpret and display content formatted like they are in print by reading certain HTML **elements** appended to the content: a pair of opening and closing **tags** with the content to which the element is to be applied nested between them. The characteristics of these elements may be further specified by including **attributes** in the tags that consist of an attribute **name** and corresponding **value**.

Duckett introduces three basic tags used in HTML: `<body>`, `<head>`, and `<title>` and explains how, together, they make up the basic parts of a web page. He explains how to create a simple web page in a text editor and view it in a browser. He explains the premise of a content management system (CMS) and how the editors in these systems are creating HTML code to be placed in a behind-the-scenes template, allowing users with little to no knowledge of HTML to create new web page content or to minimally tweak the formatting of their pages.

##Chapter 4: Links | HTML & CSS
*Duckett, Jon*

Links, an essential component of the web experience, are created using the `<a>` tag. The page to which the link points is defined using the `href` attribute (it's name) and the corresponding URL (its value). Duckett gives the following example of a link:

```
<a href="http://www.imdb.com">IMDB</a>
```

This element, when interpreted by a browser, displays like this:

<a href="http://www.imdb.com">IMDB</a>

He also explains the difference between external and relative links and how to notate these accordingly. Also, I like the way Duckett discusses the importance of good practice in creating links and using proper text as a measure of usability. It's not enough to just have HTML elements; they must be logically and carefully considered for maxium usability and accessibility standards.

Duckett then explains the importance of internal site structure and how pages should be organized. He explains root folders, sub-directories, the index.html default page, and how each folder/file is located where it can be found with a specific path called a **Uniform Resource Loader** (URL). He also touches on email `mailto:email@company.com` links, anchor-style jump links, and how different attributes can give links different behaviors (like opening in a new tab).

##How Did We Get Here?
*Pilgrim, Mark*

This piece is essentially a very broad historical (as far as 1993 being considered "history") overview of the development of HTML and web standards.

Way back in the early days of HTML, the basic elements we now take for granted were just beginning to form in the minds of early developers. The example Pilgrim follows is the early development of the `<img>` tag. Many developers were working on and proposing new ways of implementing a similar technology before the days of W3C and standardized web practice. Marc Andreessn, developing the Mosaic browser, had the initial proposal and eventually released a version with support for his proposed tag. It didn't include many of the attributes and other functionality that many other developers had in mind, but in the end, his version is the one that stuck. It stuck, "Quite simply, because Marc Andreessen shipped [it], and shipping code wins"

Interestingly, HTML has lived on more than 20 years into the future, and continues to evolve as an "unbroken line." There has been no reversal of standards, no completely new technologies. Everything seems to continue to develop, and even web pages from 1993 load on my state-of-the-art iPhone 6 in 2015. *Could this be an argument in contrast with Haas' idea of the non-linearity of technological change? Or could even be argued that it's in support of this idea of the longevity of old, legacy HTML standards alongside newer HTML 4/5 standards?*

There have been attempts to alter and even change HTML web standards, particularly with those in favor of the stringent standards of XML and its descendants in the form of XHTML; however, these markup tools (denoted by a different MIME type than "older" HTML pages) employed "draconian" error handling—unforgiving, extremely strict standards of page formatting and adherence to "proper" coding. These standards failed to catch wind and eventually fell to the wayside as the more forgiving HTML standards (you could, in theory, have an "improperly" marked-up page and have it still render correctly in a browser) were more favorable for developers and users; no one wanted to see error messages all the time. In fact, according to Pilgrim, if being judged by XHTML standards, more than 99% of pages today have at least one error in them. These pages would all return errors to a user. W3C kept with it though, and developers who believed in HTML evolution broke off to form what's known as the Web Hypertext Applications Technology Working Group (WHATWG) in June of 2004.

The WHATWG worked for five long years detailing and documenting the methods of HTML parsing and how browsers rendered technically "improper" code. They believed in not forgoing the web's decade-long investment in HTML and worked very hard to preserve its use. *I find this extraordinarily interesting because this is what the main job of a technical writer (my major). The detailing of internal systems and technologicl standards goes so far beyond things like online help and instruction manuals; sometimes, in cases like this one, it can mean the death or preservation of the emerging technology that formed the basis of the Web. Being able to write clearly, concisely, and being technologically/digitally literate is so incredibly important to technology, business, society/culture, and commerce, and technical writers are right at the apex of this ever-changing technological front.*