

- AppKit
- NSView
-  safeAreaLayoutGuide 

Instance Property

# safeAreaLayoutGuide

The layout guide you use to position content inside your view’s safe area.

macOS 11.0+

``` source
@MainActor
var safeAreaLayoutGuide: NSLayoutGuide { get }
```

## Discussion

The layout guide in this property reflects the view’s frame minus its safe area insets. Use this guide to configure layout rules relative to this safe area.

## See Also

### Respecting the View’s Safe Area

var safeAreaRect: NSRect

A rectangle in the view’s coordinate system that contains the unobscured portion of the view.

var safeAreaInsets: NSEdgeInsets

The distances from the edges of your view that define the safe area.

var additionalSafeAreaInsets: NSEdgeInsets

Custom insets that you specify to modify your view’s safe area

