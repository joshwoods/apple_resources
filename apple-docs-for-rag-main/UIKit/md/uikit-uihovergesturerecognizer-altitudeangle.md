

- UIKit
- UIHoverGestureRecognizer
-  altitudeAngle 

Instance Property

# altitudeAngle

A value that represents the altitude angle of the hovering pointing device.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+visionOS 1.0+

``` source
@MainActor
var altitudeAngle: CGFloat { get }
```

## Discussion

This value is `0` for devices that don’t support altitude.

## See Also

### Supporting Apple Pencil hover

func azimuthAngle(in: UIView?) -> CGFloat

A value that represents the azimuth angle of the hovering pointing device in the specified view.

func azimuthUnitVector(in: UIView?) -> CGVector

A value that represents the azimuth unit vector of the hovering pointing device in the specified view.

var rollAngle: CGFloat

A value that represents the current barrel-roll angle of Apple Pencil.

var zOffset: CGFloat

A value that represents the normalized distance between the screen and a hovering pointing device, such as Apple Pencil.

