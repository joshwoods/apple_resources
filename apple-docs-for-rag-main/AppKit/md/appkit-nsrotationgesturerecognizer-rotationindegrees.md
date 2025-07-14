

- AppKit
- NSRotationGestureRecognizer
-  rotationInDegrees 

Instance Property

# rotationInDegrees

The rotation of the gesture in degrees.

macOS 10.10+

``` source
@MainActor
var rotationInDegrees: CGFloat { get set }
```

## Discussion

This property contains the current rotation in effect for the gesture. Changing the value in this property also updates the value in the rotation property.

## See Also

### Interpreting the Gesture

var rotation: CGFloat

The rotation of the gesture in radians.

