

- AppKit
- NSRulerView
-  requiredThickness 

Instance Property

# requiredThickness

The thickness needed for proper tiling of the receiver within an NSScrollView.

macOS

``` source
@MainActor
var requiredThickness: CGFloat { get }
```

## Discussion

This thickness is the height of a horizontal ruler and the width of a vertical ruler. The required thickness is the sum of the thicknesses of the ruler area, the marker area, and the accessory view.

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

var baselineLocation: CGFloat

The location of the receiver’s baseline, in its own coordinate system.

var isFlipped: Bool

A Boolean that indicates if the ruler view’s coordinate system is flipped.

