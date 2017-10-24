##### How did you determine which rules should be placed in each new CSS file?

I placed the CSS selectors that target large pieces of the content, like the body, input or * selectors in the base.css file. I also added elements that contain default styles for all elements on the page. I debated whether or not I wanted to add the reset.css file into the base.css file, I opted to combine the reset.css file with the base.css file for now.

I placed the major layout selectors such as main, nav, aside, and footer selectors in the layout.css file since they primarily deal with the layout of the content.

I placed the CSS selectors that stand alone in the modules.css file. This includes selectors for the logo, slogan, hr, and print icons since they stand alone. The modules.css file seems to be concentrated with classes and id selectors.

---

##### Did you do any refactoring of the existing CSS? If so, briefly explain what you did and why.

I refactored the code by adding the reset.css file content into the base.css file and removing the reset.css file. I then had to make some adjustments to prevent duplicate selectors (for example, combine the body selectors into one). I also had to make sure to keep the imported Google Font at the top of the base.css file.
