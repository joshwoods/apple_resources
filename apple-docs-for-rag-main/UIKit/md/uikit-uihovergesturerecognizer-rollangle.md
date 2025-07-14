

- UIKit
- UIHoverGestureRecognizer
-  rollAngle 

Instance Property

# rollAngle

A value that represents the current barrel-roll angle of Apple Pencil.

iOS 17.5+iPadOS 17.5+Mac Catalyst 17.5+visionOS 1.2+

``` source
@MainActor
var rollAngle: CGFloat { get }
```

## Discussion

For models of Apple Pencil that don’t support barrel-roll angle data, the value of this property is `0`.

## See Also

### Supporting Apple Pencil hover

var altitudeAngle: CGFloat

A value that represents the altitude angle of the hovering pointing device.

func azimuthAngle(in: UIView?) -> CGFloat

A value that represents the azimuth angle of the hovering pointing device in the specified view.

func azimuthUnitVector(in: UIView?) -> CGVector

A value that represents the azimuth unit vector of the hovering pointing device in the specified view.

var zOffset: CGFloat

A value that represents the normalized distance between the screen and a hovering pointing device, such as Apple Pencil.

