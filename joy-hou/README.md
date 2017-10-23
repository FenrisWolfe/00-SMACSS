##### How did you determine which rules should be placed in each new CSS file?

It was pretty confusing, to be honest. In base, I placed the rules that should stay constant across the board for the entire site. All inputs on the site should use that font, all hrs should have that styling, etc.

The larger grouping of things were termed as layout. The three main sections if you look at the HTML tree - header, main, and footer. I also grouped the next sub-sections inside those sections into layout because I feel like they were a large-picture enough grouping to be included (nav, article, aside, section).

Anything that is a class, ID, or a smaller sub-grouping within the layout groupings I deemed as a module.

P.S. there is no <hr> image existing for the header HR.

---

##### Did you do any refactoring of the existing CSS? If so, briefly explain what you did and why.

I changed the "nav ul" and "nav li" rules to a class ".navUl" and ".navUl li." SMACSS tries to separate content and layout. If the developer at some point wanted to move the list with all of the icons out of the nav and put it on the bottom of the page, for example, the CSS would not render correctly anymore. Giving the list a class allows it to be moved around layout-wise without affecting the presentation. I could have given each li a class as well, but there were so many of them that I felt like this is where you draw the line for efficiency, presentation, and redundancy. Plus, the it makes sense that the li is tied to the ul because it will always be a child element of the ul.

I changed "main p" to a class called ".instructionsP" for the same reason, although that was a fine line to draw whether I should tie the styling to "article p" or a class. I chose a class since there's only three paragraphs, but if it were any more than that, it might be inefficient to apply a class to each paragraph.

"aside img" -> "#authorImage" - ID because they probably only want to use this once on the page.
"aside p" -> "#authorDescrip"
"aside button" -> ""#shareRecipeBtn"
"aside h3" -> "#authorName" - I gave it an ID because it seems like it would be pretty specific and only used in that one situation, whereas they might want to reuse h3 again on the page.
"section hr" -> ".hrGray"
"footer section p" -> "#copyrightP"
"footer section" -> "footer" - the nesting was redundant, there was nothing in the footer but that section. Deleted section tag under footer in html.
"#logo h1" -> "h1"

Moved classes before IDs in the modules.css and organized roughly according to where they appeared on the page, top to bottom.

Removed background-image from hr because there's no image in our files.
Removed list-bg.png from .recipe because no such image exists.
