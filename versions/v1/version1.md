// Overall

Styling:
- the styles have been broken upp to sass partitions, that each live in its own folder in sass/
- the styles thare are in this folder, are the compiled styles.

Marketo Variables:
- the vars have been renamed to convey meaning: 
e.g. boolean1 => HerosWrapperIsDisplayed
e.g. heroOrder => HerosWrapperPosNr

Id selectors => hero selectos
- many of the id selectors have been refactored to use class selectors instead,
the id's are from now on, primarily for hooks e.g. mktoHook-Hero

BEM Naming Convention:
- the block, element and modifier methodology has been applied to the elements that have been refactored.
- but with some modification to the naming; blocks in PascalCase, 



