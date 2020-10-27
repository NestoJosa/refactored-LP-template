// Overall

New blocks ClientInfoList/SoMeIconsList:
- the blocks display prop (none/block) can be toggled via marketo
- the list items are hidden as default, using a html comment as the tokens value
- the erronous inclusion of a space, either before or after the html comment, does not break the logic - the list item will remain hidden

Hide list items logic
- The reason for why we have two seperate scripts, for hiding ClientInfo list items and SoMe icons, is that the markup is different.


Styling:
- the styles have been broken upp to sass partitions, that each live in its own folder in the sass dir

Marketo Variables:
- the vars have been renamed to convey meaning: 
e.g. boolean1 => HerosWrapperIsDisplayed
e.g. heroOrder => HerosWrapperPosNr

Id selectors => class selectos
- many of the id selectors have been refactored to use class selectors instead,
the id's are from now on, primarily for hooks e.g. mktoHook-<blockName> and js-<blockName>

BEM Naming Convention:
- the block, element and modifier methodology has been applied to the elements that have been refactored, but with some modification to the naming: blocks in PascalCase and elements in camelcase.

Cleanup
- unused bootstrap classes have been removed

Snippet powered footer
- the footer, where the clientinfolist and the someiconslist live, has been refactored into a footer snippet

Heroswrapper - where the hero and subhero live
- the subhero is not displayed as default, but can be toggle on
- the order of the hero and subhero can be changed, but any change to the position of the hero/subhero will only take effect on mobile: the change is reverted on bigger screens
