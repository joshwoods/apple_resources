

- TVML
- Lockup Elements
-  overlay 

# overlay

Displays elements on top of other elements.

## Overview

The `overlay` element provides the ability to place elements on top of images contained within a `lockup` element. The `overlay` element superimposes the elements it contains over an image. The `overlay` element creates a view where the elements it contains are arranged using the `tv-align` and `tv-position` styles. Containing elements are centered by default.

Elements contained in the same position are arranged from the top of the cell to the bottom, in the same order in which they are specified in the `overlay` element. You can specify a `` that displays a background image inside of the `overlay`. The background image is top-aligned and is fitted to the size of the `overlay` while keeping the image’s original aspect ratio. Text wrapping inside of the `overlay` only occurs in the `header`, `center`, and `footer` positions.

### Subelements of overlay

- badge

- description

- progressBar

- subtitle

- title

### Elements that Use overlay

- lockup

## Topics

### Valid TVML Styles

padding

Specifies the padding between the border and contents of an element.

tv-align

Aligns an element horizontally inside its parent.

tv-position

Sets the position of an element inside of its parent element.

### Valid TVML Attributes

binding

Associates information in a data item with an element.

prototype

Associates a data item type with an element.

theme

Sets the color scheme for an element.

## See Also

### Lockup Elements

button

Displays a button icon the user can click to initiate an action.

buttonLockup

Creates a button that can also have a badge associated with it.

listItemLockup

Contains a new list item.

lockup

Contains several elements that are treated as a single element.

monogramLockup

Creates a monogram using a person’s image or initials.

