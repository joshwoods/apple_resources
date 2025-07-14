

- AppKit
- NSView
-  isFlipped 

Instance Property

# isFlipped

A Boolean value indicating whether the view uses a flipped coordinate system.

macOS

``` source
@MainActor
var isFlipped: Bool { get }
```

## Discussion

The default value of this property is false, which results in a non-flipped coordinate system. In a non-flipped coordinate system, the origin is in the lower-left corner of the view and positive y-values extend upward. In a flipped coordinate system, the origin is in the upper-left corner of the view and y-values extend downward. X-values always extend to the right.

If you want your view to use a flipped coordinate system, override this property and return true.

## See Also

### Examining Coordinate System Modifications

var isRotatedFromBase: Bool

A Boolean value indicating whether the view or any of its ancestors has ever had a rotation factor applied to its frame or bounds.

var isRotatedOrScaledFromBase: Bool

A Boolean value indicating whether the view or any of its ancestors has ever had a rotation factor applied to its frame or bounds, or has been scaled from the window’s base coordinate system.

