

- AppKit
- NSRotationGestureRecognizer
-  rotation 

Instance Property

# rotation

The rotation of the gesture in radians.

macOS 10.10+

``` source
@MainActor
var rotation: CGFloat { get set }
```

## Discussion

This property contains the current rotation in effect for the gesture. Changing the value in this property also updates the value in the rotationInDegrees property.

## See Also

### Interpreting the Gesture

var rotationInDegrees: CGFloat

The rotation of the gesture in degrees.

