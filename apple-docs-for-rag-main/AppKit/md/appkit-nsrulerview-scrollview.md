

- AppKit
- NSRulerView
-  scrollView 

Instance Property

# scrollView

The NSScrollView that owns the receiver to `scrollView`, without retaining it.

macOS

``` source
@MainActor
weak var scrollView: NSScrollView? { get set }
```

## Discussion

This method is generally invoked only by the ruler’s scroll view; you should rarely need to invoke it directly.

## See Also

### Related Documentation

var verticalRulerView: NSRulerView?

The scroll view’s vertical ruler view.

var horizontalRulerView: NSRulerView?

The scroll view’s horizontal ruler view.

### Ruler layout

var orientation: NSRulerView.Orientation

The orientation of the receiver to `orientation`.

enum Orientation

These constants are defined to specify a ruler’s orientation and are used by orientation.

var reservedThicknessForAccessoryView: CGFloat

The room available for the receiver’s accessory view to `thickness`.

var reservedThicknessForMarkers: CGFloat

The room available for ruler markers to `thickness`.

var ruleThickness: CGFloat

The thickness of the area where ruler hash marks and labels are drawn.

var requiredThickness: CGFloat

The thickness needed for proper tiling of the receiver within an NSScrollView.

var baselineLocation: CGFloat

The location of the receiver’s baseline, in its own coordinate system.

var isFlipped: Bool

A Boolean that indicates if the ruler view’s coordinate system is flipped.

