

- TVML
- alertTemplate
-  autoHighlight 

Article

# autoHighlight

Specifies that the element should initially be in focus.

## Overview

Use the `autoHighlight` attribute to denote the element that is initially in focus. Both the containing element and one child element must be set to `true`. Remove the `autoHighlight` attribute from your element to disable initial focus.

### Values for autoHighlight

Boolean  
The initial focusable state for an element. Set to `true` to have the element initially be in focus.

### Elements that Use autoHighlight

- alertTemplate that contains `button` elements

- catalogTemplate that contains `listItemLockup` elements

- compilationTemplate that contains `listItemLockup` elements

- descriptiveAlertTemplate that contains `button` elements

- grid that contains `lockup` elements

- listTemplate that contains `listItemLockup` elements

- paradeTemplate that contains `listItemLockup` elements

- row that contains any `focusable` element

- segmentBar that contains `segmentBarItem` elements.

- shelf that contains `lockup` elements

- showcaseTemplate that contains `lockup` elements

Note

The `shelf` and `grid` elements can only use the `autoHighlight` attribute when contained within a `productBundleTemplate`, `productTemplate`, or `stackTemplate`.

## See Also

### Valid TVML Attributes

binding

Associates information in a data item with an element.

layoutDirection

Specifies the direction in which text is displayed.

prototype

Associates a data item type with an element.

theme

Sets the color scheme for an element.

