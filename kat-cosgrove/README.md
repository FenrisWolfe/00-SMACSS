##### How did you determine which rules should be placed in each new CSS file?

I used the base file for anything that should be consistent no matter what, mostly typography rules. Layout contains anything I thought should apply globally as part of the site's theme, though I was torn on some things. Modules contains everything I thought might need to be used in multiple places but not necessarily everywhere, though I can see how some things might belong in layout if almost the entire website is a blog.

---

##### Did you do any refactoring of the existing CSS? If so, briefly explain what you did and why.

I reorganized some of it a little. There were also some inconsistencies in spacing and an extra curly brace. It all seemed pretty easily readable to me, once it was broken down into separate files. 
