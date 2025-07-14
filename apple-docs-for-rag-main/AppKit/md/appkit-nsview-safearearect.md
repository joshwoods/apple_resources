

- AppKit
- NSView
-  safeAreaRect 

Instance Property

# safeAreaRect

A rectangle in the view’s coordinate system that contains the unobscured portion of the view.

macOS 11.0+

``` source
@MainActor
var safeAreaRect: NSRect { get }
```

## Discussion

The safe area of a view reflects the area not covered by navigation bars, tab bars, toolbars, and other ancestor views that might obscure the current view. Draw content inside this rectangle to ensure it isn’t covered by other content.

## See Also

### Respecting the View’s Safe Area

var safeAreaInsets: NSEdgeInsets

The distances from the edges of your view that define the safe area.

var additionalSafeAreaInsets: NSEdgeInsets

Custom insets that you specify to modify your view’s safe area

var safeAreaLayoutGuide: NSLayoutGuide

The layout guide you use to position content inside your view’s safe area.

