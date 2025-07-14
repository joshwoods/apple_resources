

- TVML
- Information Elements
-  card 

# card

Creates a generic element with its contained elements arranged through TVML styles.

## Overview

The `card` element provides the ability to manually arrange its containing elements. It creates a view where the elements it contains are arranged using the `tv-align` and `tv-position` styles. Containing elements are centered by default.

Elements contained in the same position are arranged from the top of the cell to the bottom, in the same order in which they are specified in the `card` element. You can specify a `` that displays a background image inside of the `card`. The background image is top-aligned and is fitted to the size of the `card` while keeping the image’s original aspect ratio. Text wrapping inside of the `card` only occurs in the `header`, `center`, and `footer` positions.

### Subelements of card

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

### Elements that Use card

- grid

- shelf

## Topics

### Valid TVML Styles

border-radius

Changes the shape of an element’s corner.

### Valid TVML Attributes

binding

Associates information in a data item with an element.

prototype

Associates a data item type with an element.

theme

Sets the color scheme for an element.

## See Also

### Card Elements

reviewCard

Displays abbreviated review information for a media item.

ratingCard

Contains rating information about a product.

