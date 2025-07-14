

- AppKit
- NSRulerView
-  NSRulerView.Orientation 

Enumeration

# NSRulerView.Orientation

These constants are defined to specify a ruler’s orientation and are used by orientation.

macOS

``` source
enum Orientation
```

## Topics

### Constants

case horizontalRuler

Ruler is oriented horizontally.

case verticalRuler

Ruler is oriented vertically.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Ruler layout

var scrollView: NSScrollView?

The NSScrollView that owns the receiver to `scrollView`, without retaining it.

var orientation: NSRulerView.Orientation

The orientation of the receiver to `orientation`.

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

