

- AppKit
- NSAccessibility
-  screenRect(fromView:rect:) 

Type Method

# screenRect(fromView:rect:)

Returns the frame in screen coordinates.

macOS 10.10+

``` source
static func screenRect(
    fromView parentView: NSView,
    rect frame: NSRect
) -> NSRect
```

## Discussion

Given a frame in the specified view’s coordinates, it returns the same frame in the screen’s coordinates.

## See Also

### Getting Screen Coordinates

static func screenPoint(fromView: NSView, point: NSPoint) -> NSPoint

Returns the point in screen coordinates.

