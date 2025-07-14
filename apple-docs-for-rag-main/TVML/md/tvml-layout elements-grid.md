

- TVML
- Layout Elements
-  grid 

# grid

Arranges elements in a grid pattern.

## Overview

Items inside of the `grid` are displayed in a row that is bound by the size of the screen. Items are automatically moved to another row after a row is filled. Here’s an example of three `lockup` elements inside of a `grid` element.

```

            Movie 1

            Movie 2

            Movie 3

```

### Subelements of grid

- header

- section

### Elements that Use grid

- collectionList

- relatedContent

## Topics

### Valid TVML Styles

margin

Specifies the spacing around an element.

padding

Specifies the padding between the border and contents of an element.

tv-interitem-spacing

Specifies the spacing between child elements.

tv-line-spacing

Specifies the amount of space between lines of text.

### Valid TVML Attributes

binding

Associates information in a data item with an element.

autoHighlight

Specifies that the element should initially be in focus.

itemID

Mark elements for reuse during DOM updates.

needsMoreThreshold

Sets the amount of remaining screen lengths before firing the needs more event.

prototype

Associates a data item type with an element.

theme

Sets the color scheme for an element.

## See Also

### Container Elements

carousel

Arranges images in a row.

imgDeck

Contains several images to be displayed at a later time.

infoTable

Displays contained element information in a vertical format, with each successive element directly below the previous element.

organizer

Creates a generic element with its contained elements arranged through TVML styles.

row

Displays elements horizontally.

section

Combines elements and acts as a single element.

stack

Groups and lays out elements vertically.

shelf

Displays elements horizontally and adds the ability to scroll to offscreen elements.

