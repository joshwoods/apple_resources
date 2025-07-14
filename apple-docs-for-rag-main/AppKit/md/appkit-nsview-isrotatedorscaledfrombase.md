

- AppKit
- NSView
-  isRotatedOrScaledFromBase 

Instance Property

# isRotatedOrScaledFromBase

A Boolean value indicating whether the view or any of its ancestors has ever had a rotation factor applied to its frame or bounds, or has been scaled from the window’s base coordinate system.

macOS

``` source
@MainActor
var isRotatedOrScaledFromBase: Bool { get }
```

## Discussion

The value of this property is true if the view or any of its ancestors has had its frameRotation or boundsRotation properties modified at any time. The value is still true if the rotation factor is changed to a nonzero value and then back to 0.

Use this information to optimize drawing and coordinate calculation. Do not use it to reflect the exact state of the view’s coordinate system.

## See Also

### Related Documentation

func setBoundsSize(NSSize)

Sets the size of the view’s bounds rectangle to specified dimensions, inversely scaling its coordinate system relative to its frame rectangle.

func scaleUnitSquare(to: NSSize)

Scales the view’s coordinate system so that the unit square scales to the specified dimensions.

var bounds: NSRect

The view’s bounds rectangle, which expresses its location and size in its own coordinate system.

func centerScanRect(NSRect) -> NSRect

Converts the corners of a specified rectangle to lie on the center of device pixels, which is useful in compensating for rendering overscanning when the coordinate system has been scaled.

var frameRotation: CGFloat

The angle of rotation, measured in degrees, applied to the view’s frame rectangle relative to its superview’s coordinate system.

var boundsRotation: CGFloat

The angle of rotation, measured in degrees, applied to the view’s bounds rectangle relative to its frame rectangle.

### Examining Coordinate System Modifications

var isFlipped: Bool

A Boolean value indicating whether the view uses a flipped coordinate system.

var isRotatedFromBase: Bool

A Boolean value indicating whether the view or any of its ancestors has ever had a rotation factor applied to its frame or bounds.

