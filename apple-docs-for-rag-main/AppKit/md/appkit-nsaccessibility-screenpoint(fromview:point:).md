

- AppKit
- NSAccessibility
-  screenPoint(fromView:point:) 

Type Method

# screenPoint(fromView:point:)

Returns the point in screen coordinates.

macOS 10.10+

``` source
static func screenPoint(
    fromView parentView: NSView,
    point: NSPoint
) -> NSPoint
```

## Discussion

Given a point in the specified view’s coordinates, it returns the same point in the screen’s coordinates.

## See Also

### Getting Screen Coordinates

static func screenRect(fromView: NSView, rect: NSRect) -> NSRect

Returns the frame in screen coordinates.

