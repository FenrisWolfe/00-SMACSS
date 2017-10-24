##### How did you determine which rules should be placed in each new CSS file?

With difficulty. I assessed what each CSS rule was doing, and compared it to the rules for how you should organize the code based on the SMACSS book. For ID's and things that affected layout I put them in the layout.css. For things that affected visual appearance, such as color or font type, and things that were globally set such as the reset.css, they were moved to the base.css. Basically all of the classes went into the modules.css file, which was everything that didn't fit neatly into either category.

---

##### Did you do any refactoring of the existing CSS? If so, briefly explain what you did and why.

Yes, I split a couple of elements up between the base and layout files, so that they would be properly organized. Also I made sure that the flow of each was logical, with more specific things going towards the bottom of the documents.
