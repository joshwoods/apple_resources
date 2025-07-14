

- AppKit
- NSRulerView
-  baselineLocation 

Instance Property

# baselineLocation

The location of the receiver’s baseline, in its own coordinate system.

macOS

``` source
@MainActor
var baselineLocation: CGFloat { get }
```

## Discussion

This is a y position for horizontal rulers and an x position for vertical ones.

## See Also

### Ruler layout

var scrollView: NSScrollView?

The NSScrollView that owns the receiver to `scrollView`, without retaining it.

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

var isFlipped: Bool

A Boolean that indicates if the ruler view’s coordinate system is flipped.

