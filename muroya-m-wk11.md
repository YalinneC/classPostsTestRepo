#Responses Week 11
##Chapter 5: Short Descriptions

The `<shortdesc>` (short description) element serves several purposes, and may function as:

* The first paragraph of a topic (briefly summarizing the main point)
* Link previews for related or child topic links (such as for hover-activated description boxes)
* Abstracts for search engine results (containing key terms and effective descriptions)

Since short descriptions must adequately address all of these functions, they can be challening to write. Some general guidelines for writing effective short descriptions:

* Briefly state the topic purpose: what it's about and why users care. Don't build up to the main point; instead focus only in the needed info.
* Include a `<shortdesc>` with every topic. This way all links will have short descriptions and search engines won't pull from unintended data.
* Use complete sentences. If using incomplete sentences, be aware that you may face some inconsistencies with short descriptions.
* Avoid lists, tables, and figures. These may not generate proper output (if at all) and may lead to confusion.
* Keep short descriptions... well, short. Generally 35 words or fewer; 50 at most in rare cases.
* Avoid self-referential language like "this topic describes" or "in this tutorial." Keep it to the relevant information.
* Do not repeat the topic title. It doesn't give any new information and doesn't help the reader.
* Avoid cross-referencing/links. In some cases they cannot be followed and just add clutter. DITA doesn't allow `<xref>` elements inside your `<shortdesc>`.

In general, remember to answer the who/what/when/where/why/how of your task topic short descriptions. Also focus on user goals, not the actual interface or use of tools. Some (very) brief contextual information may be placed in your `<shortdesc>` to help position the reader, but remember to keep it task-oriented. For concept topics, breifly define the object and why users should care, or what they need to understand. For reference topics, define the object and explain what it would be used for.

If you are moving content to DITA, avoid copy-pasting intro paragraphs/sentences; it might save time, but in the long run, well-constructed short descriptions are worth the effort for consistency, reliability, and user-centeredness. With conditional processing, multiple `<shortdesc>` elements may be placed inside the `<abstract>` to display for different output types.

##Chapter 6: DITA Maps and Navigation

DITA maps are the structural documents that define output for DITA information sets. They bind topics together, define the information architecture, and create topic relationships.

Maps include content with the `<topicref>` element. It can be a topic, another map, or other supporting non-DITA files. Information organization, related topics, and order are all defined in the DITA map. Organization might differ for different output types or use cases. Large-scale projects might benefit from information modeling, which helps to organize large groups of topics into logical information sets.

DITA maps may be nested and referenced together, as each `<map>` is intended to address a single topic or user goal. Though many tasks may be compiled into one document, it makes much more sense to reference several maps together: you can organize/reorganize content by chapter, information sets, etc., and it allows for modular maintenance and updates to information.

DITA maps also afford control over component topic information such as `<title>` and `<shortdesc>` elements; you may choose to override topic attributes or add them to non-DITA links. You may also choose to suppress items from certain output types (HTML and PDF) or from the table of contents.

##Chapter 7: Linking

**Hierarchical links** are created by nesting `<topicref>` elements within other `<topicref>` elements in your DITA map. This nesting practice creates structure between topic/sub-topic relationships. The child topics (nested) will be linked at the bottom of the parent file and vice-versa.

The `collection-type` attribute is appended to a `<topicref>` elements to define the relationship between topics. It can have one of four values:

* Sequence: numbered topics, each with a link to previous/next
* Choice: unordered list (when multiple subtopics/child topics may be completed as different choices)
* Unordered: unordered list (when different steps may be completed in any order)
* Family: unordered list, but with each child topic having links to its related child topics (for closely related topics)

You may also set collection types in a relationship table on the `<topicgroup>` element.

##Scrawlings

It's pretty crazy that there are some 400 different elements in DITA Land. No wonder people people invest in dedicated editors like Oxygen. You'd think that, with there obviously being no practical limitation on the amount of different types of elements, `<shortdesc>` could have pretty reasonably be split up into a couple different elements that each perform different functions, right? One element for meta description (or equivalent PDF data), one for summary, and one for link preview. Sure, maybe that complicates things even more but honestly DITA/XML is already so rigidly complex that I can't see it having any negative procedural impact for authors. But then again, what do I know?

Again, the hard part with this technology is not the tool itself; a quick google search or lookup can teach you pretty much anything you need to know about DITA, but it's the content/information architecture development that will take practice and consideration: what are my topics/subtopics' relationships to one another? How can I group them in a way that makes sense? What even are relationship tables and how do/should I use them? Do I even need to use them? Also, disconnecting ideas and information so that they can be reused/referenced and applied to a larger object is so much different than the narrative-based model that I (and many writers/students) are used to. It's a different way of approaching the user-centered and goal-oriented information design mindset.

---

##Task Analysis: Media Queries

1. **What is the student goal?**
    * Responsively resize h1 elements on screen
2. **What tasks does the user need to perform to accomplish the goal?**
    * Create a validating, structurally sound HTML document
        * Must include at least one instance of the element in question
    * Create a CSS file or HTML style section
    * Define h1 sizes for basepoint screen (mobile) and target screen (other)
    * Define media breakpoint(s)
    * Write media query
3. **What are the mental and physical steps required for each task?**
    * **mental:** Developing proper HTML; considering different screen sizes; considering the device constraints/affordances
    * **physical:** Moving the mouse; clicking buttons; typing out code
4. **Who performs the task?**
    * **audience:** Readers/users of the site text
    * **experience:** All levels of web designers/writers. Pros use these techniques, but it is accessible for beginners as well
    * **role:** Web/information designer
    * **authority:** Executive authority over typography; should adhere to web standards and best practices
5. **When and under what conditions is the task performed?**
    * **requirements:** Text editor, proper HTML and CSS files, some level of knowledge of web files/coding
    * **limitations:** File sizes, practicality, browser compatibility, accessibility
    * **environment:** Digital. Interfacing with computer, tablet, or mobile phone
6. **What are potential distractions to accomplishing the goal?**
    * **troubleshooting:** Limited experience with HTML semantics/syntax; trial-and-error sizing and breakpoint testing
    * **alternative path:** one-size-fits-all non-responsive text that does not resize
    * **exception path:** improper syntax; broken file links; bad file structure; browser compatibility issues
7. **What does the user need to know about the task?**
    * **duration:** short (assuming completed HTML and initial code docs)
    * **complexity:** simple; can become more complex with sizing units/multiple breakpoints and elements
    * **frequency:** Should only need to be completed once/site (if in a stylesheet)
8. **What is the sequence of tasks?**
    1. Open your HTML and CSS documents
    2. Determine the appropriate size for h1 on mobile (ex. 2em)
    3. Add a font-size attribute to your h1 CSS:
    ```
    h1 {
        font-size: 2em;
    }
    ```
    4. Determine the appropriate size for h1 on desktop (ex. 4em)
    5. Determine breakpoint at which you want to resize h1 (ex. 40em)
    6. Add media query below h1 in CSS:
    ```
    h1 {
        font-size: 2em;
    }
    @media (min-width: 40em;) {
        h1 {
            font-size: 4em;
        }
    }
    ```
    7. Save all and test resizing of text
9. **What is the expected result?**
    * H1 tags should resize based on browser window/device width (smaller font size for smaller devices)