

- AppKit
- NSTextContainer
-  containerSize Deprecated

Instance Property

# containerSize

The size of the text container’s bounding rectangle.

macOS

``` source
var containerSize: NSSize { get set }
```

Deprecated

Use size instead.

## See Also

### Deprecated

convenience init(containerSize: NSSize)

Initializes a text container with a specified bounding rectangle.

Deprecated

func lineFragmentRect(forProposedRect: NSRect, sweepDirection: NSLineSweepDirection, movementDirection: NSLineMovementDirection, remaining: NSRectPointer?) -> NSRect

Calculates and returns the longest rectangle available in the proposed rectangle for displaying text.

Deprecated

func contains(NSPoint) -> Bool

Queries whether a point lies within the text container’s region or on the region’s edge—not simply within its bounding rectangle.

Deprecated

