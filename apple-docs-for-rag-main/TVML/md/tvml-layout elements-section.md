

- TVML
- Layout Elements
-  section 

# section

Combines elements and acts as a single element.

## Overview

The `section` element groups elements together so they can be treated as a single element for layout purposes. Here’s an example that uses a section to hold two movie `lockup` elements and places them in a `shelf` element.

```

        Viewers Also Watched

            Turn

            Road

```

### Subelements of section

- header

- listItemLockup

- lockup

- menuItem

### Elements that Use section

- carousel

- grid

- list

- menuBar

- oneupTemplate

- shelf

## Topics

### Valid TVML Styles

tv-interitem-spacing

Specifies the spacing between child elements.

### Valid TVML Attributes

binding

Associates information in a data item with an element.

indexTitles

Specifies index bar titles for a section element.

itemID

Mark elements for reuse during DOM updates.

prototype

Associates a data item type with an element.

theme

Sets the color scheme for an element.

## See Also

### Container Elements

carousel

Arranges images in a row.

grid

Arranges elements in a grid pattern.

imgDeck

Contains several images to be displayed at a later time.

infoTable

Displays contained element information in a vertical format, with each successive element directly below the previous element.

organizer

Creates a generic element with its contained elements arranged through TVML styles.

row

Displays elements horizontally.

stack

Groups and lays out elements vertically.

shelf

Displays elements horizontally and adds the ability to scroll to offscreen elements.

