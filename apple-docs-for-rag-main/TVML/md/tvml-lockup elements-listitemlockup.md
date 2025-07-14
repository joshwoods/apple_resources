

- TVML
- Lockup Elements
-  listItemLockup 

# listItemLockup

Contains a new list item.

## Overview

The `listItemLockup` subelements are arranged using the `tv-align` and `tv-position` styles. Containing elements are centered by default.

Elements contained in the same position are arranged from the top of the cell to the bottom, in the same order in which they are specified in the `listItemLockup` element. You can specify a `` that displays a background image inside of the `listItemLockup`. The background image is top-aligned and is fitted to the size of the `listItemLockup` while keeping the image’s original aspect ratio. Text wrapping inside of the `listItemLockup` only occurs in the `header`, `center`, and `footer` positions. Here is an example of a two `listItemLockup` elements inside a `section` element.

```

        1
        Opening sequence
        11:14

        2
        Fight song
        3:47

```

### Subelements of listItemLockup

- decorationImage

- decorationLabel

- img

- ordinal

- organizer

- placeholder

- relatedContent

- row

- subtitle

- title

### Elements that Use listItemLockup

- section

## Topics

### Valid TVML Styles

height

Specifies the height of an element.

tv-align

Aligns an element horizontally inside its parent.

tv-highlight-color

Changes an element’s color when it comes into focus.

tv-position

Sets the position of an element inside of its parent element.

### Valid TVML Attributes

autoHighlight

Specifies that the element should initially be in focus.

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

lockup

Contains several elements that are treated as a single element.

monogramLockup

Creates a monogram using a person’s image or initials.

overlay

Displays elements on top of other elements.

