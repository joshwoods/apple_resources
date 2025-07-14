

- UIKit
- UIHoverGestureRecognizer
-  azimuthAngle(in:) 

Instance Method

# azimuthAngle(in:)

A value that represents the azimuth angle of the hovering pointing device in the specified view.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+visionOS 1.0+

``` source
@MainActor
func azimuthAngle(in view: UIView?) -> CGFloat
```

## Parameters 

`view`  

The view the angle is relative to.

## Return Value

A CGFloat that represents the azimuth angle of the hovering pointing device.

## Discussion

If the specified view is `nil`, the method returns the azimuth angle of the hovering pointing device in the gesture recognizer’s window.

This method returns `0` for devices that don’t support azimuth.

## See Also

### Supporting Apple Pencil hover

var altitudeAngle: CGFloat

A value that represents the altitude angle of the hovering pointing device.

func azimuthUnitVector(in: UIView?) -> CGVector

A value that represents the azimuth unit vector of the hovering pointing device in the specified view.

var rollAngle: CGFloat

A value that represents the current barrel-roll angle of Apple Pencil.

var zOffset: CGFloat

A value that represents the normalized distance between the screen and a hovering pointing device, such as Apple Pencil.

