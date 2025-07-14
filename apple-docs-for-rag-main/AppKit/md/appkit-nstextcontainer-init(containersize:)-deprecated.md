

- AppKit
- NSTextContainer
-  init(containerSize:) Deprecated

Initializer

# init(containerSize:)

Initializes a text container with a specified bounding rectangle.

macOS

``` source
convenience init(containerSize aContainerSize: NSSize)
```

Deprecated

Use init(size:) instead.

## Parameters 

`aContainerSize`  

The size of the text container’s bounding rectangle.

## Return Value

The newly initialized text container.

## Discussion

The new text container must be added to an NSLayoutManager object before it can be used. The text container must also have an NSTextView object set for text to be displayed. This method is the designated initializer for the `NSTextContainer` class.

## See Also

### Deprecated

func lineFragmentRect(forProposedRect: NSRect, sweepDirection: NSLineSweepDirection, movementDirection: NSLineMovementDirection, remaining: NSRectPointer?) -> NSRect

Calculates and returns the longest rectangle available in the proposed rectangle for displaying text.

Deprecated

func contains(NSPoint) -> Bool

Queries whether a point lies within the text container’s region or on the region’s edge—not simply within its bounding rectangle.

Deprecated

var containerSize: NSSize

The size of the text container’s bounding rectangle.

Deprecated

