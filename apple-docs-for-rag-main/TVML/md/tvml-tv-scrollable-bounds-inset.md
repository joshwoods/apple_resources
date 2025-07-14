

- TVML
-  tv-scrollable-bounds-inset 

# tv-scrollable-bounds-inset

Creates an unscrollable region of a specified size at the top and bottom of the stack template.

## Overview

Use the `tv-scrollable-bounds-inset` style to create an unscrollable region of specified size from the top and bottom of the `stackTemplate`. When you use unscrollable regions, the content offset is no longer automatically adjusted to allow “peeking” — the partial view of elements directly above and below the focused element.

Once focus is shifted from an unscrollable region to a scrollable region, the content offset of the template is adjusted to the specified `tv-scrollable-bounds-inset` value, so that the unscrollable region doesn’t appear on screen.

Note

By default, the entire template is scrollable if you don’t define the tv-scrollable-bounds-inset style.

Here’s an example that sets the inset (unscrollable space) at the top, right, bottom, and left all to 100 points.

```

        …

                …

```

Here’s an example that sets the inset (unscrollable space) at the top to 50 points, and the inset at the bottom to 75 points.

```

        …

                …

```

### Values for tv-scrollable-bounds-inset

Float  
The amount of unscrollable space, in points, set at the top, right, bottom, and left of the `stackTemplate`.

Float Float  
The first value determines the amount of unscrollable space in points at both the top and the bottom of the `stackTemplate`. The second value determines the amount of unscrollable space at both the right and left.

Float Float Float  
The first value determines the amount of unscrollable space in points at the top of the `stackTemplate`. The second value determines the amount of unscrollable space at both the right and the left. The third value determines the amount of space at the bottom.

Float Float Float Float  
The first value determines the amount of unscrollable space in points at the top of the `stackTemplate`. The second value determines the amount of unscrollable space at the right. The third value determines the amount of space at the bottom. The fourth value determines the amount of space at the left.

Important

Currently, creating unscrollable regions at the left and right of the `stackTemplate `is not supported and will not have any effect.

### Elements That Use tv-scrollable-bounds-inset

- stackTemplate

## Topics

### Specifying Inset Location

tv-scrollable-bounds-inset-top

Specifies the size of an unscrollable region only at the top of the stack template.

tv-scrollable-bounds-inset-bottom

Specifies the size of an unscrollable region only at the bottom of the stack template.

## See Also

### Styles

Color Styles

Provide the ability to customize an element’s color.

Text Styles

Change the text characteristics for an element.

Element Shaping

Modify the size and shape of an element.

Element Alignment and Spacing

Modify the alignment and spacing between elements.

tv-placeholder

Sets a default image for an `img` or `monogram` element.

tv-rating-style

Sets the displayed image for rating a product.

tv-transition

Specifies how an element transitions on and off the screen.

tv-text-highlight-style

Specifies how an element looks when it comes into focus.

