

- AppKit
- NSRulerView
-  reservedThicknessForMarkers 

Instance Property

# reservedThicknessForMarkers

The room available for ruler markers to `thickness`.

macOS

``` source
@MainActor
var reservedThicknessForMarkers: CGFloat { get set }
```

## Discussion

The default thickness reserved for markers is 15.0 PostScript units for a horizontal ruler and 0.0 PostScript units for a vertical ruler (under the assumption that vertical rulers rarely contain markers). If you don’t expect to have any markers on the ruler, you can set the reserved thickness to 0.0.

An NSRulerView automatically increases the reserved thickness as necessary to that of its thickest marker. If you plan to use markers of varying sizes, you should set the reserved thickness beforehand to that of the thickest one in order to avoid retiling of the NSScrollView.

## See Also

### Related Documentation

var thicknessRequiredInRuler: CGFloat

The amount of the receiver’s image that’s displayed above or to the left of the ruler view’s baseline.

var markers: [NSRulerMarker]?

The receiver’s ruler markers to `markers`, removing any existing ruler markers and not consulting with the client view about the new markers.

### Ruler layout

var scrollView: NSScrollView?

The NSScrollView that owns the receiver to `scrollView`, without retaining it.

var orientation: NSRulerView.Orientation

The orientation of the receiver to `orientation`.

enum Orientation

These constants are defined to specify a ruler’s orientation and are used by orientation.

var reservedThicknessForAccessoryView: CGFloat

The room available for the receiver’s accessory view to `thickness`.

var ruleThickness: CGFloat

The thickness of the area where ruler hash marks and labels are drawn.

var requiredThickness: CGFloat

The thickness needed for proper tiling of the receiver within an NSScrollView.

var baselineLocation: CGFloat

The location of the receiver’s baseline, in its own coordinate system.

var isFlipped: Bool

A Boolean that indicates if the ruler view’s coordinate system is flipped.

