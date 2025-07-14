

- TVML
- Layout Elements
-  organizer 

# organizer

Creates a generic element with its contained elements arranged through TVML styles.

## Overview

The `organizer` element provides the ability to manually arrange its containing elements. The `organizer` element creates a view where the elements it contains are arranged using the `tv-align` and `tv-position` styles. Containing elements are centered by default.

Elements contained in the same position are arranged from the top of the cell to the bottom, in the same order in which they are specified in the `organizer` element. You can specify a `` that displays a background image inside of the `organizer`. The background image is top-aligned and is fitted to the size of the `organizer` while keeping the image’s original aspect ratio. Text wrapping inside of the `organizer` only occurs in the `header`, `center`, and `footer` positions.

### Subelements of organizer

- background

- badge

- button

- buttonLockup

- img

- ordinal

- placeholder

- ratingBadge

- row

- seasonBadge

- text

- textBadge

### Elements that Use organizer

- banner

- lockup

- listItemLockup

- ratingCard

- reviewCard

- row

## Topics

### Valid TVML Attributes

binding

Associates information in a data item with an element.

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

row

Displays elements horizontally.

section

Combines elements and acts as a single element.

stack

Groups and lays out elements vertically.

shelf

Displays elements horizontally and adds the ability to scroll to offscreen elements.

